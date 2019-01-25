<!---

TASK LIST:

  * Use cp -rf *.* to copy all of the files and directories in this repository
    to the starter repository for this assignment
  * Change into the directory for the starer repository
  * Update the header (e.g., #) to only give the name of the assignment
  * Update the first paragraph to include the commented-out content
  * Change the link in the # Problems section to point to this lab's starter
  * Create the assignment in the GitHub Classroom, noting the URL
  * Test the assignment by accepting it with your own GitHub account
  * Check to ensure that your GitHub repository is created correctly
  * Share the assignment link with all of the students using email or Slack

PROBLEMS?

  * Contact Gregory M. Kapfhammer by email or Slack
  * Raise an issue in the GitHub repository for this assignment

-->

# cs302-S2019-practical2-starter

Designed for use with [GitHub Classroom](https://classroom.github.com/), this
repository contains the starter for Practical 2 in Computer Science 302. Since
the Travis builds for this repository will initially fail (as evidenced by a
red &#x2717; appearing in the commit logs instead of a green &#x2714;), the
programmer is responsible for completing all of the steps needed to satisfy the
requirements for the assignment, thus causing a &#x2714; to instead appear in
the commit logs.

## Introduction

This assignment requires a programmer to fix the mistakes in a static web site
using the Markdown programming language. You will repair a web site with, for
instance, headers, paragraphs, a link, and an unordered list. Please note that
you will be repairing a Markdown file that must adhere to the standards
described in the [Markdown Syntax
Guide](https://guides.github.com/features/mastering-markdown/). Additionally,
this file should both adhere to the Markdown standards established by the
[Markdown linting tool](https://github.com/markdownlint/markdownlint) and the
writing standards set by the [Proselint tool](http://proselint.com/). Then, you
will use a Markdown conversion tool, called [Pandoc](https://pandoc.org/) to
convert your Markdown to HTML and then run a web server to provide local access
to the static web site. Ultimately, your goal is to find and fix all of the
mistakes in the provided Markdown file.

The source code in the `answers.md` file must also pass additional tests set by
the [GatorGrader tool](https://github.com/GatorEducator/gatorgrader). For instance,
GatorGrader will check to ensure that your main file contains the required
header and that, for instance, it contains the correct number of subheaders.
GatorGrader will also check that you made the required number of commits to your
repository and that your writing contains the specified number of paragraphs and
sentences per paragraph. More details about the GatorGrader checks are included
later in this document and in the assignment sheet.

When you use the `git commit` command to transfer your source code to your
GitHub repository, [Travis CI](https://travis-ci.com/) will initialize a build
of your assignment, checking to see if it meets all of the requirements. If both
your source code and writing meet all of the established requirements, then you
will see a green &#x2714; in the listing of commits in GitHub. If your
submission does not meet the requirements, a red &#x2717; will appear instead.
The instructor will reduce a programmer's grade for this assignment if the red
&#x2717; appears on the last commit in GitHub immediately before the
assignment's due date.

A carefully formatted assignment sheet for this project provides more details
about the steps that a computer scientist should take to complete this
assignment. You can view this assignment sheet by visiting the listing of
laboratories on the course web site.

## Learning

If you have not done so already, please read all of the relevant [GitHub
Guides](https://guides.github.com/) that explain how to use many of the features
that GitHub provides. In particular, please make sure that you have read the
following GitHub guides: [Mastering
Markdown](https://guides.github.com/features/mastering-markdown/), [Hello
World](https://guides.github.com/activities/hello-world/), and [Documenting Your
Projects on GitHub](https://guides.github.com/features/wikis/). Each of these
guides will help you to understand how to use both [GitHub](http://github.com) and
[GitHub Classroom](https://classroom.github.com/).

To do well on this assignment, you should also review Chapters 1 through 3 of
the course textbook, additionally paying close attention to the class notes and
the previous laboratory and/or practical assignments. Please see the course
instructor or one of the teaching assistants or tutors if you have questions
about any of these reading assignments.

## Commands

To get started in using the GatorGrader tool, you can change into the directory
for this assignment and type the command `gradle grade` in your terminal.
Running this command will produce a lot of output that you should carefully
inspect. If the output indicates that GatorGrader judges that there are no
mistakes in the assignment, then this means that your source code and writing
are passing all of the automated baseline checks. However, if the output
indicates that there are mistakes, then you will need to understand what they
are and then try to fix them. Finally, remember that you must run the `gradle
grade` command from the main (or "home base") directory for this assignment
where the `build.gradle` file is located. Then, you can type the command in
the terminal and study the output.

## Checking

In addition to making the checks that were previously mentioned in the
introduction to this document, your final submission must meet the following
requirements.

- src/www/answers.md:
  - Passes the checks performed by the Markdown linting tool
  - Passes the checks performed by the prose linting tool
  - Contains exactly one use of a `# A Web Site Created by` content
  - Contains exactly five uses of a `##` sectioning markers
  - Contains exactly four uses of a `**` formatting markers
  - Contains exactly one reference to a file with a `png` extension
  - Produces exactly four lines of output in the terminal
  - Contains exactly four uses of the fenced code block formatting markers
  - Can be converted to HTML by `pandoc` without producing an error

- GitHub repository:
  - Contains five commits beyond the repository's starting number of commits

## Updates

If the course instructor updates the provided material for this assignment and
you would like to receive these updates, then you can type this command in the
main directory for this assignment:

```
git remote add download git@github.com:Allegheny-Computer-Science-302-S2019/cs302-S2019-practical2-starter.git
```

You should only need to type this command once; typing the command additional
times may yield an error message but will not negatively influence the state of
your repository. Now, you are ready to download the updates provided by the
course instructor by typing:

```
git pull download master
```

This second command can be run whenever the course instructor needs to provide
you with new source code for this assignment. However, please note that, if you
have edited the files that the course instructor updated, running the previous
command may lead to Git merge conflicts. If this happens, you may need to
manually resolve them with the help of the instructor or a teaching assistant.

## Travis

This assignment uses [Travis CI](https://travis-ci.com/) to automatically run
the checking programs every time you commit to your GitHub repository. The
checking will start as soon as you have accepted the assignment, thus creating
your own private repository, and the course instructor enables Travis for it. If
you are using Travis for the first time, you will need to authorize Travis CI to
access the private repositories that you created on GitHub.

## Requirements

The GatorGrader software that supports the checking of this assignment was
developed for the following software and versions:

- Gradle 4.6
- Java 1.8.0
- MDL 0.4.0
- Proselint 0.8.0
- Python 3.6

## Problems

If you have found a problem with this assignment's provided source code, then
you can go to the [Computer Science 302 Practical 2
Starter](https://github.com/Allegheny-Computer-Science-302-S2019/cs302-S2019-practical2-starter)
repository and create an issue by clicking the "Issues" tab and then clicking
the green "New Issue" button. If you have found a problem with the [GatorGrader
tool](https://github.com/GatorEducator/gatorgrader) and the way that it checks you
assignment, then you can follow the aforementioned steps to create an issue in
its repository. To ensure that your issue is properly resolved, please provide
as many details as is possible about the problem that you experienced. If you
discover a problem with the laboratory assignment sheet, then please raise an
issue in the
[cs302-S2019-lab-sheets](https://github.com/Allegheny-Computer-Science-302-S2019/cs302-S2019-sheets)
repository and mention this assignment.

Students who find, and use the appropriate GitHub issue tracker to correctly
document, a mistake in any aspect of this laboratory assignment will receive
free laptop stickers and extra credit towards their grade for it.

## Assistance

If you are having trouble completing any part of this project, then please talk
with either the course instructor or a teaching assistant during the laboratory
session. Alternatively, you may ask questions in the Slack team for this
course. Finally, you can schedule a meeting during the course instructor's
office hours.
