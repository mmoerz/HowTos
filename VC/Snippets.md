# Snippets

## Step before defining a new Code Snippet
Check if the code snippet shortcut already exists:
In VC type CTRL+J, use the filter bar at the end of the drop down to only show
snippets (outmost right symbol) and check that the drop down doesn't contain
the new shortcut.

## XML Structure

The basic structure looks like:
```
```

tagname | purpose
------- | -------
title | that is displayed for the snippet (on import, etc.)
author | the one responsible ...
description | for the not so lazy ones
shortcut | is the string that invokes the snippet (but optional)
code language | the language the snippet is written for e.g. CSharp, html
CDATA | that's the actual code that get's replaced, including CRs etc.


### Parameters

Parameters are defined after CDATA.
Their structure looks like:
```
```


## Visual Studio Code

VSCode is only used as a text editor here.
create new file with ending ```.snippet```
Change the contenttype to xml: click on Plaintext and type xml and select it

Notes on the code:
- shortcut is the text that gets expanded on hitting TAB, TAB
- Code Language e.g.:
  - CSharp
  - html


## Import in Visual Studio

Tools -> Code Snippet Manager
  select Language
  select File

  Place it in ```MyCodeSnippets```

## Snippet template

```
```
