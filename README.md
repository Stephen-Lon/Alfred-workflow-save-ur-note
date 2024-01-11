# Alfred-workflow-save-ur-note
A workflow to create and save quick, temporary plain text notes

# Introduction

Sometimes when working you want to make a short, temporary quick note for future reference without bothering to open a dedicated Notes app. That is what this workflow does. It uses a simple plain text file (which will be created for you when you first create a note by running the workflow) to which saved notes will be appended (rather like a scratch pad). You select the location folder for that file in the workflow configuration.

However, the workflow does a little more than that. You can also save text clippings by selecting text and using your Universal Action hot key on the selected text.

# Setup

In the workflow configuration choose:
- the folder where you want to keep your `QuickNote.txt` file;
- the keyword you want to use to create a quick note;
- the keyword you want to use the view the `QuickNote.txt` in QuickLook;
- the keyword you want to use to *open* the `QuickNote.txt` file in your default text editor;
- the keyword you want to use to *delete* the `QuickNote.txt` file.

# Usage—saving quick notes

There are two ways in which to create a quick note.

1. You can use your Universal Action hotkey on selected text, choose `Save a quick note` from the list and press ⏎. The selected text will be saved in the quick notes file (which is created if it does not already exist) together with the date and time the note was appended.

2. You can use the keyword set to create a quick note and type the text of the note. In that case that you must type a single line of text (with spaces and punctuation as necessary, of course): you cannot use newlines or returns to create a multi-line note. (There is no such restriction if you are *copying* selected text as in 1 above.)

# Usage—viewing quick notes

The result of saving quick notes will be a plain text file which you can open in your default text editor by using the relevant keyword set in the workflow configuation (by default `vqn` for "view quick notes").

You can also view the file in QuickLook by using the relevant keyword set in the workflow configuation (by default `vql` for "view [using] QuickLook").

**Note**: [DEBUG] in the QuickLook window title is a function of the command line `qlmanage` and (so far as I am aware) cannot be avoided.

# Usage—deleting the quick notes file

Simply use the keyword set in the workflow configuration (by default `dqn` for "delete quick notes") to move the quick notes file to the Trash.
