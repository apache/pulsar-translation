## :warning: Project Archived :warning:

[![development](https://img.shields.io/badge/development-halted-red.svg)](https://github.com/apache/pulsar/issues/17972)

**This initiative is halted because no further contributor or maintainer is active to contributor to or shepherd it.**

Still, transaltion of Pulsar document and content is welcome and desired. If you're willing to revive this initiative, feel free to send a proposal to the [dev mailing list](mailto:dev@pulsar.apache.org) ([subscribe](mailto:dev-subscribe@pulsar.apache.org)).

# Translation workflow and guidelines

Welcome to join the Pulsar translation project! Before translating, read translation [workflow](#workflow) and [guidelines](#guidelines).

You can find other language guidelines as listed below:

Language|Guidelines
--------|-----
Chinese Simplified (zh-CN) | [README_zh-CN](https://github.com/apache/pulsar-translation/blob/master/README_zh-CN.md)
Chinese Traditional (zh-TW) | [README_zh-TW](https://github.com/apache/pulsar-translation/blob/master/README_zh-TW.md)

## Workflow

You can find [Apache Pulsar translation project](https://crowdin.com/project/apache-pulsar) on Crowdin. For further details about the functions of Crowdin, see [Crowdin](https://crowdin.com/).
Here are the steps of the translation workflow:

### Join the Pulsar translation project

1. Sign in [Apache Pulsar Crowdin project](https://crowdin.com/project/apache-pulsar). If you don’t have a Crowdin account, on the crowdin page, click **SIGN UP** at the upper right corner and fill in the information to create an account. If you have a GitHub, Facebook, Google, Twitter, or Gitlab account, you can link any of them to sign in.

2. After signing in, click **Join** at the upper right corner on the crowdin page.

> **Note:**
> The source language of Pulsar files is English. Currently the target languages of translation projects are Chinese, French, and Japanese.  
> Select a language. Take the **Simplified Chinese Translation Project** as an example.

### Choose a file to translate and submit a PR

1. Click **Simplified Chinese Translation Project**.
2. Click  **master > docs**,  and check out the status of each file. 
Files in **master > docs** are the source files of the latest versions on Pulsar official website. You only need to translate these markdown files.

- Green: translated and approved  
- Blue: translated but not approved
- Grey: not translated

![](media/translation-status.jpg)

Based on your knowledge about Pulsar, you can translate the content that you are familiar with first.

After choosing the file to translate, please check it out in [Translation schedule](https://github.com/apache/pulsar-translation/blob/master/schedule.md). If you find someone is translating this file, please choose another one. If not, you can create a PR and add the file name to [Translation schedule](https://github.com/apache/pulsar-translation/blob/master/schedule.md). Then you can submit the PR.

### Label Setting

- Reviewers: No need to set up. Reviewers will receive the notification of PR you submitted automatically and will designate someone to handle it.
- Assignees: Choose yourself to receive notifications.
- Label: Choose “translation”.

### Translating

While translating, you don’t need to translate the ID of the file and keep the tag the same as the source file.
> **Important**  
> Don’t modify, omit or add a space in a tag, as the omission or relocation of a tag leads to mistakes shown on the website.

![](media/id-tag.jpg)

You can modify and save the content directly. Your version will appear automatically at the top of the translation list, as Crowdin will record different versions from different translators. **TM AND MT TRANSLATION** in the bottom-right corner offers you TMs in Pulsar, Crowdin, and other websites.

![](media/translation-interface.jpg)

> **Tip:**
> You can use and update [Pulsar 文档翻译术语库](https://shimo.im/sheets/5jozGy5WIUQQf5JV/MODOC) while translating.

### Review

After finishing a translation, please leave a comment in your PR.
For example, I've finished the translation, could you help review?

After receiving the comment, reviewers start to review. The reviewer can make simple comments and notify the translator. Direct discussion in PR is encouraged.

If there are no problems, the reviewer will approve this PR and merge it.

The following image gives a general workflow. The workflow source file is available at [lucidchat](https://www.lucidchart.com/invitations/accept/0ebad9d8-ddf3-4a92-8ee6-e813a9bc58ff).
Masakazu shares a more detailed [swimlane](https://swimlanes.io/d/8L04SRASw) for the workflow.

![](media/translation-workflow.jpg)

## Guidelines

For different language, there are some translation guidelines written to make sure the sytles consistency  and reading fluency. Please read it before translation start.

Language|Guidelines
--------|-----
Chinese Simplified (zh-CN) | [README_zh-CN](https://github.com/apache/pulsar-translation/blob/master/README_zh-CN.md)
Chinese Traditional (zh-TW) | [README_zh-TW](https://github.com/apache/pulsar-translation/blob/master/README_zh-TW.md)

## Add you as a contributor

When your first pull request is merged, feel free to add your name to the [contributor list](https://github.com/apache/pulsar-translation/blob/master/CONTRIBUTORS.md).
