# GitHub special files and paths

GitHub special files include `README`, `LICENSE`, etc. GitHub special paths include `.github`, `docs`, etc. These help automate repository managment and developer interactions.  This page summarizes these files and paths. We welcome pull requests and welcome GitHub staff creating an official page that replaces this page.

* [Introduction](#introduction)
* [History](#history)
* [Also known as](#also-known-as)
* [Community profile checklist](#community-profile-checklist)
* [CODE_OF_CONDUCT](#code_of_conduct)
* [CODEOWNERS](#codeowners)
* [LICENSE](#license)
* [PULL_REQUEST_TEMPLATE](#pull_request_template)


## Introduction

GitHub special files can typically be written with a variety of formats and file name extensions:

  * using freeform text, such as `README` or `README.txt`.

  * using Markdown, such as `README.md` or `README.markdown`.

  * There are exceptions, such as the `CODEOWNERS` file.

  * TODO: any other formats, such as ASCIIDOC?
 
 
GitHub special files are typicallylocated in special paths a.k.a. special directories:
 
  * `/` is the repository root directory

  * `/.github` is a dot files directory

  * `/docs` is a typical documention directory

  * There are exceptions, such as the `PULL_REQUESTS_TEMPLATES` directory.

  * TODO: any other special directories?

 
## History

Some of the file names have a very long history.

  * For example the file name `README` is a convention that goes far back to the 1980's or earlier. 

Some of the file names are unique to GitHub as far as we know.

  * For example the name `CODEOWNERS` and its syntax were created by GitHub staff.


## Also known as

The special files and paths are sometimes also known as:

  * community health files

  * recommended repository files

  * well-known files and well-known directories 

  * TODO: any other terminology?


## Community profile checklist

The GitHub community profile checklist checks to see if a project includes recommended community health files, such as README, LICENSE, CONTRIBUTING, etc.

TODO: how to add other files to the checklist?


## CODE_OF_CONDUCT

https://help.github.com/articles/adding-a-code-of-conduct-to-your-project/

CODE_OF_CONDUCT is a file that explains how to engage in a community, and how to inclusive environment that respects all people, and how to address any problems among members of your project's community. 


## CODEOWNERS

https://help.github.com/articles/about-codeowners/

CODEOWNERS is a file that defines individuals or teams that are responsible for code in a repository.

Code owners are automatically requested for review when someone opens a pull request that modifies code that they own. When someone with admin or owner permissions has enabled required reviews, they also can optionally require approval from a code owner before the author can merge a pull request in the repository.


# CONTRIBUTING

https://help.github.com/articles/setting-guidelines-for-repository-contributors/

CONTRIBUTING is a file that explains how people should contribute, and that can help verify people are submitting well-formed pull requests and opening useful issues.


## LICENSE

https://help.github.com/articles/adding-a-license-to-a-repository/

LICENSE is a file that explains the legal licensing, such as any rights, any restrictions, any regulations, etc. 

If you include a detectable license in your repository, people who visit your repository will see it at the top of the repository page.


## PULL_REQUEST_TEMPLATE

https://help.github.com/articles/creating-a-pull-request-template-for-your-repository/

When you add a pull request template to your repository, project contributors will automatically see the template's contents in the pull request body. Templates customize and standardize the information you'd like included when contributors create pull requests.

You can create a PULL_REQUEST_TEMPLATE/ subdirectory in any of the supported folders to contain multiple pull request templates. Use the template query parameter to specify the template that will automatically fill the pull request body. For more information, see "[About automation for issues and pull requests with query parameters.](https://help.github.com/articles/about-automation-for-issues-and-pull-requests-with-query-parameters/)"



