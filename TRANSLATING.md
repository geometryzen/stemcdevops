# Translating Pro Git (2nd Edition)

The translations are managed in a decentralized way. Each translation team maintains their own project. Each translation is in its own repository, the Pro Git team simply pulls the changes and builds them into the https://git-scm.com website when ready.

## General guidance for translating Pro Git

Pro Git is a book about a technical tool, therefore translating it is difficult compared to a non-technical translation.

The following are guidelines to help you on your way:
* Before you begin, read the whole Git Pro book in English, so that you're aware of the content, and are familiar with the style used.
* Ensure you have a good working knowledge of git, so that explaining the technical terms is doable.
* Stick to a common style and format for the translation.
* Be sure to read and understand the basics of [Asciidoc formatting](https://asciidoctor.org/docs/asciidoc-syntax-quick-reference/). Not following the asciidoc syntax can lead to problems with building/compilation of the pdf, epub and html files needed for the book.

## Translating the book to another language

### Helping with a existing project

* Check for an already existing project in the following table.
* Go to the project's page on GitHub.
* Open an issue, introduce yourself and ask where you can help.

| Language       | GitHub page     |
| :------------- | :------------- |
| العربية        | [geometryzen/stemcdevops-ar](https://github.com/geometryzen/stemcdevops-ar) |
| Беларуская     | [geometryzen/stemcdevops-be](https://github.com/geometryzen/stemcdevops-be) |
| български език | [geometryzen/stemcdevops-bg](https://github.com/geometryzen/stemcdevops-bg) |
| Čeština        | [geometryzen/stemcdevops-cs](https://github.com/geometryzen-cs/stemcdevops-cs) |
| English        | [geometryzen/stemcdevops](https://github.com/geometryzen/stemcdevops) |
| Español        | [geometryzen/stemcdevops-es](https://github.com/geometryzen/stemcdevops-es) |
| فارسی          | [stemcdevops/stemcdevops-fa](https://github.com/geometryzen/stemcdevops-fa) |
| Français       | [geometryzen/stemcdevops-fr](https://github.com/geometryzen/stemcdevops-fr) |
| Deutsch        | [geometryzen/stemcdevops-de](https://github.com/geometryzen/stemcdevops-de) |
| Ελληνικά       | [geometryzen/stemcdevops-gr](https://github.com/geometryzen/stemcdevops-gr) |
| Indonesian     | [geometryzen/stemcdevops-id](https://github.com/geometryzen/stemcdevops-id) |
| Italiano   | [geometryzen/stemcdevops-it](https://github.com/geometryzen/stemcdevops-it) |
| 日本語   | [geometryzen/stemcdevops-ja](https://github.com/geometryzen/stemcdevops-ja) |
| 한국어   | [geometryzen/stemcdevops-ko](https://github.com/geometryzen/stemcdevops-ko) |
| Македонски | [geometryzen/stemcdevops-mk](https://github.com/geometryzen/stemcdevops-mk) |
| Bahasa Melayu| [geometryzen/stemcdevops-ms](https://github.com/geometryzen/stemcdevops-ms) |
| Nederlands | [geometryzen/stemcdevops-nl](https://github.com/geometryzen/stemcdevops-nl) |
| Polski | [stemcdevops-pl/stemcdevops-pl](https://github.com/geometryzen2-pl/stemcdevops-pl) |
| Português (Brasil) | [geometryzen/stemcdevops-pt-br](https://github.com/geometryzen/stemcdevops-pt-br) |
| Русский   | [geometryzen/stemcdevops-ru](https://github.com/geometryzen/stemcdevops-ru) |
| Slovenščina  | [geometryzen/stemcdevops-sl](https://github.com/geometryzen/stemcdevops-sl) |
| Српски   | [geometryzen/stemcdevops-sr](https://github.com/geometryzen/stemcdevops-sr) |
| Svenska  | [geometryzen/stemcdevops-sv](https://github.com/geometryzen/stemcdevops-sv) |
| Tagalog   | [geometryzen/stemcdevops-tl](https://github.com/geometryzen/stemcdevops-tl) |
| Türkçe   | [geometryzen/stemcdevops-tr](https://github.com/geometryzen/stemcdevops-tr) |
| Українська| [geometryzen/stemcdevops-uk](https://github.com/geometryzen/stemcdevops-uk) |
| Ўзбекча  | [geometryzen/stemcdevops-uz](https://github.com/geometryzen/stemcdevops-uz) |
| 简体中文  | [geometryzen/stemcdevops-zh](https://github.com/geometryzen/stemcdevops-zh) |
| 正體中文  | [geometryzen/stemcdevops-zh-tw](https://github.com/geometryzen/stemcdevops-zh-tw) |

### Starting a new translation

If there is no project for your language, you can start your own translation.

Base your work on the first edition of the book, available [here](https://github.com/geometryzen/stemcdevops). To do so:
 1. Pick the correct [ISO 639 code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for your language.
 1. Create a [GitHub organization](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/creating-a-new-organization-from-scratch), for example: `stemcdevops-[your code]` on GitHub.
 1. Create a project `stemcdevops`.
 1. Copy the structure of geometryzen/stemcdevops (this project) in your project and start translating.

### Updating the status of your translation

On https://git-scm.com, the translations are divided into three categories. Once you have reached one of these levels, contact the maintainers of https://git-scm.com/ so that they can pull the changes.

| Category | Completion     |
| :------------- | :------------- |
| Translation started for | Introduction translated, not much else. |
| Partial translations available in | up to chapter 6 has been translated. |
| Full translation available in |the book is (almost) fully translated. |

## Continuous integration with GitHub Actions

GitHub Actions is a [continuous integration](https://en.wikipedia.org/wiki/Continuous_integration) service that integrates with GitHub. GitHub Actions is used to ensure that a pull-request doesn't break the build or compilation. GitHub Actions can also provide compiled versions of the book.

The configuration for GitHub Actions is contained in the `.github/workflows` directory, and if you bring in the `main` branch of the root repository you'll get them for free.
However, if you created your translation repo by _forking_ the root repo, there's an extra step you must complete (if you did not fork, you can skip this part).
GitHub assumes that forks will be used to contribute to the repo from which they were forked, so you'll have to visit the "Actions" tab on your forked repo, and click the "I understand my workflows" button to allow the actions to run.

## Setting up a publication chain for e-books

This is a technical task, please ping @david to get started with epub publication.
