# Contributing to our standards

If you would like to contribute to these standards, please raise an [Issue](https://github.com/nhsengland/it-standards/issues) in the first instance.

## Contribution process

Except for [small corrections](#small-corrections), proposals for new standards or changes to exsisting standards will follow this process:

1. Proposal Stage

   Proposals can be submitted as [Issues on GitHub](https://github.com/nhsengland/it-standards/issues). Please use the appropriate template and fill in all sections.

2. Response Stage

   Once an Issue has been raised, the proposal will be reviewed by the owners of the repository and raised with the NHS England and NHS Improvement joint Architecture Review Board and other relavent colleagues as needed.
   
   The proposal will be reviewed, any questions and responses will be added to comments in the Issue.
   
   If the proposal is not accepted, the issue will be closed. Otherwise the label on the issue will be change to #3 and the appropriate people will be notified to start work on the change.

3. Development Stage

   The assigned author(s) will either create a new topic branch of this repository (if they have direct change rights) or will create a fork.
   
   Text and images will be added in the branch or fork.
   
   Once the fork is ready for final review, the lead author will submit a [Pull Request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests) (PR) against the master branch.

4. Final Approval Stage

   When the PR is received, it will be reviewed by the repository owners and any final discussion will take place.
   
   If necessary, this version will be reviewed by the ARB and other stakeholders.
   
   If changes are required, the PR will be rejected and the authors will make further changes and submit a new PR. Small corrections however may be accepted on the existing PR.
   
   Once the reviewers are happy, the PR will be accepted and the changes will be live. The master branch of this repository will always be the live, approved version of the standards.

5. Live

   Live standards are under change control. Suggested changes to live standards will go back through these stages.
   
### Small corrections

The main process is not needed for small corrections to standards. Small changes may include typos, layout issues correction to links or contacts.

In this case, PR's will be accepted directly. Alternatively, if the person raising the issue does not have the tools or knowledge to make a change themselves, they can raise an Issue using the blank template.

In these cases, the corrections will be reviewed by the repository owners or suitable SME's and accepted or rejected directly.

## Formatting and layout

All standards will use [GitHub Flavored Markdown (GFM)](https://github.github.com/gfm/) throughout. Other document formats may be allowed via exception but may not be considered a long-term solution for authoring standards. However, some additional document format files may be accepted as example or template files. PDF files will only be accepted for convenience of sharing standards with other parties not as a master file format.

In addition to GFM, there are a few extensions provided by the [Docsify tool](https://docsify.js.org/#/helpers)S used to turn the files into a web site.

Diagrams should be developed in a suitable tool (e.g. Visio or PowerPoint) and exported as SVG files (.svg) wherever possible. These should then be uploaded and linked to in the markdown document. The master file, in this case, may be retained in the original tool's native format and uploaded for future development.

Other images should be uploaded in JPeg (.jpg or .jpeg or .jfif) format and suitably referenced in the document(s).

Other markdown extensions _may_ be approved in the future dependent on them being compatible with output formats required. The [Commonmark](https://commonmark.org/) standard will be used as the gold-standard for extended markdown in that case.

You should use logical header levels to ensure a good structure to your document. Only use heading level 1 once in a document and don't use it at all if using the `title` metadata field.

### Folder Structures

TBC

### Metadata

Document metadata may be included in a markdown file. Metadata, if used, must be at the start of the file and must use [YAML](https://yaml.org/) formatting. This is in keeping with website generators such as [Hugo](https://gohugo.io/content-management/front-matter/) or [Jekyll](https://jekyllrb.com/docs/front-matter/) which may be used to generate documentation websites.

Note that, when using `title`, you do not need to provide a title in the text of your document, it is added automatically. The description will also be shown.

The following metadata will be automatically shown on the pages:

- `title` - Document title. Will be used as the initial line of the document marked as a heading1 level.
- `description` - A single paragraph describing the document. Will be added as text to the top of the output document.
- `stage` - The approval stage of the document. 1-5 is allowed. Normally, only stages 3-5 would be used as 1 & 2 would be before a document is created. You only need the number but can add other text after it, it will be ignored.
- `created` - Date (and optionally time) that the document was originally created. Should not be changed.
- `lastUpdated` - Date (and optionally time) that the document was last amended.
- `reviewDate` - Date (and optionally time) after which the document requires review/revision. A warning will be displayed on the page if this date has passed.

A version number is not needed since any updates should have a comment against them when they are committed to the repository. Changes can be undone using the commit mechanism in Git.

#### Example

Note that the `---` lines are required and deliniate the metadata. Metadata will be shown as a table in GitHub.

```
---
title: Standard for open source development
description: >
  This is an extended description or summary of the document.
  It can occupy multiple lines thanks to the use of ">" above.
stage: 3. Development
created: 2020-06-10 14:42:49
lastUpdated: 2021-06-10 14:43:03
reviewDate: 2021-01-01
tags:
- tag1
- tag2
author: Main Author Name
---
```

## Tooling

It is strongly recommended to use either Microsoft Visual Studio Code (VSCode) or Typora for authoring documentation in this repository. Both should be configured to format as GitHub Flavored Markdown.

### Docsify

This is used to present the contents of the repository as a web site.

The following features and plugins are used:

- Themable plugin with Simple Theme - easy theming. Coupled with some customisations to start to bring the display to NHS standards.
- Front-matter plugin - Allows for YAML based front-matter variables.
- Mustache plugin - Allows data from various internal and external sources to be displayed with some conditional and repeating features.
- Pagination plugin - Previous/Next page navigation at the foot of each page.
- Edit-on-GitHub plugin - Adds a link to each page.
- Custom plugin - Display document metadata on each page.

### Git

You will need Git installed to enable you to work with the repository. GitHub Desktop can be useful for managing the process of cloning branches or forks to your local machine for editing and submission of changes.

VSCode can use Git directly. There are also optional extensions for working with GitHub directly.

### Typora

Typora is a visual editor for Markdown (WYSIWYG). It is particularly helpful when working with tables.

Typora supports more markdown extensions than GitHub does and so some features should be turned off in Preferences if necessary. It also has a GitHub theme which may be useful to be able to see the impact of changes.

Typora also has a useful Table of Contents feature that should be used at least with longer documents. (VSCode also has extensions that will manage TOCs).

For pasting images from the clipboard, you can set Typora to automatically copy the image as a file to the current folder.

### VSCode

VSCode is a powerful open source text editor and integrated development environment from Microsoft. It is free to use for commercial and personal use. Unlike Typora, editing Markdown happens in text only but there is a live, synchronised preview view that opens in a side window of the editor.

VScode has a number of useful extensions that can help when authoring, including:

* [Markdown All-In-One](https://github.com/yzhang-gh/vscode-markdown)
* [Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)
* [Markdown Shortcuts](https://marketplace.visualstudio.com/items?itemName=mdickin.markdown-shortcuts)
* [Paste Image](https://marketplace.visualstudio.com/items?itemName=mushan.vscode-paste-image) - will copy a pasted image to the same folder as the open file & add a link to the document.

There are also several powerful GitHub and Git extensions that may be useful for some people.

