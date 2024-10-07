---
tags:
  - guide
  - project/pkm
aliases:
  - how to obsidian
  - obsidian
title: Obsidian Guide
parent:
  - "[[Projects/pkm-meta/README|pkm-meta]]"
related:
---

## Contents

- 

## Basics

- Your **vault** is the location of your Obsidian files.
	- See a more detailed folder structure [here](pkm-system.md#vault).
- You can add [community plugins](obsidian-plugins.md), [themes](obsidian-guide.md#theme), and [CSS snippets](obsidian-guide.md#snippets) to extend the capabilities or make the interface prettier.

### Hotkeys

Below is a table of basic hotkeys. You can view and change any hotkeys in `Settings > Hotkeys`. Some of my personal hotkeys have been changed to mirror those in VS Code.

| Command                      | Hotkeys (default) | Hotkeys (personal)     |
| ---------------------------- | ----------------- | ---------------------- |
| **Open** file                | `CTRL/CMD + O`    | `CTRL/CMD + P`         |
| **Commands** list            | `CTRL/CMD + P`    | `CTRL/CMD + SHIFT + P` |
| **New** note                 | `CTRL/CMD + N`    |                        |
| Move line **up**             |                   | `ALT + ↑`              |
| Move line **down**           |                   | `ALT + ↓`              |
| Open **settings**            | `CTRL/CMD + ,`    |                        |
| **Live** preview/source mode |                   | `CTRL/CMD + SHIFT + M` |
| Insert **template**          |                   | `ALT + I`              |
| Toggle **left sidebar**      |                   | `CTRL/CMD + SHIFT + ,` |
| Toggle **right sidebar**     |                   | `CTRL/CMD + SHIFT + .` |

## Links

- Wikilinks:
	- You can link to notes in your vault using two square brackets: `[[another-note]]`. 
		- Headings in the note: `[[another-note#heading]]`
- Markdown links:
	- Alternatively, you can link to files as such: `[Link to file](another-note.md)`.
		- Headings in the note: `[Link to file](another-note.md#heading)`.
- You can change how links are generated `Settings > Files and links > Use [[Wikilinks]]`.

## Properties

- The properties/frontend/metadata is written in YAML. These data are attached to the file and can be used for organisation - see [dataview](obsidian-guide.md#dataview).
- You can create any variable you like, but the most important are [tags](obsidian-guide.md#tags) and [aliases](obsidian-guide.md#aliases). Additional tags that I like to use include:

- `created`: date note created
- `parent`: broader topic or parent of this note
- `related`: other notes related to this note

### Tags

- Tags help categorise notes. Click on the tag #guide to open the search tab.
- Using tags is a personal journey and add tags as you see fit.
- I recommend the plugin `Tag Wrangler` so that you can rename tags *en masse*.

### Aliases

I love aliases - it's one of primary reasons I love Obsidian so much. Say, for example, you have forgotten the name and placement of *this* file. In the `aliases` property you can add `how to obsidian` or, simply, `obsidian` (different notes can have the same alias). So, when you search for this file, any matches in the `aliases` property will lead you here.

Another example to illustrate the usefulness of this feature is in species notes. Say you have a note about *Ursus maritimus* but have forgotten the Latin, simply add "polar bear" as an alias.

## Core Plugins

### Templates

- Templates are pre-built blocks of text or code that you can insert into you note. This includes the metadata. For example, I have a default template that includes the metadata: `tags` and `aliases`. Unless I'm creating a special note, every time I create a new note I insert this template.
- Templates need to be stored in a specific folder. You name the folder anything and place it anywhere, just let Obsidian know where it is in the settings.
	- My folder structure is `Meta/Templates`.

#### Task: Create a default note template

Steps:

1. Create a `Templates` folder.
2. Go to `Settings > Templates` and fill in `Template folder location`.
3. Make a new note and copy-paste the code below:

```yaml
---
tags:
aliases:
created: {{date:YYYY-MM-DD}}
parent:
related:
---
```

4. Name the file something like `DEFAULT NOTE` and move it to the `Templates` folder.
5. Make a new note, open the command list, find `Templates: Insert template`, and press `ENTER`.
6. Find `DEFAULT NOTE` and press `ENTER`.

You have just inserted a template with properties that you can start populating. You may have noticed that the `created` property has a link - this is related to the [daily notes](obsidian-guide.md#daily%20notes) core plugin.

### Daily notes

## Aesthetics

### Fonts

### Theme

## Advanced

### Snippets

- [CSS Snippet Collection from r-u-s-h-i-k-e-s-h](https://github.com/r-u-s-h-i-k-e-s-h/Obsidian-CSS-Snippets/tree/Collection/Snippets)

## Aesthetics

### Fonts

### Theme

## Resources

If you have questions, email me. Otherwise, there is an active Reddit community, Obsidian forums, and numerous YouTube tutorials ([Nicole van der Hoeven](https://www.youtube.com/@nicolevdh) and [Brian Jenks](https://youtube.com/@BryanJenks)).
