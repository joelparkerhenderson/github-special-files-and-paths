# GitHub special files and paths

<img src="README.png" alt="GitHub special files and paths" style="width: 100%;"/>

GitHub uses special files such as `README` and `LICENSE`, and special paths such as `/.github` and `/docs`, to improve repository managment and developer interactions.  This page is a summary. We welcome pull requests.

* [Introduction](#introduction)
* [CODE_OF_CONDUCT](#code_of_conduct)
* [CODEOWNERS](#codeowners)
* [CONTRIBUTING](#contributing)
* [ISSUE_TEMPLATE](#issue_template)
* [Jekyll](#jekyll)
* [LICENSE](#license)
* [PULL_REQUEST_TEMPLATE](#pull_request_template)
* [README](#readme)
* [SECURITY](#security)


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

- Help: <https://help.github.com/articles/about-readmes/>
- Awesome list: <https://github.com/matiassingers/awesome-readme>

`README` or `README.txt` or `README.md` etc. is a file that explains your project, what it does, why it is useful, etc. The `README` file is often the first item a visitor will see when visiting your repository. GitHub will recognize and automatically surface your `README` to repository visitors.


## CHANGELOG

`CHANGELOG` or `CHANGELOG.txt` or `CHANGELOG.md` etc. is a file that describes what's happening in a reposity, such as version number increases, software updates, bug fixes, and the like. This file name convention has been around since the early days of the web.


## LICENSE

https://help.github.com/articles/adding-a-license-to-a-repository/

`LICENSE` or `LICENSE.txt` or `LICENSE.md` etc. is a file that explains the legal licensing, such as any rights, any restrictions, any regulations, etc. If you include a detectable license in your repository, people who visit your repository will see it at the top of the repository page.

If you want help to choose a license, then try https://choosealicense.com

If your project is significant, or contains other peoples' work or intellectual property, then you may want to consult with a lawyer who can help you with your specific goals and needs.

If you don't provide a license, then in some locations, there are default copyright laws that will apply.


## CODE_OF_CONDUCT

- Help: <https://help.github.com/articles/adding-a-code-of-conduct-to-your-project/>
- Awesome list: <https://i-sight.com/resources/18-of-the-best-code-of-conduct-examples/>

`CODE_OF_CONDUCT` is a file that explains how to engage in a community, and how to inclusive environment that respects all people, and how to address any problems among members of your project's community.


## CONTRIBUTING

- Help: <https://help.github.com/articles/setting-guidelines-for-repository-contributors/>
- Awesome list: <https://github.com/mntnr/awesome-contributing>

`CONTRIBUTING` is a file that explains how people should contribute, and that can help verify people are submitting well-formed pull requests and opening useful issues. GitHub links this file on page "New Issue" and the page "New Pull Request". This helps people understand how to contribute.


## CONTRIBUTORS

`CONTRIBUTORS` or `CONTRIBUTORS.txt` or `CONTRIBUTORS.md` etc. is a file that lists people who have contributed to the project. When we use a `CONTRIBUTORS` file in our projects, we ask people how they want to be listed, such as by their name, handle, email address, website link, etc. Compare this file to the file `AUTHORS`.


## SUPPORT

`SUPPORT` or `SUPPORT.txt` or `SUPPORT.md` etc. is a file that explains how a reader can get help with the repository and project. Github links this file on the page "New Issue". Unlike the "CONTRIBUTING" file, GitHub does not link this file on the page "New Pull Request".


## SECURITY

- Help: <https://help.github.com/en/articles/adding-a-security-policy-to-your-repository>

`SECURITY` describes your project's security policies, including a list of versions that are currently being maintained with security updates. It also gives instructions on how your users can submit a report of a vulnerability. If you provide a `SECURITY` file, it will appear under the "Policy" link on the "Security" tab of your repository.


## CODEOWNERS

https://help.github.com/articles/about-codeowners/

`CODEOWNERS` is a file that defines individuals or teams that are responsible for code in a repository.

Code owners are automatically requested for review when someone opens a pull request that modifies code that they own. When someone with admin or owner permissions has enabled required reviews, they also can optionally require approval from a code owner before the author can merge a pull request in the repository.


## ISSUE_TEMPLATE

- Help: <https://help.github.com/articles/creating-an-issue-template-for-your-repository/>
- Awesome list: <https://github.com/devspace/awesome-github-templates>

When you add an issue template to your repository, project contributors will automatically see the template's contents in the issue body. Templates customize and standardize the information you'd like included when contributors open issues.

https://blog.github.com/2018-01-25-multiple-issue-and-pull-request-templates/

To add multiple issue templates to a repository create an `ISSUE_TEMPLATE/` directory in your project root. Within that `ISSUE_TEMPLATE/` directory you can create as many issue templates as you need, for example `ISSUE_TEMPLATE/bugs.md`.


## Jekyll
- Help: <https://jekyllrb.com/docs/structure/>

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


## PULL_REQUEST_TEMPLATE

- Help: <https://help.github.com/articles/creating-a-pull-request-template-for-your-repository/>
- Awesome list: <https://github.com/devspace/awesome-github-templates>

When you add a `PULL_REQUEST_TEMPLATE` file to your repository, project contributors will automatically see the template's contents in the pull request body. Templates customize and standardize the information you'd like included when contributors create pull requests.

https://blog.github.com/2018-01-25-multiple-issue-and-pull-request-templates/

You can create a `PULL_REQUEST_TEMPLATE/` subdirectory in any of the supported folders to contain multiple pull request templates. Use the template query parameter to specify the template that will automatically fill the pull request body. For more information, see "[About automation for issues and pull requests with query parameters.](https://help.github.com/articles/about-automation-for-issues-and-pull-requests-with-query-parameters/)"
