# GitHub special files and paths

GitHub uses special files such as `README` and `LICENSE`, and special paths such as `/.github` and `/docs`, to improve repository managment and developer interactions.  This page is a summary. We welcome pull requests.

* [Introduction](#introduction)
* [CODE_OF_CONDUCT](#code_of_conduct)
* [CODEOWNERS](#codeowners)
* [CONTRIBUTING](#contributing)
* [ISSUE_TEMPLATE](#issue_template)
* [LICENSE](#license)
* [PULL_REQUEST_TEMPLATE](#pull_request_template)
* [README](#readme)


## Introduction

GitHub special files can typically be written with a variety of formats and file name extensions:

  * Freeform text, such as `README` or `README.txt`.

  * Markup formats, such as `README.markdown` or `README.asciidoc` - see [markups](https://github.com/github/markup/blob/master/README.md#markups)

  * Custom syntaxes, such as the file `CODEOWNERS`.
 
GitHub special files are typically located in special paths a.k.a. special directories:
 
  * `/` is the repository root directory.

  * `/.github` is a dot file directory.

  * `/docs` is a typical documention directory.

  * Custom directories, such as the directory `ISSUE_TEMPLATE`.

The special files and paths are sometimes also known as community health files, recommended repository files, well-known configurations, etc. 

For a general overview see [building a strong community](https://help.github.com/categories/building-a-strong-community/)


## CODE_OF_CONDUCT

https://help.github.com/articles/adding-a-code-of-conduct-to-your-project/

CODE_OF_CONDUCT is a file that explains how to engage in a community, and how to inclusive environment that respects all people, and how to address any problems among members of your project's community. 


## CODEOWNERS

https://help.github.com/articles/about-codeowners/

CODEOWNERS is a file that defines individuals or teams that are responsible for code in a repository.

Code owners are automatically requested for review when someone opens a pull request that modifies code that they own. When someone with admin or owner permissions has enabled required reviews, they also can optionally require approval from a code owner before the author can merge a pull request in the repository.


## CONTRIBUTING

https://help.github.com/articles/setting-guidelines-for-repository-contributors/

CONTRIBUTING is a file that explains how people should contribute, and that can help verify people are submitting well-formed pull requests and opening useful issues.


## ISSUE_TEMPLATE

https://help.github.com/articles/creating-an-issue-template-for-your-repository/

When you add an issue template to your repository, project contributors will automatically see the template's contents in the issue body. Templates customize and standardize the information you'd like included when contributors open issues.

https://blog.github.com/2018-01-25-multiple-issue-and-pull-request-templates/

To add multiple issue templates to a repository create an `ISSUE_TEMPLATE/` directory in your project root. Within that `ISSUE_TEMPLATE/` directory you can create as many issue templates as you need, for example `ISSUE_TEMPLATE/bugs.md`.


## LICENSE

https://help.github.com/articles/adding-a-license-to-a-repository/

LICENSE is a file that explains the legal licensing, such as any rights, any restrictions, any regulations, etc. 

If you include a detectable license in your repository, people who visit your repository will see it at the top of the repository page.


## PULL_REQUEST_TEMPLATE

https://help.github.com/articles/creating-a-pull-request-template-for-your-repository/

When you add a pull request template to your repository, project contributors will automatically see the template's contents in the pull request body. Templates customize and standardize the information you'd like included when contributors create pull requests.

https://blog.github.com/2018-01-25-multiple-issue-and-pull-request-templates/

You can create a PULL_REQUEST_TEMPLATE/ subdirectory in any of the supported folders to contain multiple pull request templates. Use the template query parameter to specify the template that will automatically fill the pull request body. For more information, see "[About automation for issues and pull requests with query parameters.](https://help.github.com/articles/about-automation-for-issues-and-pull-requests-with-query-parameters/)"


## README

https://help.github.com/articles/about-readmes/

README is a file that explains your project, what it does, why it is useful, etc. The README file is often the first item a visitor will see when visiting your repository. 

If you put your README file in your repository's root, docs, or hidden .github directory, GitHub will recognize and automatically surface your README to repository visitors.

