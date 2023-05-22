# Open Source & Contributing Notes

## Basic README.md format

Try to include the following section headings in your repo README file:


1. Description - absolutely necessary
2. Table of Contents - only include if your README is long
3. Installation - not necessary if it's a simple HTML, CSS & vanilla JS project.
4. Usage - not sure about this one
5. License - not necessary if it is a simple project
6. Contributing - you need this if you want contributors
7. Code of Conduct - same as above
7. Tests - skip if you do have a testing library as part of the repo
8. Questions - this could be helpful

## Best Of

1. License for your repo: [Choose a License](https://choosealicense.com/)
   1. I prefer the [MIT Version](https://choosealicense.com/licenses/mit/). Just enter your GitHub repo link in the right sidebar.
1. Contributing Templates:
   1. [Contributor guidelines template](https://opensource.com/life/16/3/contributor-guidelines-template-and-tips)
   1. Check [contributing-template](https://github.com/nayafia/contributing-template/blob/master/CONTRIBUTING-template.md)
   1. [Example 1](https://gist.github.com/briandk/3d2e8b3ec8daf5a27a62), [Example 2](https://gist.github.com/PurpleBooth/b24679402957c63ec426)
1. [Contributor Covenant](https://www.contributor-covenant.org/): A Code of Conduct for Open Source Communities

## Open Source

Notes from Eddie Jaoude & freeCodeCamp

- Labels: used to find your repos - need issues with labels – javascript,
- review other people’s Prs to see what they do
- find gist: [GitHub starred gists](https://gist.github.com/starred)
- Must have elements in all OS projects:

1. License: If a project does not have an open-source license, then it is not open source
   1. The license helps protect contributors and users. Businesses and savvy developers usually won't touch a project without this protection: [Choose a License](https://choosealicense.com/)
1. README file: explains how to get started with a project. It lists the requirements for contributing to the project
   1. A good README should contain everything a potential contributor would want to know about the project
1. Contribution Guidelines: These are guidelines that help people who contribute to the project know exactly what is expected from them: [Contributor guidelines template](https://opensource.com/life/16/3/contributor-guidelines-template-and-tips) - no longer any good
1. Code of Conduct: a document that establishes your expectations for how your contributors and participants behave: [Code of Conduct](https://opensource.guide/code-of-conduct/)

- Issue Tracker – a contributor can create an issue and link it to a pull request and fellow contributors can opt in to try and fix it
- Pull Requests - tell others about changes you've pushed to a branch in a repository on GitHub. Once a pull request is opened, you can discuss and review the potential changes with the collaborator and add follow-up commits before the're merged into the base branch
- do everything on the insights tab to make sure your repos are good

## Places to find contributions

1. [First timers only](https://www.firsttimersonly.com/)
1. [GitHub first contributions](https://github.com/firstcontributions/first-contributions)
1. [Specref API](https://github.com/tobie/specref) - not sure what this one is
1. [GitHub Docs](https://github.com/github/docs)
1. Find new issues: [Mariner Issue Collector](https://github.com/indeedeng/Mariner-Issue-Collector)
1. [GitHub Odoo](https://github.com/odoo/odoo): a suite of web based open source business apps
1. [GitHub Good First Issues](https://github.com/iedr/goodfirstissues)
1. [Good First Issues](https://24pullrequests.com/) and [Good First Issues website](Good First Issues)
1. [CodeTriage](https://www.codetriage.com/)

## How to choose an Open-Source Project

1. Check if it has a license, 
2. check the date of the last commit (is it recent?), 
3. check the # of contributors, 
4. how often do they make commits?

Also, look for: 

1. open issues, 
2. time for maintainers to respond, 
3. are there active discussions, 
4. are issues closed regularly, 
5. are there open pull requests

### Tips

- Also search: `is:open is:issue archived:false label:"good first issue" language"javascript"`
- Another Tip: search the project for "To D" or "ToDo" or "To-Do"- they often get forgotten about – find one, raise an issue, then fix it

## How to make money from open source

Github now has a sponsorship 

- People can sponsor and github doesn’t take anything but they can match it
- Click the Settings tab and go to the FEatures section 
- Click the checkbox for Sponsorships 
- There is a card with the title _Display a "Sponsor" button_ with the text _Add links to GitHub Sponsors or third-party methods your repository accepts for financial contributions to your project_
- There is also a button that says _Set up sponsor button_ 
- Clicking it takes you to a file named _FUNDING.yml_ - in that file are notes to add links to things like Patreon, Open Collective, Ko-fi and many more.

## TAGS

A tag/release is where you are happy with the state of the project> It means it is a production ready asset. A tag is made up of multiple comits between tags – or they are after commits, a save point – and a tag is a collection of commits.

## Miscellaneous

`config.yml`

- YAML/yml files start with 3 dashes and end with 3 dots which allows you start and stop the the yaml data and allows you to have multiple in one file 
- Though the ending 3 dots are optional – you have key-value pairs 
- Values can be strings, integers, floats, booleans, arrays, lists and dictionaries – use the vscode extension YAML
- Can be `.yml` or `.yaml` – both are good – yaml can detect strings so you don’t actually need the quotes but you need quotes when you have numbers/integer that needs to be interpreted as a string
- For lists use an slight index and a dash then space like markdown
- The dictionary data type has elements that have elements (Attibutes) inside it – or more importantly you can do nesting
- It's important to have some pull requests and issues - and branches greater than 1 – main/master, develop, feature1, feature2, … but not more than 9,
- Open source is more about communication and collaboration
- README – can include technologies needed to run the app like node or MySQL – what is the goal of the project, why it is important, why people should get involved
- Great GitHub README profiles: https://github.com/nhcarrigan/nhcarrigan | https://github.com/santoshyadavdev/santoshyadavdev | https://github.com/salitha10/salitha10 | https://github.com/iresharma/iresharma | https://github.com/joesinghh |
- Great link: [Awesome GitHub Profile README](https://github.com/abhisheknaiidu/awesome-github-profile-readme)
- [Awesome GitHub profiles](https://github.com/EddieHubCommunity/awesome-github-profiles/blob/main/profiles.md)
