---
title: "Git for Document Management"
date: 2022-01-25T12:41:42-05:00
draft: false
toc: true
images:
tags:
  - untagged
---

{{< image src="/images/posts/git-for-document-management.png" alt="graphic-of-person-on-computer" position="center" style="border-radius: 8px;" >}}

The idea for this came to me while exploring and contributing to open source communities. It was (and still is) quite impressive how well these communities self govern using the Git version control system. Developers use the Git system to maintain a record of any changes to programming files and to me I couldn't see why we couldn't use the same system for documents.

## The Markdown language

One downside to using Git for document management is the need to use plain text files and the Markdown language. Using software like Microsoft Office Suite or anything similar is not really possible due to the way Git tracks changes. Markdown is a very simplistic language and only provides basic support for formatting the document. To me this is actually quite powerful when it comes to document management because it requires an individual to simplify the document in a way that works with Markdown. Personally I am not a fan of long text heavy documents, no one reads them if they are long so why have them (exception being legal documents)?

## Creating commits

This is actually difficult because all of the standards (i.e. conventional commits) revolves around software development and not document management. Because of this I decided to create my own that track important changes for document management and are as follows:

| type   | description                                             |
| ------ | ------------------------------------------------------- |
| new    | When a document is being added to the repo for tracking |
| add    | When new text is added to an existing document          |
| update | When text is changed in an existing document            |
| style  | No text is changed only formatting                      |
| chore  | Changes not affecting documents                         |

### Example commits

- new: Create incident response process document
- add: Add point of contact table to incident response process
- update: Change document owner to john doe
- style: Change location of table of contents
- chore: Move incident response plan to incident response folder

## Creating and managing branches

Branches follow the same methodology that is used in software development. If a document needs to be added or altered a branch is created and all changes are made before making a pull request to update the main production documents. Anything living on the main or master branch are considered published documents and any other branches are considered pending changes.

### Example branches

- new/incident-response-process
- add/add-point-of-contacts-to-incident-response-process
- update/change-incident-response-process-document-owner
- style/change-incident-response-process-table-of-contents-location
- chore/move-incident-response-plan-to-incident-response-folder
