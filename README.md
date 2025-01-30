# definition-of-done
A Definition of Done for CorrelAid projects

# What is a Definition of Done?

Especially in volunteering contexts, it is important to have concrete achievements and moments of being "really done" with a task. 

> Proverbially, to get an answer to that, the question to ask is, “I know that you are done, but are you DONE-done?”. ([Source](https://www.agilealliance.org/glossary/definition-of-done/))

But how do we know that we're really done and have not forgotten anything important? At CorrelAid, we use a Definition of Done. 
A Definition of Done (DoD) is a tool from Scrum, a popular framework that is often used in software development. It "creates transparency by providing everyone a shared understanding" of what "being done" means ([Scrum Guide](https://scrumguides.org/docs/scrumguide/v2020/2020-Scrum-Guide-US.pdf#zoom=100), p.12).

We know that it can be hard to pay attention to things like code quality and documentation when your time resources are scarce - as is often the case with volunteering. However, we have found that things like good documentation and structure are a key factor for the long-term success and impact of CorrelAid projects:

- Well documented code can be adapted by NPO partners who are often coding beginners. 
- With a good README, someone at CorrelAid can help out the NPO if a problem comes up a couple of months later when you're already off the project. 
- Not having old, irrelevant code or visualizations in your repository makes it easier for someone not familiar with the project to find the relevant files and data. 
- ...

**All this really makes a difference for the long-term success of a project**. 

# How do you use the DoD?
First of all, the Definition of Done is a reminder for you as a volunteer to not forget the "chores" that are so important for a quality project outcome. When working on an issue/task, you can come back to the DoD to not forget something important like documenting your code properly. 
Second of all, it serves as a "checklist" for you as a team to see whether something can be really considered "done". In your regular meeting, you review issues that have been worked on and are "done" against the DoD to see whether they're "really done". If yes, then you can close the issue - well done (pun intended!)! 🎉  If something is missing, the issue/task is not _really_ done and cannot be closed - but it will be by the next meeting, just some little things left to do! :) 💪

# Definition of Done

- **Functionality**: the code runs / has no defects
- **Code documentation**: the code itself is properly documented
- **Project documentation** such as README/wiki is updated where necessary
    - scope/features of project: what does this project do? How can you run it?
    - setup of project
        - data requirements (files, folders)
        - software requirements (packages, other tooling)
    - developer documentation: things like the definition of done, agreed upon standards, ...
- **Peer Review**: someone else has had a look at the code and tested it on their machine
- **Git**: the code is ready to be merged to the main branch or is already on the main branch
- **Clean Repository**: old, outdated code and files are deleted
- **Consistent code style**: code is styled consistently

## R / Python packages
Some additional points for projects that wrap code in R / Python packages:

- **Code documentation**: Function/class documentation is up to date (e.g. roxygen / documentation strings)
- **Unit tests**
    - existing unit tests pass
    - if possible: new code is properly tested 
    - unit test coverage >xx% 
- **Standards**: no errors on coding standards (e.g. lintr, Black)


# Tips for implementation
## General

See the docs [here](https://docs.correlaid.org/project-manual/project-team/best-practices/collaboration#general-best-practices).

## R 
See the documentation about [R best practices here](https://docs.correlaid.org/project-manual/project-team/best-practices/r).

## Python
See the documentation about [Python best practices here](https://docs.correlaid.org/project-manual/project-team/best-practices/python).

Feel free to submit best practices to Leo or directly to the [documentation repo](https://github.com/correlaid/docs).
