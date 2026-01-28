---
title: Diagramming Tools
layout: single
classes: wide
permalink: /tools/
author: Andrea Magnorsky
---

What are good tools to use with Bytesize Architecture Sessions?


## During a session


During a session use any collaborative board all the participants of a sessions can **easily** access. 

### In person

{{ site.images }}

![whiteboard]({{site.url}}/images/whiteboard.png)


* Use paper and markers for [Alone Together]({{site.url}}/running-your-first-sessions) 
* A whiteboard (don't forget working whiteboard markers for everyone)is extremely practical for [Convergence]({{site.url}}/running-your-first-sessions)  
* Sticky notes to add comments about assumptions and other areas you might wa to come back to.
* Write down questions that you have discussed for over 2 minutes and have not answered
> Top tip 
> Take pictures of final result.



### Online 

If you are working online, anything that would enable everyone that should take part to change the diagram at the same time is a good option. 
A popular online board at the moment is Miro. If you are working on Miro, having multiple Bytesize Sessions in one board can be a really nice way to see progression and note diagrams that need updating. You could lay it out using frames so that it looks like this:

![Miro board]({{site.url}}/images/miro-bas.png)

* For alone together give each person a frame
* For convergence zoom into the frame with title Convergence board. I generally update the title of the Frame to: Together - <the goal of the session>.
* Do the retro in a nearby area.

This is just a suggestion, the best tool is to use what that participants are already familiar with, at least at the start.

## After a session

Once the collaboration session finishes, it is recommended to clean up the diagram and make sure it follows whatever standard notation is recommended for the given diagram. At a minimum, a diagram should have: a title, the type of diagram and a legend section. Adding date and scope of the diagram and a brief description can be useful too.

When you have just one or two diagrams it's probably best to not worry too much about where to store them. This is a good time to observe how people interact with the diagram. 
Making the decision of how to manage these diagrams will dictate how they will be used. Try things and listen to the users. 

Answering these questions might help finding the best option

* What kind of diagrams are you making?  

Consider who should have access to update the diagrams or models, these are live documents.

* What tooling do you need to generate them?

If you are using C4 [PlantUml](https://github.com/plantuml-stdlib/C4-PlantUML), [Structurizr](https://structurizr.com/) and [IcePanel](https://icepanel.io/) are popular options. Please visit the tools section of the [the c4 model website](https://c4model.com/tooling) too, for a more comprehensive review of the tools. 
Some of these tools would enable you to navigate and update the model as you are there but you might need to ensure access, and payment in some cases, for that access.

This is where your context is important, access to the tools and capability to edit the diagrams is what will dictate how often these documents are updated, and you want to encourage updates inline with changes to the system they represent.

* If you generate diagrams rather than create navigable models. How to easily find them?

This question also depends on how your organisation works. The principle to apply here is to focus on access to view and edit for all the people creating the diagrams.

If you actively use a collaboration website such as [Wiki software](https://en.wikipedia.org/wiki/List_of_wiki_software), Confluence, Notion, or similar you probably want to be able to easily see your diagrams there. If you need code to generate to diagrams, ideally it should be in the codebase that the diagrams model. When you put these two things together, you might be tempted to automate this problem, don't rush to a solution... look for the access patterns rather than what people ask and find a solution that will enable the live aspect of the diagrams to surface. 

These are some (surprising?) options that worked for some organisations:

* More people with access to edit the codebase that contains the diagrams (after some light training on how to use plantUml)
* Keep the diagrams in the diagramming tool, but remove anything invalid every few months
* The person that last updates the diagram in code is responsible for updating the collaboration site (but there is just one place to do it)

What worked for your organisation? Keen to hear about it  

