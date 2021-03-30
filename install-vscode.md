# Install VSCode

This document contains simple instructions for installing VSCode.

## Download VSCode

You can download VSCode [from here](https://code.visualstudio.com/Download). Once downloaded, run the install. 

## Setup

1. Once installed, click in the user icon in the lower left corner:

![vscode](https://user-images.githubusercontent.com/516548/112903017-97c55a00-90ac-11eb-9077-e9c34b3e8a6f.png)

2. Click sign in to sync settings. 
3. Select whichever account applies. There will be two options, GitHub and Microsoft. I save my settings to GitHub. In either case, it will open a browser session for you to authenticate into the site. 
4. Once authenticated, it will sync down any settings previously saved, including any installed plugins/extensions. Any changes made to VSCode will be synced to your account. 

<br/>

## Plugins (Extensions)

Here is the list of plugins I install from scratch (assuming I can't get to my synced content on GitHub):

```txt
Auto Close Tag
Better HAML
Bracket Pair Colorizer 2
Disable ESLint Rule
EditorConfig for VSCode
Erb-types
ESLint
Git
Git Blame
Git Graph
Git History
GitLens
Import Cost
JavaScript ES6 Snippets
Language Stylus
Live Server
Material Icon Theme
Prettier
Rails Edit Credentials
Rails i18n
Ruby
Ruby HAML
Simple Icons
VSCode Database
Markdown All in One
Markdown Converter
Markdown Preview Enhanced
MarkdownLint
Sass
Sublime Comands
Sublime Text Keymap
Slim
Sunburst Theme
TODO Highlight
Pug extension pack
Vetur
Vue Peek
Vue VS Code Extension Pack
vscode-elixir
XML Tools
Rainbow CSV
Edit csv
Svelte for VSCode
```

After extension are installed, I open preferences and settings.

<br/>

## Settings

To get to the settings click `File > Preferences > Settings`

When the settings open, I click the JSON settings icon:

![vscode settings](https://user-images.githubusercontent.com/516548/112904337-69487e80-90ae-11eb-8416-19d0db5ffafe.png)

Then I paste the following:

```json
{
  "workbench.startupEditor": "newUntitledFile",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Sunburst",
  "editor.minimap.enabled": false,
  "editor.tabSize": 2,
  "editor.detectIndentation": false,
  "editor.wordWrap": "on",
  "files.trimTrailingWhitespace": true,
  "diffEditor.ignoreTrimWhitespace": false,
  "files.trimFinalNewlines": true,
  "explorer.confirmDelete": false,
  "editor.rulers": [
    120
  ],
"explorer.confirmDragAndDrop": false,
  "gitlens.advanced.messages": {
    "suppressGitMissingWarning": true
  }
}
```

Once your account is ready to sync, your extensions are installed and your JSON settings are in place, you are good to go. The next time you install VSCode, simply log in to your account and all the extensions and settings will automatically pull down to VSCode, saving you a ton of time in setup.

Now you are ready to move to the next setup step, which can be found [here](https://github.com/scott-knight/ubuntu-on-windows-setup/blob/main/install-windows-terminal.md) 
