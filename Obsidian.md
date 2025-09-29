---
tags:
  - pkm
aliases:
  - community plugins
  - obsidian guide
---

To increase the functionality of Obsidian you can install community plugins: `Settings > Community plugins`.

>[!bug] Avoid too many Obsidian plugins as it may slow down the program or plugins may negatively interact.

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

## Vault Structure

- `📁 Vault` mine is simply named 'PKM'
	- `📁 Archive` projects with end dates are placed in here according to the year
	- `📁 Library` notes on literature, movies, and image collections
	- `📁 Resources`
		- `📁 ZoteroLibrary` PDFs organised using [Zotero](Zotero.md)
			  ❕I moved my PDFs outside of Obsidian increase the speed of the application.
		- `📁 Figures` figures imported from Zotero
	- `📁 Meta` files related directly to my vault
		- `📁 Templates`
		- `📁 Plugins and Snippets` description of Community Plugins and [CSS snippets](obsidian-guide.md#snippets)

## Templates and Templater

Folder path:

```
"Meta/Templates"
```

## Basics

- Your **vault** is the location of your Obsidian files.
	- See a more detailed folder structure [here](pkm-system.md#vault).
- You can add [community plugins](Obsidian.md), [themes](obsidian-guide.md#theme), and [CSS snippets](obsidian-guide.md#snippets) to extend the capabilities or make the interface prettier.

### Hotkeys

Below is a table of basic hotkeys. You can view and change any hotkeys in `Settings > Hotkeys`. Some of my personal hotkeys have been changed to mirror those in VS Code.

See [hotkeys](obsidian/hotkeys.md).

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
projects: 
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

My preferred setup is as follows:

- **Text & interface font**: Roboto, Segoe UI, [Manrope](https://www.gent.media/manrope), Arial, sans-serif
- **Monospace font**: Roboto Mono, [Fira Code](https://github.com/tonsky/FiraCode), Consolas, mono
- **Accent color** suggestion: `#28afea` is a blue similar to Microsoft Outlook
- **Theme**: Minimal (with Minimal Theme Settings and Style Settings)
	- Light & dark mode color schemes: macOS

## Advanced

### Snippets

- [CSS Snippet Collection from r-u-s-h-i-k-e-s-h](https://github.com/r-u-s-h-i-k-e-s-h/Obsidian-CSS-Snippets/tree/Collection/Snippets)

## Community Plugins

Simple, necessary plugins that need no explanation include:

- **Calendar**
- **Minimal Theme Settings**
- **Settings Search**
- Extras
	- **CSS Inlay Colors**

More complicated plugins and their context include:

- Vault organisation functionality:
	- **Dataview** for showing notes using different filters
	- **Templater** for making more functional templates
	- **Tasks** for organising and automating Markdown checkboxes (`- [ ]`)
	- **Excalidraw** for drawing
	- *Good for homepage and mobile*
		- **Homepage** is used to indicate a note as home page
		- **Banners** adds banners to notes like in Notion (I only use this for my home page)
		- **Buttons** creates buttons that can perform certain functions
	- **Kanban**
	- **Tag Wrangler** lets you change tag names throughout your vault
	- **Periodic Notes** expands the default daily note into weekly, monthly, quarterly, and yearly notes
- Zotero-Obsidian workflow:
	- **Pandoc Reference List**
	- **Zotero Integration**
	- Pandoc Plugin

## Resources

If you have questions, email me. Otherwise, there is an active Reddit community, Obsidian forums, and numerous YouTube tutorials ([Nicole van der Hoeven](https://www.youtube.com/@nicolevdh) and [Brian Jenks](https://youtube.com/@BryanJenks)).
