# GitHub Special Files and Paths

![GitHub special files and paths](README.png)

GitHub uses special files (like `README` and `LICENSE`), paths (like `/.github` and `/docs`), and repositories (like `<org>/.github`) to improve repository management. This guide summarizes these conventions.

- [Introduction](#introduction)
- [README](#readme)
  - [Profile README](#profile-readme)
  - [Organization README](#org-readme)
- [CHANGELOG](#changelog)
- [LICENSE](#license)
- [SUPPORT](#support)
- [SECURITY](#security)
- [CODE_OF_CONDUCT](#code-of-conduct)
- [CONTRIBUTING](#contributing)
- [CONTRIBUTORS](#contributors)
- [AUTHORS](#authors)
- [ACKNOWLEDGMENTS](#acknowledgments)
- [CODEOWNERS](#codeowners)
- [ISSUE_TEMPLATE](#issue-template)
- [PULL_REQUEST_TEMPLATE](#pull-request-template)
- [CITATION.cff](#citation-cff)
- [FUNDING.yml](#funding-yml)
- [dependabot.yml](#dependabot-yml)
- [Workflows](#workflows)
- [Jekyll](#jekyll)
- [Tracking](#tracking)

## Introduction

GitHub special files can be written in multiple formats:

- Plain text: `README` or `README.txt`
- Markup: `README.md`, `README.markdown` - see [markups](https://github.com/github/markup/blob/master/README.md#markups)
- Custom syntax: `CODEOWNERS`

These files are typically placed in:

- Root directory (`./`)
- `.github` directory for GitHub-specific files
- `docs` directory for documentation
- Custom directories like `ISSUE_TEMPLATE`

These are often called community health files, recommended repository files, or configuration files.

For more information, see [building a strong community](https://help.github.com/categories/building-a-strong-community/) and [GitHub's Open Source Guides](https://opensource.guide/).

## README

- File: `README.md`, `README.txt`, or `README`
- Locations: Root directory, `.github/`, or `docs/`
- Docs: [About READMEs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- Examples: [Awesome README examples](https://github.com/matiassingers/awesome-readme)

A README describes what your project does and why it's useful. GitHub displays this file automatically when visitors open your repository. README files in subdirectories appear when that directory is viewed.

### Profile README

- Repository: `<username>/<username>`
- Docs: [Managing your profile README](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)

Create a README in a repository named after your username (like [mojombo/mojombo](https://github.com/mojombo/mojombo)) to display content at the top of your GitHub profile.

### Organization README

- Repository: `<org>/.github` or `<org>/.github-private`
- Docs: [Customizing your organization's profile](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/customizing-your-organizations-profile)

A README in an organization's `.github` repository (like [github/.github](https://github.com/github/.github)) appears at the top of the organization profile. Using `.github-private` instead makes it visible only to organization members.

## CHANGELOG

- File: `CHANGELOG.md`, `CHANGELOG.txt`, or `CHANGELOG`
- Locations: Root directory, `.github/`, or `docs/`

A CHANGELOG documents version changes, new features, and bug fixes in your project.

## LICENSE

- File: `LICENSE.md`, `LICENSE.txt`, or `LICENSE`
- Locations: Root directory, `.github/`, or `docs/`
- Docs: [Adding a license](https://help.github.com/articles/adding-a-license-to-a-repository/)

The LICENSE file defines the legal terms for using your project. GitHub displays recognized licenses at the top of your repository page.

Need help choosing? Visit [choosealicense.com](https://choosealicense.com)

For projects with significant scope or that include others' intellectual property, consider consulting a lawyer. Without a license, default copyright laws may apply in some jurisdictions.

## SUPPORT

- File: `SUPPORT.md`, `SUPPORT.txt`, or `SUPPORT`
- Locations: Root directory, `.github/`, or `docs/`

The SUPPORT file explains how users can get help with your project. GitHub links to this file on the "New Issue" page, but not on the "New Pull Request" page.

Organization-wide default: Place in `<org>/.github` repository - [Learn more](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)

## SECURITY

- File: `SECURITY.md`, `SECURITY.txt`, or `SECURITY`
- Locations: Root directory, `.github/`, or `docs/`
- Docs: [Adding a security policy](https://help.github.com/en/articles/adding-a-security-policy-to-your-repository)

The SECURITY file outlines your project's security policies and how to report vulnerabilities. GitHub links to this file under the "Policy" link on the repository's "Security" tab.

Organization-wide default: Place in `<org>/.github` repository - [Learn more](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)

## CODE_OF_CONDUCT

- File: `CODE_OF_CONDUCT.md`, `CODE_OF_CONDUCT.txt`, or `CODE_OF_CONDUCT`
- Locations: Root directory, `.github/`, or `docs/`
- Docs: [Adding a code of conduct](https://help.github.com/articles/adding-a-code-of-conduct-to-your-project/)
- Examples: [Code of conduct examples](https://i-sight.com/resources/18-of-the-best-code-of-conduct-examples/)

A CODE_OF_CONDUCT establishes community behavior guidelines and outlines how to create an inclusive environment. It should explain how to address problems between community members.

Organization-wide default: Place in `<org>/.github` repository - [Learn more](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)

## CONTRIBUTING

- File: `CONTRIBUTING.md`, `CONTRIBUTING.txt`, or `CONTRIBUTING`
- Locations: Root directory, `.github/`, or `docs/`
- Docs: [Setting contributor guidelines](https://help.github.com/articles/setting-guidelines-for-repository-contributors/)
- Examples: [Awesome contributing guides](https://github.com/mntnr/awesome-contributing)

The CONTRIBUTING file explains how to contribute to your project. It helps ensure quality pull requests and useful issue reports. GitHub links to this file on both the "New Issue" and "New Pull Request" pages.

Organization-wide default: Place in `<org>/.github` repository - [Learn more](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)

## CONTRIBUTORS

- File: `CONTRIBUTORS.md`, `CONTRIBUTORS.txt`, or `CONTRIBUTORS`
- Locations: Root directory, `.github/`, or `docs/`

Lists all contributors to the project. Typically includes names, usernames, email addresses, or website links as preferred by each contributor.

Related to, but different from, the AUTHORS file.

## AUTHORS

- File: `AUTHORS.md`, `AUTHORS.txt`, or `AUTHORS`
- Locations: Root directory, `.github/`, or `docs/`

Lists the significant authors of the project, especially those with legal connection to the work. As the GNU project notes: "Only the contributions that are legally significant for copyright purposes need to be listed. Small contributions, bug reports, ideas, etc., can be omitted."

Related to, but different from, the CONTRIBUTORS file.

## ACKNOWLEDGMENTS

- File: `ACKNOWLEDGMENTS.md`, `ACKNOWLEDGMENTS.txt`, or `ACKNOWLEDGMENTS`
- Locations: Root directory, `.github/`, or `docs/`

Lists related projects, dependencies, libraries, and other resources that support the project. May include attribution for code with different copyrights or licenses.

## CODEOWNERS

- File: `CODEOWNERS`
- Locations: Root directory, `.github/`, or `docs/`
- Docs: [About code owners](https://help.github.com/articles/about-codeowners/)

The CODEOWNERS file defines who is responsible for specific parts of a codebase. These owners are automatically requested as reviewers when a pull request modifies their code. With required reviews enabled, code owners' approval can be required before merging.

## ISSUE_TEMPLATE

- File: `ISSUE_TEMPLATE` or files in `ISSUE_TEMPLATE/` directory
- Locations: Root directory, `.github/`, or `docs/`
- Docs: [Creating issue templates](https://help.github.com/articles/creating-an-issue-template-for-your-repository/)
- Examples: [GitHub template examples](https://github.com/devspace/awesome-github-templates)

Issue templates standardize information in new issues. When someone creates an issue, the template is automatically added to the issue body.

For multiple templates, create an `ISSUE_TEMPLATE/` directory and add templates like `bugs.md` or `feature_request.md`.

Organization-wide default: Place in `<org>/.github` repository - [Learn more](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)

## PULL_REQUEST_TEMPLATE

- File: `PULL_REQUEST_TEMPLATE` or files in `PULL_REQUEST_TEMPLATE/` directory
- Locations: Root directory, `.github/`, or `docs/`
- Docs: [Creating PR templates](https://help.github.com/articles/creating-a-pull-request-template-for-your-repository/)
- Examples: [GitHub template examples](https://github.com/devspace/awesome-github-templates)

PR templates standardize information in new pull requests. When someone creates a PR, the template is automatically added to the PR body.

For multiple templates, create a `PULL_REQUEST_TEMPLATE/` directory with different templates. Use query parameters to specify which template to use. [Learn about query parameters](https://help.github.com/articles/about-automation-for-issues-and-pull-requests-with-query-parameters/)

## CITATION.cff

- File: `CITATION.cff`, `CITATION.md`, `CITATION.bib` or variations
- Locations: Root directory (or `inst/CITATION` for R packages)
- Docs: [About citation files](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-citation-files)

The CITATION file defines how people should cite your project. It uses a plain text format with both human-readable and machine-readable citation information.

When added to your repository's root directory, GitHub automatically links to it from the repository landing page.

## FUNDING.yml

- File: `.github/FUNDING.yml`
- Docs: [Displaying a sponsor button](https://docs.github.com/en/github/administering-a-repository/managing-repository-settings/displaying-a-sponsor-button-in-your-repository)

This file configures the sponsor button for your repository. You can include GitHub Sponsors, external funding platforms, or custom funding URLs.

Organization-wide default: Place in `<org>/.github` repository - [Learn more](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)

## dependabot.yml

- File: `.github/dependabot.yml`
- Docs: [Dependabot documentation](https://github.com/dependabot)

Dependabot automatically updates dependencies in your repository. The configuration file specifies which dependencies to update and where to find them. When updates are available, Dependabot creates pull requests with the changes.

## Workflows

- Directory: `.github/workflows`
- Docs: [Workflow syntax](https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions)

Workflows are automated processes that run on GitHub Actions. Create YAML files (`.yml` or `.yaml`) in this directory to define workflows that build, test, or deploy your code when specific events occur.

## CNAME

- File: `CNAME`
- Docs: [Managing custom domains](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)

For GitHub Pages with a custom domain (like `example.com` instead of `username.github.io`), this file specifies the domain to direct to your site.

## Jekyll

- Docs: [Jekyll structure](https://jekyllrb.com/docs/structure/)

GitHub Pages uses Jekyll to build static websites. Key Jekyll files and directories:

- `_config.yml` - Configuration
- `_drafts/` - Unpublished posts
- `_includes/` - Reusable content
- `_layouts/` - Page templates
- `_posts/` - Blog posts
- `_data/` - Site data files
- `_sass/` - Style partials
- `_site/` - Generated output
- `.jekyll-metadata` - Build state
- `index` - Main page

Other files are included in the site without processing.

## Tracking

- Package: github-special-files-and-paths
- Version: 5.1.0
- Created: 2017-08-22T00:00:00Z
- Updated: 2023-08-02T13:01:05Z
- License: GPL-2.0-or-later or contact us for custom license
- Contact: Joel Parker Henderson (<joel@sixarm.com>)
