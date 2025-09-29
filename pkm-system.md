---
tags:
  - project/evergreen
aliases:
  - "#pkm"
title: Productivity System
cssclasses: []
---

# Contents

- [[pkm-system-types|Type of PKM System]]
- [[vault|Vault Structure]]
- [[Obsidian|Guide to Obsidian]]

# Resources

- [Fork My Brain - Nicole van der Hoeven](https://notes.nicolevanderhoeven.com/Fork+My+Brain)
- [GitHub - oleeskild/obsidian-digital-garden](https://github.com/oleeskild/obsidian-digital-garden)
- [Welcome to Quartz 4](https://quartz.jzhao.xyz/)
- [I built Jeff Su's Notion in Obsidian](https://www.youtube.com/watch?v=PGPBYBTO7xA)
- https://github.com/groepl/Obsidian-Templates

# Notes

```dataview
TABLE WITHOUT ID link(file.name) as file,
	"<sub>" + aliases + "</sub>" as aliases,
	tags,
	parent
FROM -"Meta/Templates"
WHERE contains(tags, "pkm")
SORT parent, file.name
```
