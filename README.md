# GitHub special files and paths

<img src="README.png" alt="GitHub special files and paths" style="width: 100%;"/>

GitHub uses special files such as `README` and `LICENSE`, and special paths such as `/.github` and `/docs`, to improve repository managment and developer interactions.  This page is a summary. We welcome pull requests.

* [Introduction](#introduction)
* [README](#readme)
* [CHANGELOG](#changelog)
* [LICENSE](#license)
* [SUPPORT](#support)
* [SECURITY](#security)
* [CODE_OF_CONDUCT](#code_of_conduct)
* [CONTRIBUTING](#contributing)
* [CONTRIBUTORS](#contributors)
* [AUTHORS](#authors)
* [ACKNOWLEDGMENTS](#acknowledgments)
* [CODEOWNERS](#codeowners)
* [ISSUE_TEMPLATE](#issue_template)
* [PULL_REQUEST_TEMPLATE](#pull_request_template)
* [CITATION.cff](#citationcff)
* [FUNDING.yml](#fundingyml)
* [dependabot.yml](#dependabotyml)
* [workflows](#workflows)
* [Jekyll](#jekyll)


## Introduction

GitHub special files can typically be written with a variety of formats and file name extensions:

  * Freeform text, such as `README` or `README.txt`.

  * Markup formats, such as `README.markdown` or `README.asciidoc` - see [markups](https://github.com/github/markup/blob/master/README.md#markups)

  * Custom syntaxes, such as the file `CODEOWNERS`.

GitHub special files are typically located at the repository top level or in special paths:

  * `/.github` is a hidden dot file directory.

  * `/docs` is a typical documentation directory.

  * Custom paths, such as the directory `ISSUE_TEMPLATE`.

The special files and paths are sometimes also known as community health files, recommended repository files, well-known configurations, etc.

For a general overview see [building a strong community](https://help.github.com/categories/building-a-strong-community/) and [GitHub's Open Source Guides](https://opensource.guide/).


## README

  * File: `README` or `README.txt` or `README.md` etc.

  * Help: <https://help.github.com/articles/about-readmes/>

  * Awesome: list: <https://github.com/matiassingers/awesome-readme>

This file that explains your project, what it does, why it is useful, etc. 

This file is often the first item a visitor will see when visiting your repository, because GitHub automatically shows this file to repository visitors.


## CHANGELOG

  * File: `CHANGELOG` or `CHANGELOG.txt` or `CHANGELOG.md` etc. 

This file explains a reposity's notable changes, updates, versions, bug fixes, and the like. This file name convention has been around since the early days of the web.


## LICENSE

  * File: `LICENSE` or `LICENSE.txt` or `LICENSE.md` etc. 

  * Help: <https://help.github.com/articles/adding-a-license-to-a-repository/>

This file explains the respostory's legal license, such as any legal rights, any copyright restrictions, etc. If you include a detectable license in your repository, people who visit your repository will see it at the top of the repository page.

If you want help to choose a license, then try https://choosealicense.com

If your project is significant, or contains other peoples' work or intellectual property, then you may want to consult with a lawyer who can help you with your specific goals and needs. If you don't provide a license, then in some locations a default copyright law will apply.


## SUPPORT

  * File: `SUPPORT` or `SUPPORT.txt` or `SUPPORT.md` etc. 

This file explains how a reader can get help with the repository and project. Github links this file on the page "New Issue". Unlike the "CONTRIBUTING" file, GitHub does not link this file on the page "New Pull Request".


## SECURITY

  * File: `SECURITY` or `SECURITY.txt` or `SECURITY.md` etc.

  * Help: <https://help.github.com/en/articles/adding-a-security-policy-to-your-repository>

This file explains the project's security policies, such as a list of versions that are currently being maintained with security updates. This file also provides instructions on how users can submit a report of a vulnerability. 

GitHub links to this file, under the "Policy" link on the "Security" tab of your repository.


## CODE_OF_CONDUCT

  * File: `CODE_OF_CONDUCT` or `CODE_OF_CONDUCT.txt` or `CODE_OF_CONDUCT.md` etc.

  * Help: <https://help.github.com/articles/adding-a-code-of-conduct-to-your-project/>

  * Awesome: list: <https://i-sight.com/resources/18-of-the-best-code-of-conduct-examples/>

This file explains how to engage in a community, and how to foster an inclusive environment that respects all people, and how to address any problems among members of your project's community.


## CONTRIBUTING

  * File: `CONTRIBUTING` or `CONTRIBUTING.txt` or `CONTRIBUTING.md` etc.

  * Help: <https://help.github.com/articles/setting-guidelines-for-repository-contributors/>

  * Awesome: list: <https://github.com/mntnr/awesome-contributing>

This file explains how people can contribute to the project. This file can help verify people are submitting well-formed pull requests and opening useful issues. 

GitHub links to this file, on the page "New Issue" and the page "New Pull Request".


## CONTRIBUTORS

  * File: `CONTRIBUTORS` or `CONTRIBUTORS.txt` or `CONTRIBUTORS.md` etc. 

This file explains who has contributed to the project. When we use a `CONTRIBUTORS` file in our projects, we ask people how they want to be listed, such as by their name, handle, email address, website link, etc. 

Compare this file to the file `AUTHORS`.


## AUTHORS

  * File: `AUTHORS` or `AUTHORS.txt` or `AUTHORS.md` etc. 

This file lists people who are significant authors of the project, such as the people who are legally related to the work. The GNU project states "Only the contributions that are legally significant for copyright purposes (see Legally Significant) need to be listed. Small contributions, bug reports, ideas, etc., can be omitted." 

Compare this file to the file `CONTRIBUTORS`.


## ACKNOWLEDGMENTS

  * File: `ACKNOWLEDGMENTS` or `ACKNOWLEDGMENTS.txt` or `ACKNOWLEDGMENTS.md` etc. 

This file explains relevant related work, such as other projects that are dependencies, or libraries, or modules, or have their own copyrights or licenses that you want to include in your project.


## CODEOWNERS

  * File: `CODEOWNERS`

  * Help: <https://help.github.com/articles/about-codeowners/>

This file defines individuals or teams that are responsible for code in a repository. 

Code owners are automatically requested for review when someone opens a pull request that modifies code that they own. When someone with admin or owner permissions has enabled required reviews, they also can optionally require approval from a code owner before the author can merge a pull request in the repository.


## ISSUE_TEMPLATE

  * File: `ISSUE_TEMPLATE`

  * Help: <https://help.github.com/articles/creating-an-issue-template-for-your-repository/>

  * Awesome: list: <https://github.com/devspace/awesome-github-templates>

When you add an issue template to your repository, project contributors will automatically see the template's contents in the issue body. Templates customize and standardize the information you'd like included when contributors open issues.

See <https://blog.github.com/2018-01-25-multiple-issue-and-pull-request-templates/>

To add multiple issue templates to a repository create an `ISSUE_TEMPLATE/` directory in your project root. Within that `ISSUE_TEMPLATE/` directory you can create as many issue templates as you need, for example `ISSUE_TEMPLATE/bugs.md`.


## PULL_REQUEST_TEMPLATE

  * File: `PULL_REQUEST_TEMPLATE` or can be a subdirectory

  * Help: <https://help.github.com/articles/creating-a-pull-request-template-for-your-repository/>

  * Awesome: list: <https://github.com/devspace/awesome-github-templates>

This file triggers project contributors to automatically see the template's contents in a new pull request body. The template can customize and standardize the information you'd like included when contributors create pull requests.

See <https://blog.github.com/2018-01-25-multiple-issue-and-pull-request-templates/>

You can create a `PULL_REQUEST_TEMPLATE/` subdirectory in any of the supported folders to contain multiple pull request templates. Use the template query parameter to specify the template that will automatically fill the pull request body. For more information, see "[About automation for issues and pull requests with query parameters.](https://help.github.com/articles/about-automation-for-issues-and-pull-requests-with-query-parameters/)"


## CITATION.cff

  * File: `CITATION.cff`

  * Help: <https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-citation-files>

This file explains how you would like people to cite your work. The citation file format is plain text with human-readable and machine-readable citation information.

When you add this file to the default branch root directory of your repository, then GitHub automatically links to it from the repository landing page.


## FUNDING.yml

  * File: `.github/FUNDING.yml`

  * Help: <https://docs.github.com/en/github/administering-a-repository/managing-repository-settings/displaying-a-sponsor-button-in-your-repository>

You can configure your sponsor button by adding a  file in your repository on the default branch. You can configure the button to include sponsored developers in GitHub Sponsors, external funding platforms, or a custom funding URL.


## dependabot.yml

  * File: `.github/dependabot.yml`

  * Help: <https://github.com/dependabot>

Dependabot is a GitHub tool that provides automated dependency updates. To enable updates, create a Dependabot configuration file and add it to a repository. The file describes the dependencies to update, where dependency manifests are located, etc. If Dependbot discovers that an update is available, then Dependabot sends you a pull request to update your dependency.


## Workflows

  * Directory: `.github/workflows`

  * Help: <https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions>

A workflow is a configurable automated process made up of one or more jobs. You must create a YAML file to define your workflow configuration. Workflow files use YAML syntax, and must have file extension `.yml` or `.yaml`.


## Jekyll

Files and diretories: see below

  * Help: <https://jekyllrb.com/docs/structure/>

GitHub uses Jekyll to compile static sites for hosting through its GitHub Pages service.  Jekyll configuration is read directly from the repository.

The following files and directories are used by Jekyll:

* `_config.yml`
* `_drafts/`
* `_includes/`
* `_layouts/`
* `_posts/`
* `_data/`
* `_sass/`
* `_site/`
* `.jekyll-metadata`
* `index`

All other files in the repository are included in the generated site without additional processing.


## Tracking

* Package: github-special-files-and-paths
* Version: 5.0.0
* Created: 2017-08-22T00:00:00Z
* Updated: 2022-02-21T17:07:56Z
* License: GPL-2.0-or-later or contact us for custom license
* Contact: Joel Parker Henderson (joel@sixarm.com)
