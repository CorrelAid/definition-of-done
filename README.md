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

#### How to document code
Documenting your code should always be less about the "what" and more about the "why". However, if you are writing code which might be a bit more advanced/complex, adding some comments about _how_ it works is also useful, especially for the less experienced team members.

#### Peer review 
Peer reviewing someone else's code involves three things:

1. test the code on your machine
2. provide feedback (possibly suggesting changes)

Whenever the skills of the team allow for it, you should use [branches](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches) and [pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) for this. [Pull request reviews](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews) are a great way to directly suggest changes.

If a team member is still quite new to Git, a file-driven "review process" (e.g. `data_cleaning_jack.R`) is also acceptable as to not overwhelm them with Git. You can leave comments in the file and commit it back to Git or discuss your feedback in a GitHub issue. Always be kind to team members with less experience.

## R 
#### code styling
You can use the [styler](https://styler.r-lib.org/) package.

```
styler::style_dir()
```

You can also adapt the default tidyverse style to your liking (e.g. different identation). What matters is the consistency.

#### code linting
The [lintr](https://github.com/r-lib/lintr) package provides linting functionalities.

## Python
## code styling and linting 

There are various libraries for styling and linting code, some covering both aspects.

See [this blog post](https://deepsource.io/blog/python-code-formatters/) for an overview over code styling libraries. [This one](https://realpython.com/python-code-quality/) goes into more detail about the difference between linting and styling/formatting.
