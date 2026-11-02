# hp-ttrpg
A single-file, offline character sheet for a Harry Potter tabletop RPG. It has built-in dice rolling and seven tabs: Character, Cheat Sheet, Charms, Other Spells, Potions, Notes and Reference. Spell rules, reference material and your own notes are searchable (with typo-tolerant matching), and characters save in the browser. You can export and import all of your data as a backup file, and game masters can switch on an optional GM View to keep track of several characters at once. Includes dark mode and meets WCAG AA accessibility standards.

## Changelog

### 2026-11-02 (v2.0)
**New optional GM View for game masters**
- Turn it on with the new **Enable GM View** switch at the top of the page. It is off by default, so players see no change. While it is on, the tabs become GM View, Notes and Reference, and the page uses a neutral grey theme instead of house colours. Turning it off brings everything back, and the roster is kept.
- **GM View tab:** a roster table of player characters and NPCs with name, house, year, body and mind condition, story points, attributes, and skill and spell counts. Search the roster, select a character to see their full detail (attributes, wand, pets and items, skills, health, learned spells and potions, and their notes), and remove entries you no longer need.
- **Import sheets:** add several exported character files at once. A file for a character already in the roster updates that entry (matched by character ID, or by name with a confirmation). Files that aren't character backups are skipped and reported.
- The GM can adjust a character's story points and body/mind condition. Changed values are marked as edited since import, and re-importing a file asks before replacing them. The existing Lock values switch also locks these controls.
- **Private GM notes** per character. They stay in the GM's browser and are never included in a player's export. A player's own notes are shown read-only.
- The GM roster is stored separately from your own character, and imported data is cleaned on the way in. Your own sheet is never changed by importing sheets into the roster.

**Sharing your sheet**
- Export data now asks whether to include your Notes. Choose "Export without notes" to share your sheet with your GM without your private notes. The confirmation on import says when a file has no notes.
- Exports now carry a character ID so a GM can update the right roster entry. The ID is added to your saved character the first time you export.
- The Export data / Import data buttons are hidden on the GM View tab, where they don't apply.

**Your saved data**
- Characters saved with v1.5 and v1.9 load unchanged, and GM View is off until you switch it on. The new roster is saved under its own storage entry.

### 2026-10-30 (v1.9)
Changes since the original upload (v1.5):

**Search**
- Typo-tolerant search everywhere: spell and potion lists, the Reference tab and the attribute/skill drop-downs now match misspellings, words in any order, and accented letters. Short words (under 4 letters) still need an exact match.
- Abbreviations written with dots match without them: "dada" finds D.A.D.A.
- Potions can be searched by level (beginner, intermediate, advanced, expert). Charms and Other Spells can be searched by year ("1st year", "first year", "year 1", through 7th year, plus "non-curricular"). The Cheat Sheet and the Reference year columns understand the same wording.

**New Notes tab**
- Create, title, rename and delete note sections.
- Rich text editor: bold, italic, underline, strikethrough, headings, bulleted and numbered lists, quotes, links and Clear formatting (which also turns list items back into normal paragraphs).
- One search box searches the titles and text of every section and shows a snippet around each match.
- Notes save automatically in the browser. Export notes / Import notes buttons back them up; importing adds to your existing notes and strips scripts and unsafe links.

**Backup**
- Export data / Import data buttons in a footer on every tab. Export saves your whole character, notes and display preferences (dark mode, lock values, tooltips) to one file. Import replaces everything after a confirmation that names what will be overwritten, and offers to download your current data first.

**Character sheet**
- Pets, artifacts, etc. now has 8 lines instead of 7.

**Your saved data**
- Characters saved with the previous version load unchanged. The new `notes` data is only added when you create a note, and no existing saved fields were renamed or removed. This was checked by loading a v1.5 save into v1.9 and back.

### 2026-10-09 (v1.5)
- Initial upload.
