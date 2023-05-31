---
name: Contributions
about: Contributing to the process guidance
title: ''
labels: ''
assignees: ''

---

**Contribution summary**
A clear and concise description of the changes proposed.

**Additional context**
Add any other context about the changes here.

**Check page purpose**
It's important that the content of each section is in the correct place. The aim of the
current structure is to provide lighweight documentation and to place detailed guidance
in dedicated subpages. Please review your contibution against the purposes of each page:

* index.qmd: Help the user navigate the website structure.
* general-considerations/guidance.qmd : Things that apply to any approach to code
publication (open at start, end or never open). Things to think about prior to making
this decision.
* general-considerations/references.qmd : Please do not add references here. Instead,
add references to bibliography/references.bib and reference using the `@` notation.
* open-at-the-start/guidance.qmd : Considerations for projects that will develop in
the open.
* open-at-the-end/guidance.qmd : Considerations for projects that will publish at
close or at intervals. This may be with a full or partial commit history.
* never-open/guidance.qmd : Things to consider if a project is too sensitive to
consider publishing.
* what-could-go-wrong/checklist.qmd : A page to help us learn from each other.
Things that may not have been caught by the 'fit for publishing'checklist or are more
specific to certain kinds of projects (eg webscraping activities).

**Consider accessibility guidance**
Please help us meet Government Digital Standard by:

- [ ] render your documentation and check with the [WAVE accessibility browser plugin](https://wave.webaim.org/extension/).
- [ ] avoiding the use of italic or strikethrough text.
- [ ] ensuring all images have descriptive alt text.
- [ ] only using image tags as markdown syntax renderring cannot be relied upon to
present alt text as required by WCAG guidance. Avoid using markdown to render images.
- [ ] avoid skipping headers for visual purposes. Header orders should be incremental,
such as h1,h2,h3,h2,h2,h2,h3,h4,h4 etc. Headers can be restyled using CSS where
required.

**Referencing issues and pull requests**
You can bring up a list of suggested issues and pull requests within the repository by
typing #. Type the issue or pull request number or title to filter the list, and then
press either tab or enter to complete the highlighted result. Linking PRs to issues
helps to keep an audit trail in the repository's history.

**Mentioning people**
You can mention a person or team on GitHub by typing @ plus their username or team name.
This will trigger a notification and bring their attention to the conversation. People
will also receive a notification if you edit a comment to mention their username or team
name.
