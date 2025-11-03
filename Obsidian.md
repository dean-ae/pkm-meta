---
tags:
  - app
aliases:
  - community plugins
  - obsidian guide
---

<br><center><i><span class='fire'>Personal Knowledge Management System for Biology Students.</span></i></center><br>

| →   | [[Markdown]] | [[Zotero]] | [[obs-zot\|Obsidian-Zotero Workflow]] | [[R]] |
| --- | ------------ | ---------- | ------------------------------------- | ----------- |

I try, hard, to stick to the principle of KISS (keep it simple, stupid). However, Obsidian is wildly customisable through community plugins and CSS snippets. The classic cycle of many Obsidian users is: (A) download many plugins and customise appearance to increase functionality; (B) find yourself working too much ON Obsidian, and not enough IN Obsidian; (C) return to a more basic form of the application; (D) repeat cycle. I am at stage C and intend not to repeat the cycle. Thus, here I present how I use Obsidian as a researcher trying not to get too absorbed. I will briefly go over my basic setup for Obsidian (appearance, basic settings, and plugins), but if you're already familiar with the basics, jump to [[obs-zot|Obsidian-Zotero Workflow]].

See [[Markdown]] (MD) for text formatting.

## Plugins

Plugins, either built by Obsidian or the community, expand the functionality of the application. Some are small and some large. It can be fun to explore them; but, as I have said above, I am trying to keep it as simple as possible.

>[!BUG] Avoid too many Obsidian plugins as it may slow down the program or plugins may negatively interact.

## Links

To link files you can use Wikilinks: the link to the above note is written as `[[Markdown]]`. You can give it a different name, such as [[Markdown|MD]] (`[[Markdown|MD]]`) or link to headings inside the note [[Markdown#Basics|MD basics]] (`[[Markdown#Basics|MD basics]]`). Use can also link using pure MD format: `[link to note, image, or webpage](Markdown.md)`.

## Properties

The properties/frontend/metadata is written in YAML. These data are attached to the file and can be used for organisation in Bases.

You can create any variable you like, but the most important I have found are **tags** and **aliases**. See templates for the other properties I sometimes use.

### Tags

Obsidian supports hashtags to so that you can organise your notes (see Bases). By clicking on a tag you can search all notes that include it: #species. Otherwise, you can add tags into the properties of a file - they function very similar.

You can edit your tags *en masse* using the Tag Wrangler community plugin.

### Aliases

I love aliases - it's one of primary reasons I love Obsidian so much. Say, for example, you have a note named *Ursus maritimus* but have forgotten the Latin. When creating the note you might add "polar bear" in the `aliases` property. So, when you search for the note (`CTRL + P`) and type "polar", the note will be presented.

## Templates

Certain notes might share the same structure, for this, you use templates. To insert a template, I have set the hotkey as `ALT + I`. I mostly use templates to put properties into files in order of frequency:

1. [[0-default]] includes `tags` and `aliases`
2. [[1-extra]] includes `title`, `parent`, `related`, and `description`
3. [[2-icon-banner]] includes `icon` (emoji) and `banner` (image)
4. [[3-archive]] includes a check box, `archive`

See [here](https://help.obsidian.md/plugins/templates) for base templates and [here](https://github.com/SilentVoid13/Templater) for the Templater community plugin.

Note, you need to set a template folder. My example is `Meta/Templates`.

## Hotkeys

Hotkeys can be useful, but if you only learn one short learn the **command palette**. Default Obsidian makes it `CTRL + P`, but I have changed mine to mimic Visual Studio Code, so `CTRL + P` opens the note browser and `CTRL + SHIFT + P` opens the command palette. Either way is acceptable. You can change your hotkeys in settings or learn what they are from the command palette.

## Clippings

Clippings is a browser extension that lets you extract web pages into Obsidian. You can extract the entire content, or merely some metadata. The 'templates' need to be built in your browser.

My default new clipping has the template:

![[Pasted image 20251103125509.png]]

## Appearance

I highly recommend the Minimalist theme. It is has low energy use and is well supported. It also can be used with the community plugins Minimal Theme Settings, Style Settings, and Hider. The Minimal Theme Settings allows you to set a hotkey to toggle dark and light mode (I have set it as `CTRL + SHIFT + L`).

My appearance settings are as such:

| Setting        | Value      |
| -------------- | ---------- |
| Theme          | Minimal    |
| Interface font | Segoe UI   |
| Text font      | Aptos Mono |
| Monospace font | Aptos Mono |
| Accent color   | `#487eba`  |

### CSS snippets

The `Vault/.obsidian/snippets` contains CSS files that change the appearance of Obsidian. They are generally for small details, but can be extensive. Access the folder in the CSS snippets section of the appearances settings tab.

The ones I have included are:

- `folder-descriptions` (see the file explorer tab)
- `color-blocks` <span class='fire'>defines HTML</span> <span class='water'>'span' blocks</span>
- `tag-colours` makes tags different colours in reading mode, e.g. #water, #ice
- [1] `checkbox-progress-bar` sets a 1-5 progress bar using `- [1]`

## Vault structure

This is personal - where you place different classes of notes/files and what you name your folders. In Obsidian, at the very least you need folder for you templates, daily notes, and clippings. I have used the CSS snippet `folder-descriptions.css` to explain the use of each folder.

Obsidian allows you to use minimal folder as you can easily filter through different notes using tags and [[Obsidian#Bases|Bases]]

## Some simple plugins

### Core

You can access all of the core plugins in the settings. Below are some worth mentioning.

| Plugin           | Use                                                                                                                                 |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| Canvas           | Make mind maps by manually linking notes together.                                                                                  |
| Graph view       | See how notes are linked by wikilinks (`[[wikilink]]`) or tags (`#tag`).<br>Though novel and fun, I don't use this feature.         |
| Outline          | Navigate the headings (`# heading`) of your notes quickly.                                                                         |
| Publish and Sync | Paid features to make your vault accessible or shareable online.                                                                    |
| Daily notes      | Creates a note linked to each day. See [[2025-10-01]] as an example.<br>You can create your own daily note template. See [[daily]]. |

### Community

Some simple community plugins that add small but useful changes are listed with their use. Install them in the community plugins tab.

| Plugin           | Use                                                                                                           |
| ---------------- | ------------------------------------------------------------------------------------------------------------- |
| Calendar         | Provides a calendar view so that you can quickly navigate your daily notes.                                   |
| Homepage         | Allows you to set a note as your homepage; this can be a single note, your daily note, or even a random note. |
| CSS Inlay Colors | Generates the colour when you write it inline code: `purple`, `pink`, or `#9e77ed`                            |
| Settings Search  | Adds a search bar in the settings menu.                                                                       |
| Tag Wrangler     | Allows your to *en masse* edit the value of a tag.                                                            |

## Bases

Bases lets you view files and their properties in database format or card format. See [here](https://help.obsidian.md/bases) for more information.

### Table

![[Base.base]]

### Cards

![[Mammals.base#Ursidae]]

## Excalidraw

This community plugin allows you to draw in Obsidian. The functionality is expansive, but I have not used it much.

# Additional resources

If you have questions, email me. Otherwise, there is an active Reddit community, Obsidian forums, and numerous YouTube tutorials ([Nicole van der Hoeven](https://www.youtube.com/@nicolevdh) and [Brian Jenks](https://youtube.com/@BryanJenks)).
