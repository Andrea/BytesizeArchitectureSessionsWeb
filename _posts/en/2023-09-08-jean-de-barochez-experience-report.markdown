---
layout: single
classes: wide
title:  Experience report of Using Bytesize Architecture Sessions by Jean de Barochez at Payfit
date:   2023-09-28 13:53:25
lang: en
author: Jean
categories: 
- case study
- Payfit
- video
tags:
- case study
- bytesize architecture sessions
---

This is an article by Jean de Barochez, where he describes how his team uses **Bytesize Architecture Sessions** at [PayFit](https://payfit.com/).

---




## Bytesize Architecture Sessions for teams at PayFit

### Context

In my company, we're developing a SaaS payroll software. My team specifically is in charge of orchestrating payroll closings, as well as publishing payslips for employees. As any fast growing startup, some core capabilities grew old and in order to enable new development, we took the tasks of progressively revamping our payslip generation system, use case by use case. At the same time, we also had parallel improvements to develop, which forced the team to split on different initiatives. During this time, we also had Summer holidays for every members. When everyone returned, the knowledge was scattered in the team. We were unable to decide how to complete one of the use case, as we were not understanding the problem the same way.

This is where we started to organize *Bytesize Architecture Sessions* to capitalize on the knowledge we have so far, to document how our components interact with each other, annotated with unanswered questions and key decisions made. To picture it, imagine a Miro board, using this [C4 Model template](https://miro.com/miroverse/c4-model-getting-started-workshop/), with different set of Context Diagram and Container Diagram, to keep a high level and give the team enough context to understand the whole flow.

What I describe after is a session we performed to design together how this use case was designed. It was a session of 4 engineers for 1h30.

### Setting up the goal

We always start from the context diagram from C4 Model: the higher level, showing the personas and their interactions with the system. Before this session, I previously had setup a Context Diagram telling the following story:

> When a payroll administrator requests to close their payroll, and after waiting a moment, their employees are notified of a new payslip available they can access on their personal employee space. In case of one error with one payslip for a company, we don't publish any payslip to any employees.

We discussed the scope of the exercise for 5-10 minutes. We always try to narrow down the boundaries of the problem to focus on a single problem at a time. This time, we had questions to refresh everyone mental model. We reminded ourselves our constraints for this:

- release should be transparent to users
- the behavior remains the same
- the change is purely technical on the live system, without downtime.

### Alone together

During 8 minutes, each participant duplicated an empty frame to draw each respective mental model of the change they would do. We are not yet master in C4 modelling. We believe the important part of the exercise is to convey an opinion. What's important is to draw quickly the components we need. For this, we added to the board a legend of components we can reuse.

![A Miro legend of C4 Model Container level with shapes for personas, databases, APIs, external systems and container dependencies](/images/jdb-article3.alone-together-legend.png)

We all had something to share, more or less detailed, depending on the degree of familiarity and ability to model quickly, but all were a working solution. One by one, we presented our diagrams and asked questions about meaning of some dependencies.

### Consensus (this section is now called Convergence in BAS - January 2026)

During 35 minutes, we discussed how we would implement it. In this session, the major part of the feature implementation quickly reached consensus. We all had similar solutions, while discarding alternatives approach. In our context, an event driven approach would be best to decouple some components, but it would increase the error management. On top of that, our user interface is not ready for showing a progress bar with the number of payslips being generated. Some alternatives are ideal, but unreachable in a short term.

I took the pen to draw the consensus. We started from the frontend, while the other participants were telling what to pick, copy/pasting me boxes from their diagram or re-creating from scratch.

We have today a process manager doing the orchestration of the payroll closing steps. It would be in charge to loop over every employees to generate a payslip. We create batches of _X_ payslip generation at a time, knowing most of our customers have less than _X_ employees. If a batch fail, the process manager halts the execution.

The debate in our case went in length about release strategy. How do we change a working system with one that is supposed to do the same? We took an approach of a feature flag to enable the behavior progressively, and easily rollout in case of unknown unknown. Our diagram was showing were the feature would be enabled or not. We work in a distributed system and feature flag updates may take time to rollout, thus we had to detail how to cope with overlapping execution between the old and the new system.

We listed few tasks for later:

- when can we deprovision the legacy service?
- what metrics should we look into on this new flow?
- what name for our feature flag?

We took the time to document properly on the fly, discussing C4 component labels and dependencies.

### Session summary

The summary in our case was quick, having a quickly reached convergence. We listed the key steps to perform. What was amazing, is that at this point, we had a clear understanding of the implementation, a documentation diagram to support it and a plan everyone agreed on.

### Mobbing

We did a break, then started a mob programming session. With the momentum and the knowledge we accumulated, people were keen on starting development and get rid of the task. A major part of the tests and code were implemented. Only was left details regarding environment and feature flag configuration, that one person could continue the day after, providing pull requests to the others to approve the completion of the task.

## Conclusion

We may sometimes work on small isolated tasks (maintenance, investigation, etc). We are not always there all the time neither as we may be absent, or working on a different priority. Yet, to work as a team and collaborate on it, we need everyone to have the same understanding of the problem. This requires for people to be in the mood to participate, as well as feeling in a safe environment to share their mental model. This greatly increases the adoption of the problem and the quality of the debate for the consensus. We also have to ensure everyone understand this is also for them, to grow their understanding of how this will help them to contribute to it.

We found in Bytesize Architecture Sessions a powerful way to keep people up to date on particular topic. Given a complex task at hand, which changes a lot the system and its technical behavior, using a session to then kick start a mob programming session helped in sharing knowledge, and having everyone contributing to the problem at hand.


--- 

Jean is a software engineer with affinities to software architecture, domain driven design and gardening. 🧑‍🌾
Learn more about him on [mastodon](https://mastodon.social/@jdebarochez).

If you have used Bytesize Architecture Sessions and want to share your experience in this website, reach out to Andrea via [mastodon](https://types.pl/@roundcrisis/) or [LinkedIn](https://www.linkedin.com/in/magnorsky/) so we can make it happen.