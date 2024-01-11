# CSS 
## Visual Studio Code - MarkDown Preview

This css file extends the vscode MarkDown preview with a hierarchical numbering of the headings.
Starting at level 2 (`##`) to allow titles as level 1.

## Installation
### Filesystem

Add the relative path to `markdonw-numbering.css` file in the settings:  
  File > Preferences > Settings > Markdown: Styles

_vscode restriction (state 2024/01/01):_ It is not possible to set an absolute path, so the css file must be copied to each workspace: 
> A list of URLs or local paths to CSS style sheets to use from the Markdown preview. Relative paths are interpreted relative to the folder open in the Explorer. If there is no open folder, they are interpreted relative to the location of the Markdown file. All '\' need to be written as '\\'.

Alternativly you can use the web page setting

### Setup as https Page

The web page must deliver the css file with the mime type `text/css`

Hint:

If sites return their content as plaintext, likely because they don't want to be used as a generic CDN for stylesheets and script, vscode do not accept it.

`used to apply style from 'https://XXX' because its MIME type ('text/plain') is not a supported stylesheet MIME type, and strict MIME checking is enabled.`


Source of info: [github.com/microsoft/vscode/issues/148677#issuecomment-1118027411](https://github.com/microsoft/vscode/issues/148677#issuecomment-1118027411)

