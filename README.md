<img src="https://github.com/datasciencecampus/awesome-campus/blob/master/ons_dsc_logo.png">

# Coding in the Open

# Introduction
## About
A compendium of open-source guidance which aims to share the benefits, risks and a summarised strategy for open-source coding.

## Installation
This documentation is written and built using [Quarto](https://quarto.org/) - an open-source scientific and technical publishing system. To work with Quarto, you will need to install the Quarto CLI (Command Line Interface). How this is done is dependent on the system you are using:

- _Internal to ONS_: Installation is possible via ServiceNow. Select 'I Want Something' > Computer Software - Add / Transfer / Remove > Complete and submit the request form.
- _External to ONS_: Follow the [Quarto Getting Started page](https://quarto.org/docs/get-started/) for more details.

If you are new to Quarto, check out Quarto's [tutorials](https://quarto.org/docs/get-started/hello/vscode.html) and [detailed documentation](https://quarto.org/docs/reference/) for further information.

In addition to the Quarto CLI, and if VS Code is your integrated development environnement of choice, a useful (and completely optional) [VS Code extension](https://quarto.org/docs/tools/vscode.html) is available. This provides additional functionality to VS Code that will make previewing and rendering using Quarto easier. Another useful VS code extension is the Microsoft verified [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker). This is useful when editing documentation within VS code since it offers basic spell checking capability. Note: it is recommended you configure the settings of this extension to only work with a subset of file types you want to be spell checked (e.g., .md and .qmd files only).

## Usage

### Editing the Documentation

At it's core, editing this set of documentation means writing in markdown within a set of `.qmd` files. The table below summarises the current structure of the `.qmd` files:

| .qmd file | description |
| --- | --- |
| `index.qmd` | The main documentation landing page. |
| `common/general_considerations.qmd` | A page in which general considerations for working in an open-source environment are shared. |
| `common/references.qmd` | A page that shares all sources used to build this documentation. |
| `private_to_public/guidance.qmd` | A page dedicated summarising a strategy for transitioning private repositories into the public domain. |

Whilst editing the documentation, from root directory you can call:

```console
quarto preview
```
from the command line (or use the VS Code button at the top right hand corner of the .qmd file) to open a live preview locally on your machine.

### Controlling the Configuration

The main configuration is controlled via `_quarto.yml`. Here, numerous options are available from fixing the layout to adding new pages. You can find out more about these options on Quarto's [project basics page](https://quarto.org/docs/projects/quarto-projects.html.).

In addition to the main configuration, it is possible to create dynamic/global variables that can then be used throughout the documentation. This is done within `_variables.yml`. See the [variables section](https://quarto.org/docs/authoring/variables.html) of Quarto's documentation for more details.

### References
This documentation is built from and adds to existing sources of information and guidances on open-sourcing codebases. Therefore, referencing/citations are an important part of this documentation.

Quarto handles this automatically using [citation markdown](https://quarto.org/docs/authoring/footnotes-and-citations.html#sec-citations). This can simply be used anywhere within `.qmd` files to reference a source.

The sources themselves are stored in the `BibLaTeX` file `bibliography/references.bib`. See [BibTeX's guide](https://www.bibtex.com/g/bibtex-format/) for more information on the required referencing syntax.

A CSL (Citation Style Language) file (`bibliography/ieee.csl`) is used to control the format and layout of the references once the pages are rendered. At the moment, the IEEE format has been chosen for it's simplicity and conciseness, but other CSL formats exist, with their complementary files being provided by [the Citation Style Language Project](https://github.com/citation-style-language/styles).

### Adding Assets

Assets (such as images) can be added to the `assets/` directory. There is a subdirectory within this specifically for images, to keep them all in one common place. Quarto then reads these in as [figrues](https://quarto.org/docs/authoring/figures.html) using a relative (to the root) reference to the image.

### Rendering the Documentation

Once you are happy with the content and any modifications you have made, the documentation can be rendered. Please note that manual renderring is not a requirement of hosting this guidance on GitHub Pages. This can be done by calling:

```console
quarto render
```
from the command line at the root directory (or use the VS Code button at the top right hand corner of the .qmd file). This will build the documentation, storing it within the `docs` folder. Feel free to render a local copy for styling etc, but please **do not commit html files to the repository**. 

### Developer Guidance

* If you'd like to [raise an issue](https://github.com/datasciencecampus/coding-in-the-open/issues), please check against the current list of issues first.
* PRs are most welcome. [Link your PR to an existing issues where possible](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue). 
* Please do not commit HTML to the repo. [CI is setup to handle rendering & publishing](https://quarto.org/docs/publishing/github-pages.html).


# Data Science Campus
At the [Data Science Campus](https://datasciencecampus.ons.gov.uk/about-us/) we apply data science, and build skills, for public good across the UK and internationally. Get in touch with the Campus at [datasciencecampus@ons.gov.uk](datasciencecampus@ons.gov.uk).

# License

<!-- Unless stated otherwise, the codebase is released under [the MIT Licence][mit]. -->

The code, unless otherwise stated, is released under [the MIT Licence][mit].

The documentation for this work is subject to [© Crown copyright][copyright] and is available under the terms of the [Open Government 3.0][ogl] licence.

[mit]: LICENCE
[copyright]: http://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/
[ogl]: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/
