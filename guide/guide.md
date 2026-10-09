# Buttermark guide

Everything the app does, in the order you'll want it. Two minutes for the tour is the welcome page; this is the rest.

## Writing

**The melt.** Markdown turns into formatting as you type and turns back when you touch it. Type `**` around a word and the asterisks dissolve when you leave; arrow back in and they return. Headings, lists, quotes, links and code all behave this way. There's no preview pane because the page is the preview.

**Headings and lists.** `#` for a heading, `-` for a list, `1.` for a numbered one. The marks fade in at the margin when your caret is on the line and fade out when it leaves. Enter continues a list; Enter on an empty item ends it.

**Code.** Backticks for inline code, three backticks for a block. In a block the text stays raw, with the language name after the opening fence if you want highlighting.

**Tables.** Pipes and dashes, the usual way. Buttermark aligns the columns while you type. In reading mode the header row stays pinned while you scroll.

**Footnotes.** Press Footnote on the floating toolbar, or type `[^1]`, and the note appears at the foot of the document. A footnote never eats your selection; it goes after it.

![The floating toolbar over a selection: bold, italic, strike, code, link, footnote, note, ask](guide/toolbar.png)

**Links.** `[text](url)` as always. Ctrl+click opens it. `[[Another note]]` links to a file by name anywhere in your workspace, or beside the document when no folder is open.

**Long files.** Fold a section from the chevron beside its heading; Ctrl+Shift+Up collapses the whole document to its headings and Ctrl+Shift+Down opens it again. The Contents panel on the right lists every heading; click one to jump. Ctrl+F finds in the document; Ctrl+Shift+F searches the whole workspace from the field under its name in the left bar.

**Focus.** Typewriter scroll keeps your line in the middle of the window; focus dimming fades everything but the paragraph you're in. Both live in the View menu and the palette.

## Reading

**Reading mode** turns a file into a page: no caret, no marks, the table headers pinned, footnotes in place. Ctrl+R turns it on and off, or Read mode in the palette. Buttermark reads any `.md`, including the ones other tools left behind.

![Reading mode: a table scrolled halfway, its header row pinned at the top](guide/reading-table.png)

**Page tone.** As is, Sepia or Night: a tint for reading that leaves your theme alone.

**Skim** shows the headings and first lines only, for finding your place in something long. The **reading ruler** is a soft band that follows your pointer or the arrow keys.

**Text size, line spacing and line width** for reading are separate from writing; change them in Settings › Reading and your writing view keeps its own.

## Asking your agent

Buttermark never calls a model. Your agent does, with your account, into your file.

**Leave an ask.** Select a sentence, press Ask on the floating toolbar, say what you want: "shorter", "make this a list", "find a better word for quiet". A small marker appears on the sentence. Leave a few around the draft as you go. An ask is an HTML comment in the file, so any other editor sees plain text.

**Hand them over.** The status bar says "3 asks for your agent · Copy prompt". Click it, and your clipboard holds a short instruction: open this file, find the asks, do what they say, save. Paste it to Claude, ChatGPT, Codex or anything that can open a file. If the document was never saved, Buttermark asks you to save first.

![An ask marker on a sentence, and the status bar reading 1 ask for your agent · Copy prompt](guide/ask.png)

**The answer arrives.** When the file changes, the new text appears with a highlighter wash and three small buttons: keep, take back, ask again. Keep dries the ink. Take back restores your sentence with its ask. Ask again reopens the ask so you can say it differently. The markers are gone from the file once the ask is answered.

![An arrival: the new sentence under a highlighter wash, with Keep, Take back and Ask again beside it](guide/arrival.png)

## Notes to yourself

Select words, press Note, write. A note is yours alone: it never enters the file, so you can send the `.md` to anyone and they get a clean document. Notes live in a small sidecar folder beside the document (`.notes/`), and the Annotations panel on the right lists every note and every ask in the file. If the words a note was attached to disappear, the note stands at the top of the document until they return or you remove it.

![The Annotations panel listing one note and one ask](guide/annotations.png)

## Themes

Four come with the app: Fresh, Linen, Evening and Midnight Oil. Settings › Appearance has a Light slot and a Dark slot, and a switch that follows your system or a schedule of evening hours. Click a theme in the gallery and the page wears it at once.

![Settings › Appearance: the Light and Dark slots and the gallery of themes](guide/appearance.png)

**The Maker.** Open any theme in the Maker (right panel) and change eleven colors and the typeface; everything else derives from them. Name it in the first field; every change saves itself. A theme is a `.bmtheme` file: plain JSON, shareable, and the gallery can install one from disk. F7 and F8 switch themes from the keyboard if you ever paint yourself into a corner.

![The Theme Maker in the right panel: the name, the eleven colors, the typeface](guide/maker.png)

## Workspaces

Open a folder and Buttermark shows its files in the left bar; that folder is your workspace. Save workspace as… gives it a name and keeps its folders, open tabs and layout together; the name shows at the head of the left bar. Open workspace… lists every saved one; pick one and it opens in its own window. Close workspace drops the name and leaves everything where it was.

![Open workspace: the picker listing the saved workspaces](guide/workspaces.png)

## Settings

Ctrl+, opens Settings, or the gear at the foot of the left bar, or type "settings" (or "config") in the palette. Seven groups: Page, Reading, Writing, Appearance, Interface, Shortcuts, Updates. Every change applies as you make it.

Your settings are a plain file, `settings.json`; "Show in Explorer" opens the folder. Edit it by hand if you like; your edits survive. Reset a group with "Reset group", or all of it from the foot of the dialog.

## Keyboard

Ctrl+K opens the palette, and every command in the app lives there; start typing what you want. Ctrl+, Settings. Ctrl+O open, Ctrl+S save (saves are atomic; a crash can't corrupt your words). Ctrl+F find. Ctrl+Z walks anything back. Ctrl+Enter presses a button in the text, like the two on the welcome page; Ctrl+click follows a link. Settings › Shortcuts lists every chord and lets you change any of them; "Test a chord" tells you whether your system is swallowing one before Buttermark sees it.

## Files

Buttermark writes ordinary `.md` files to your disk. No account, no vault, no database. Nothing leaves your machine unless you send it. Updates arrive on their own and ask before they install. If you ever stop using Buttermark, your files don't notice.

That's the lot. Like good butter, it's better spread than explained.
