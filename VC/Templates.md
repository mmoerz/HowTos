# Templates

## Options

Creating a C# Template project
As a New Project - Search for Extensions
C# Item Template (*hints* ther is c# project template)

Exporting an Itemtemplate using:

Menu - Project - Export Template...

- select the project where the source for the template is stored
- select the item to export
- select item references: most often left alone, for .net framework libraries (not for nuget packages)
- select template options
  - add name, description
  - check output location
  - remove import checkbox

## install template

Install template by copying the .zip file to the ItemTemplates folder. Better
place it in the respective language folder (e.g. into c# subfolder).

### Template location
Your document folder /Visual Studio 2019/Templates/ItemTemplates

Subdirectories for Code, Data, WPF, etc. so that it shows up in the respective
folder in VC.

ItemTemplate consists of:
- Icon
- cs
- template xml definition

special replacement text:

text | replaced with
---- | -------------
$username$ | username of the logging in user
$time$ | time of creation
$itemname$ | the name of the template item created
$rootnamespace$ | name of the root namespace (project) where the item is added.

safe prefix for all exists, meaning the in the safe prefixed variable the
contents are escaped for safe use = spaces get replaced by "_".


