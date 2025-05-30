Contributor's Guide
'HOW TO CONTRIBUTE TO OPEN SOURCE' accepts PR's (pull requests) from newbies only. This is to help newbies get familiar with the contribution processes.

Issues can be submitted by anyone - either seasoned developers or newbies.

Contents

Choosing an Issue
Getting Started
Submitting a Pull Request
Adding to the Main README
Adding to Non-English README
Adding to the Project File
Notation and terminology
Helpful Resources
Choosing an Issue
Before getting started and setup with contributing, you'll want to look at and choose an issue to work on. Here is a basic workflow you want to work from:

Search through issues
Find issue you want to work on
Check if someone else has already worked on and made a pull request on said issue
(Optional) Double check pull requests for someone who has worked on the pull request
If you have gotten that far, then you can go ahead and work on the issue. Below are more detailed instructions based on the basic workflow above.

You can find open issue here.

Once you've found an issue you want to work on, take a look at the issue to see if anyone else has made a pull request for this issue yet.

You can tell if someone has correctly referenced and worked on an issue if in the issue you find some text saying, the following:

This was referenced on ____

where that ____ is the date and below it is the pull request of another individual working on that issue. Here is an example of what this looks like.

To be extra sure no one has worked on it, you can take a look at the pull requests as well to see if anyone has made a similar pull request.

If you've gotten this far, then you can continue on with the next section on "Getting Started" to working on your first pull request and contribution to our repository.

Getting Started
If you are new to Git and GitHub, it is advisable that you go through GitHub For Beginners before moving to Step 2.

Fork the project on GitHub. Help Guide to Fork a Repository.

Illustration for How to Fork a Repository

Clone the project. Help Guide to Clone a Repository

Create a branch specific to the issue you are working on.

git checkout -b update-readme-file
For clarity, name your branch update-xxx or fix-xxx. The xxx is a short description of the changes you're making. Examples include update-readme or fix-typo-on-contribution-md.

Open up the project in your favorite text editor, select the file you want to contribute to, and make your changes.

If you are making changes to the README.md file, you would need to have Markdown knowledge. Visit here to read about GitHub Markdown and here to practice.

If you are adding a new project/organization to the README, make sure it's listed in alphabetical order.
If you are adding a new organization, make sure you add an organization label to the organization name. This would help distinguish projects from organizations.
Add your modified files to Git, How to Add, Commit, Push, and Go.

git add path/to/filename.ext
You can also add all unstaged files using:

git add .
Note: using a git add . will automatically add all files. You can do a git status to see your changes, but do it before git add.

Commit your changes using a descriptive commit message.

git commit -m "Brief Description of Commit"
Push your commits to your GitHub Fork:

git push -u origin branch-name
Submit a pull request.

Within GitHub, visit this main repository and you should see a banner suggesting that you make a pull request. While you're writing up the pull request, you can add Closes #XXX in the message body where #XXX is the issue you're fixing. Therefore, an example would be Closes #42 would close issue #42.

Submitting a Pull Request
What is a Pull Request?

If you decide to fix an issue, it's advisable to check the comment thread to see if there's somebody already working on a fix. If no one is working on it, kindly leave a comment stating that you intend to work on it. By doing that, other people don't accidentally duplicate your effort.

In a situation where somebody decides to fix an issue but doesn't follow up for a particular period of time, say 2-3 weeks, it's acceptable to still pick up the issue but make sure that you leave a comment.

Note: Every open-source project has a CONTRIBUTING.md file, please make sure to read this before you open up a pull request; otherwise, it may be rejected. However, if you do not see any CONTRIBUTING.md file, you can send a pull request but do it in a descriptive manner.

Adding to the Main README
The main README.md file contains a list of useful resources for beginners who want to contribute to open source.

You can contribute to this page by adding a Markdown-formatted link.

It should look similar to the one below.

- [Title of the page](www.websitename.com/slug-name-here) - Add a description of why I should look at this site.
When in doubt, take a look at the current list of items to get an idea of how you should format your contribution.

When adding your contribution to the list, please add your link to the most appropriate section. If you are unsure, feel free to ask in your pull request or comment in an issue asking for guidance.

If a video link is added, try to add in the length of the video as well, as shown below.

- ["Complete Guide to Open Source - How to Contribute"](https://www.youtube.com/watch?v=yzeVMecydCE) (41:52) - Learn why and how to contribute to open source software with Eddie Jaoude.
Adding to Non-English README
The main README.md file is written in English. That file will be the template for all of the other languages.

This repository is about contributing to open source and generally, translation is important to reach diverse audiences. It is recommended that you provide language-specific resources links instead of the English-resource links.

The non-English README files are named README-XX.md, where xx is the two letter language code for the language.

You can contribute to the non-English README files by taking links that are in the English README but are not in the language of your choosing. When making a pull request with these changes, please tag someone who can verify your language contribution by adding @ in front of their GitHub username to the pull request.

If your language does not exist yet, feel free to start it yourself. If you decide to do this, please add more than just the title. If you do not have the time to create one, feel free to create an issue to crowdsource help.

Adding to the Project File
We have a PROJECT.md file to help curate a list of projects and organizations that are friendly to contributions.

If you know of a project or organization that fits this description, feel free to add them to this list.

The list is generally formatted like below.

- [freeCodeCamp](https://www.freecodecamp.org/) (org)
    - [freeCodeCamp](https://github.com/freeCodeCamp/freeCodeCamp/) (project)
        - [Contributing guide](https://github.com/freeCodeCamp/freeCodeCamp/blob/master/CONTRIBUTING.md)
        - Issue labels:
            - [first-timers-only](https://github.com/FreeCodeCamp/FreeCodeCamp/issues?q=is%3Aopen+is%3Aissue+label%3Afirst-timers-only)
So you have the project page itself at the top. This can be the front-facing website or GitHub page.

Next, we ask to link to the contributing page. This will give direction to people who want to contribute. This file is important to read so that you understand what is expected from contributors who have not contributed to their project before.

Lastly, we want to link to beginner-friendly labels. These are typically Good First Issue or something similar.

Notation and terminology
This section will list any notations, terminology, or words that we will keep consistent.

"Open Source" will be capitalized unless it is within a article or video title
Helpful Resources
Pro GIT Book

Try Git

Git/ Git Hub on Windows
