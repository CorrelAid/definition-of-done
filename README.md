# definition-of-done
A Definition of Done for CorrelAid projects

# What is a Definition of Done?

Especially in volunteering contexts, it is important to have concrete achievements and moments of being "really done" with a task. 

> Proverbially, to get an answer to that, the question to ask is, “I know that you are done, but are you DONE-done?”. ([Source](https://www.agilealliance.org/glossary/definition-of-done/))

But how do we know that we're really done and have not forgotten anything important? At CorrelAid, we use a Definition of Done. 
A Definition of Done (DoD) is a tool from Scrum, a popular framework that is often used in software development. It "creates transparency by providing everyone a shared understanding" of what "being done" means ([Scrum Guide](https://scrumguides.org/docs/scrumguide/v2020/2020-Scrum-Guide-US.pdf#zoom=100), p.12).

We know that it can be hard to pay attention to things like code quality and documentation when your time resources are scarce - as is always the case with volunteering. However, we have found that things like good documentation and structure are a key factor for the long-term success and impact of CorrelAid projects. Broken or poorly documented code is very hard to use or adapt by NPO partners who are often coding beginners. Without a good README, it will be hard to impossible to for someone at CorrelAid to help out the NPO if a problem comes up a couple of months later when you're already off the project. And having old, irrelevant code or visualizations in your repository is probably very confusing for someone not familiar with the project. 
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
- **Code documentation**: Function/class documentation is up to date (e.g. roxygen / documentation strings)
- **Unit tests**
    - existing unit tests pass
    - if possible: new code is properly tested 
    - unit test coverage >xx% 
- **Standards**: no errors on coding standards (e.g. lintr, Black)


# Related Resources

## coding style recommendations

## Python setup recommendations
