---
tags:
  - guide
aliases:
  - markdown tutorial
  - pandoc tutorial
title: Markdown Guide
publish: 
parent: 
related: 
projects:
---

## Basic Markdown

Headers:

- Don't use more than one Level One Header (`#`)...
- ...unless you have a `title` property in the metadata.

| Format        | Markdown            | HTML                                                                           | Output                 |
| ------------- | ------------------- | ------------------------------------------------------------------------------ | ---------------------- |
| Italics       | `*Italics*`         | `<i>Italics</i> or <em>Italics</em>`                                           | *Italics*              |
| Bold          | `**Bold**`          | `<b>Bold</b> or <strong>Bold</strong>`                                         | **Bold**               |
| Strikethrough | `~~Strikethrough~~` |                                                                                | ~~Strikethrough~~      |
| Underline     |                     | `<u>Underline</u> or <span style="text-decoration:underline">Underline</span>` | <u>Underline</u>       |
| Subscript     |                     | `<sub>Subscript</sub>`                                                         | <sub>Subscript</sub>   |
| Superscipt    |                     | `<sup>Superscript</sup>`                                                       | <sup>Superscript</sup> |

For a more detailed overview of markdown syntax go to these links:

- [Markdown cheat sheet syntax](https://www.markdownguide.org/cheat-sheet/).
- [Syntax for writing on GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

### Footnotes

- Footnote example[^1].
- Another footnote example[^longnote].

[^1]: Footnotes can be numbered or,
[^longnote]: Foot notes can also be denoted without numbers; which will make numbering automatic.

## Images

![My cat Lillian](https://images.unsplash.com/photo-1635866208025-3b8079feab24?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D){#fig:ExampleImage}

Example of a figure (Fig. ref{fig:ExampleImage}). This will only render correctly using pandoc.

## References

See

- [citation syntax](https://pandoc.org/chunkedhtml-demo/8.20-citation-syntax.html#:~:text=To%20cite%20a%20bibliographic%20item,%40smith2000%3B%20%40smith2004%5D.)

- Simple reference format is `@citation-key` or `[@citation-key]`
	- e.g. @petersen.luxton1982 or [@petersen.luxton1982].
- Place `## References` as your last header.

## Exporting

Compiling your literature and exporting to other formats is done using Pandoc. Do this in the terminal in VS Code (`CTRL + SHIFT + O`).

- [Pandoc Crash Course](https://www.youtube.com/watch?v=bHMIL822NVs)

Necessary first steps including opening the folder:

```sh
cd Path/to/file/folder
```

```shell
cd C:\Users\deane\OneDrive\PKM\Projects\msc-git
```

### PDF

```sh
pandoc yourfile.md --citeproc -o output.pdf
```

### HTML

```shell
pandoc "C:/Users/deane/OneDrive/PKM/Projects/pkm-meta/markdown-guide.md" -o "C:/Users/deane/OneDrive/PKM/Projects/pkm-meta/markdown-guide.html" --standalone --filter citeproc
```

## Resources

- [Markdown basic syntax](https://www.markdownguide.org/basic-syntax/)
- [Mastering markdown and formatting for github](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [Zotero Style Repository](https://www.zotero.org/styles)
- [Citation Keys for Better BibTex](https://retorque.re/zotero-better-bibtex/citing/)
- [ZotFile Renaming Rule](http://zotfile.com/#:~:text=RENAMING%20RULES,-ZotFile%20renames%20files&text=Zotfile%20also%20supports%20optional%20and,the%20entry%20for%20%25j%20otherwise.)
- [## Scientific Writing with Markdown](https://jaantollander.com/post/scientific-writing-with-markdown/)
- [Markdown Preview Enhanced](https://shd101wyy.github.io/markdown-preview-enhanced/#/)
- Pandoc Citer for citation navigation.
- https://pandoc.org/chunkedhtml-demo/8.17-images.html
