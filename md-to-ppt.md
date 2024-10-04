---
tags:
  - workflow
  - note/slides
aliases:
  - MD to Slides
  - Markdown Powerpoint
  - markdown to powerpoint
bibliography: C:/Users/deane/OneDrive/PKM/Resources/ZoteroLibrary.bib
csl: C:/Users/deane/OneDrive/PKM/Resources/csl/chicago-author-date.csl
link-citations: true
css:
---

# H1 creates a **Section Title**

## H2 creates a **Slide Title**

Text on a slide: 

- bullet
- bullet
- bullet

:::
Speaker notes go here
:::

---

## Two columns

:::::::::::::: {.columns}
::: {.column width="50%"}

Left column:

- bullet
- bullet
- bullet

:::
::: {.column width="50%"}

![](frog-mushroom.png)

:::  
::::::::::::::

---

## Compile using pandoc

```shell
pandoc md-to-ppt.md -o md-to-ppt.pptx
```

See more details on [pandoc's website](https://pandoc.org/chunkedhtml-demo/10-slide-shows.html).

# Testing limits

## Test sizing

- Will the text get smaller if I fill up the *entire* space?
	- No.
- A
- B
- C
- D
- E
- F
- G
- H
- I
- J
- K
- L
- M
- N
- O

## Referencing

@gullan.cranston2014 is an entomology textbook.

Compile references using:

```shell
pandoc md-to-ppt.md --citeproc -o md-to-ppt.pptx
```

## References
