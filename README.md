# vscode-squid-settings (v1)
Permet d'importer facilement les paramètres, extensions, polices et thèmes pour VS Code d'un ordinateur sur l'autre.

***
## 1/ Extensions
Liste des extensions utilisées :
### -- Thème
* [Material Theme](https://marketplace.visualstudio.com/items?itemName=Equinusocio.vsc-material-theme)
### -- Code
* [Visual Studio IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)
* [REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client)
* [Quokka.js](https://marketplace.visualstudio.com/items?itemName=WallabyJs.quokka-vscode)
* [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
* [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
* [Live SASS Compiler](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass)
* [Javascript (ES6) code snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets)
* [Ionic Snippets](https://marketplace.visualstudio.com/items?itemName=fivethree.vscode-ionic-snippets)
* [indent-rainbow](https://marketplace.visualstudio.com/items?itemName=oderwat.indent-rainbow)
* [HTML CSS Support](https://marketplace.visualstudio.com/items?itemName=ecmel.vscode-html-css)
* [CSS Peek](https://marketplace.visualstudio.com/items?itemName=pranaygp.vscode-css-peek)
* [Bracket Pair Colorizer 2](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer-2)
* [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
* [Angular Snippets](https://marketplace.visualstudio.com/items?itemName=johnpapa.Angular2)
### -- Autres
* [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons)
* [Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)
* [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
* [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
* [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
* [Custom CSS and JS loader](https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-custom-css)

## 2/ Polices
Installer la police *"Operator Mono Lig"* située dans le dossier *"/fonts"*.  
**Source** : https://github.com/lissanh95/operator-mono-lig-1

## 3/ Intégration Cmder
Mettre le fichier *"vscode.bat"* à la racine du dossier d'installation de Cmder.  
**NE PAS OUBLIER** : Penser à changer le chemin du dossier Cmder dans le fichier *"vscode.bat"*

## 4/ Fichier settings.json
Mettre à jour le fichier settings.json de VS Code en suivant les étapes suivantes :  
* Ouvrir VS Code
* Taper F1
* Renseigner *"Open settings"* dans la barre de recherche
* Copier/coller le code ci-dessous dans le fichier *"settings.json"* qui vient de s'ouvrir
* **NE PAS OUBLIER** : Changer le chemin du fichier vscode.bat à la ligne *"terminal.integrated.shellArgs.windows"* du fichier settings.json
```
{
    "editor.fontFamily": "Operator Mono Lig, Consolas, 'Courier New', monospace",
    "editor.fontWeight": "100",
    "terminal.integrated.shell.windows": "C:\\WINDOWS\\system32\\cmd.exe",
    "terminal.integrated.shellArgs.windows": ["/K", "C:\\cmder\\vscode.bat"],
    "workbench.iconTheme": "vscode-icons",
    "workbench.colorTheme": "Material Theme Ocean",
    "workbench.colorCustomizations": {
        "activityBarBadge.background": "#C6FF00",
        "activityBar.activeBorder": "#C6FF00",
        "list.activeSelectionForeground": "#C6FF00",
        "list.inactiveSelectionForeground": "#C6FF00",
        "list.highlightForeground": "#C6FF00",
        "scrollbarSlider.activeBackground": "#C6FF0050",
        "editorSuggestWidget.highlightForeground": "#C6FF00",
        "textLink.foreground": "#C6FF00",
        "progressBar.background": "#C6FF00",
        "pickerGroup.foreground": "#C6FF00",
        "tab.activeBorder": "#C6FF00",
        "notificationLink.foreground": "#C6FF00",
        "editorWidget.resizeBorder": "#C6FF00",
        "editorWidget.border": "#C6FF00",
        "settings.modifiedItemIndicator": "#C6FF00",
        "settings.headerForeground": "#C6FF00",
        "panelTitle.activeBorder": "#C6FF00",
        "breadcrumb.activeSelectionForeground": "#C6FF00",
        "menu.selectionForeground": "#C6FF00",
        "menubar.selectionForeground": "#C6FF00",
        "editor.findMatchBorder": "#C6FF00",
        "selection.background": "#C6FF0040"
    },
    "materialTheme.accent": "Acid Lime",
    "editor.suggestSelection": "first",
    "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue"
}
```
