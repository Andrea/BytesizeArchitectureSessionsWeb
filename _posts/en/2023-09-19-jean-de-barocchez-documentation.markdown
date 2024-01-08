---
title: Using Bytesize Sessions to improve documentation practices by Jean de Barochez at Payfit
layout: post
lang: en
author: Jean de Barochez
categories: usage-report Payfit
date: 2023-09-19  13:53:25
---

This is an article by [Jean de Barochez](https://mastodon.social/@jdebarochez), where he describes his thoughts and practices when it comes to documentation and how he uses Bytesize Architecture Sesssions in the context of documentation.

---


Documentation is an important part of software development, with a lot of opportunity for improvements and I recently discovered a workshop format to solve my pain points.

## About documentation


I have never been keen on the documentation practice. This article is the retrospective of my own experience and different scenario I met.

Over the years, I learned documentation is hardly maintained, often forgotten, never targets the right audience. The process review, and fool proofing is often light. We often find a dedicated author and a lack of shared ownership among a team. When the author leaves, a handover may be done, yet again often a light process. Documentation may be reviewed upon completion, it does not follow the same care as the code it reflects. In the recent years, we found an increase toward documentation as code tools (Structurizr, OpenAPI specifications). These greatly helps in having different views over the code. The closer the documentation is to the code, the more consistent it stays. On the other hand, documentation manually written in a Notion page, rarely survives the passage of time. Architecture diagrams often fall short over the iterations, refactoring and evolutions.

When discussing with peers, I often draw my mental model of a high level architecture diagram on the fly, specifically for the context we are in, ignoring existing diagrams, which serve a different purpose, yet represent the same components. It's probably a problem of documentation structure and search. A lot of waste is generated this way, ephemeral diagram for the purpose of sharing knowledge with a group of person as a support for an initiative. Even though we invest a lot of time in documentation, review and maintenance, we fail to reuse this documentation for another purpose than knowledge.

This is where the following practice helped me to change my understanding about documentation.

### Bytesize Architecture Sessions

I discovered at a virtual-ddd meetup the framework [Bytesize Architecture Sessions](https://bytesizearchitecturesessions.com/) from [Andrea Magnorsky](https://www.roundcrisis.com/). It's a workshop framework to share the same understanding of a system among the participant. Bonus, you get great documentation at the end of a fun session. From there on, I will consider you checked out the website and are familiar with the framework.

The "Alone together" part is the key part to me of the session. People naturally focus on what they believe is important from their point of view. With diverse people, it gives a rich output of the session. Some may be traumatized by a previous incident, or an underestimated edge case or a detail only them are aware of. Some other may not have enough confidence to share, underestimating their knowledge, ability or fearing the exposure ("wait, you're the senior and you don't know?!"). At first, people would be surprised by their unfinished work. I try to warn ahead to not focus on doing something perfect since we'll redraw later in the consensus. I found interesting to push people who even don't know the system to exercise:

- it makes them think about the problem, and adopt it
- they may challenge the solution with out-of-the-box thinking
- make mistakes and learn edge cases
- ...

The consensus part is the second most important to me. So much happens in this part. Questions are raised, curiosity is answered, we can even review the design altogether. "This should not be this way. Why not like this?", "What happens when ...?", "Are we still doing it like this?!", "Oh this is deprecated and we forgot to clean?", etc.

When using a live system as goal, it's great to share understanding of the system. When setting the goal for a change, we design and document first the solution, then head for implementation, easily going back and forth between both. We reach a living documentation.

### Applications

With the team I'm part of, we practiced it several times. We also applied in two other situations: in discussion with peers, as well as cross team alignment for integration contracts.

#### A team ceremony

This is where it makes more sense as the iterative approach helps to continuously build the documentation until nothing is left to draw. The past quarter, the team and I were constrained to work two features in parallel. I'll keep for a later post why it was a difficult experience. Yet, the **Bytesize Architecture Sessions** helped us bridge the gap between the members about what has been done on each side. We did it after the implementation was done. People adopted both contexts. The design and implementation were reviewed. Finally, a documentation was agreed upon.

#### With a peer

I discovered a new framework and I wanted to share it with many more people. I was having a session with someone with a different experience on the system. We both had one bit of an undocumented legacy process, I proposed to spend some time alone to draw our knowledge and then we searched for consensus, noting down questions, uncharted areas and connecting dots.

#### Cross team interactions

When dealing with reorganization, scopes change, knowledge is transferred and usually this is time for a load of Notion page transferred from one team to the other. The knowing team will expect questions for a few months, until the team taking over will be comfortable with the system.

Applying the Bytesize Architecture Session helped in adopting the problem, collaborate to the documentation, practice the implementation as we had to look up the code. Instead of spending few hours in presentations, with one way discussions, rare questions, overflow of information, we actually spent fun times to draw together and sharing why we did things in a different manner, which incident happened and where.

## Conclusion

Documentation is finally something fun to do, with a collaborative approach like the Bytesize Architecture Session. The output of each session are always carefully crafted, and great outcome for the team with this shared understanding of the system.

--- 

Jean is a software engineer with affinities to software architecture, domain driven design and gardening. 🧑‍🌾
Learn more about him on [mastodon](https://mastodon.social/@jdebarochez).

If you have used Bytesize Architecture Sessions and feel like sharing your experience reach out to Andrea via [mastodon](https://types.pl/@roundcrisis/) or [LinkedIn](https://www.linkedin.com/in/magnorsky/) so we can make it happen.