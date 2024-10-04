---
tags:
  - guide
  - project/pkm
aliases:
  - community plugins
parent: 
related:
---

To increase the functionality of Obsidian you can install community plugins: `Settings > Community plugins`.

>⛔ Avoid overloading your Obsidian with plugins as it may slow down the program or plugins may negatively interact.

- Here are some small plugins to improve functionality:
	- Homepage
	- Tag Wrangler
	- Calendar
	- Kanban
- Here are some more complicated plugins I recommend:
	- Dataview
		- This can get very confusing. For now, just note that it can show you all the notes in a folder and you can select the metadata you want to see and sort by.
	- Style Settings
		- Once you've installed a community theme (my choice is Minimal), you can edit it using Style Settings.
	- Templater
		- Create and use detailed templates.

### Dataview

- [ ] Edit the `FROM` variable to where you keep your templates.

```dataview
TABLE 
	tags as 🏷️,
	aliases
FROM "Meta"
WHERE contains(tags, "guide")
AND contains(file.name, "obsidian")
SORT file.name
```

