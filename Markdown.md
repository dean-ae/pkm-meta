---
tags:
  - computer-language
aliases:
  - MD
title: Markdown Guide
---

## Basics

Headings are written with a `#`. For example, the above heading is written as `## Basics`.

>[!TIP] Why do we start with two #'s instead of one?
>The first `# Heading` in the document is read as the title.
>You can use the Level One Header (`#`) or a `title` property in the metadata (YAML).

Here are some basic text formats you may want.

| Format        | Markdown            | HTML                                                                           | Output                 |
| ------------- | ------------------- | ------------------------------------------------------------------------------ | ---------------------- |
| Italics       | `*Italics*`         | `<i>Italics</i> or <em>Italics</em>`                                           | *Italics*              |
| Bold          | `**Bold**`          | `<b>Bold</b> or <strong>Bold</strong>`                                         | **Bold**               |
| Strikethrough | `~~Strikethrough~~` |                                                                                | ~~Strikethrough~~      |
| Underline     |                     | `<u>Underline</u> or <span style="text-decoration:underline">Underline</span>` | <u>Underline</u>       |
| Subscript     |                     | `<sub>Subscript</sub>`                                                         | <sub>Subscript</sub>   |
| Superscipt    |                     | `<sup>Superscript</sup>`                                                       | <sup>Superscript</sup> |
| Highlight     | `-> ==Highlight==`  |                                                                                | ==Highlight==          |

## Footnotes

- Footnote example[^1].
- Another footnote example[^longnote].

[^1]: Footnotes can be numbered or,
[^longnote]: Foot notes can also be denoted without numbers; which will make numbering automatic.

## Images

Images can be both local on online. The format for embedding images is as such:

`![Image Alt Text](Image Link)`

![My cat Lillian](https://images.unsplash.com/photo-1635866208025-3b8079feab24?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

## More Resources

For a more detailed overview of markdown syntax go to these links:

- [Markdown Cheat Sheet | Markdown Guide](https://www.markdownguide.org/cheat-sheet/)
- [Basic writing and formatting syntax - GitHub Docs](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
