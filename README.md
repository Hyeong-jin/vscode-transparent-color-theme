# HJY Transparent Color Theme

<img src="images/icon.png" style="height:100px;float:right"></img>

Experience the ultimate coding environment with the HJY Transparent Color theme.
Designed exclusively for macOS, this theme brings the stunning vibrancy
background blur of macOS to Visual Studio Code. Enjoy a sleek and modern coding
experience with translucent backgrounds that seamlessly blend with the rest of
your macOS interface.

## Screenshots

![Screenshot](images/screenshot.png)

## Installation

1. Launch Visual Studio Code
2. Go to the Extensions view by clicking on the square icon on the left side
   toolbar or by pressing `Ctrl+Shift+X`
3. Search for "HJY Transparent Color Theme" and click on the "Install" button
4. Once the theme is installed, click on the "Reload" button to activate it

### Blur effect

To achieve the transparent effect with Visual Studio Code, you can use the
[Apc Customize UI++](https://marketplace.visualstudio.com/items?itemName=drcika.apc-extension)
extension. It allows you to configure the transparency settings by adding the
following settings to your VS Code settings.json:

```json
"apc.electron": {
    "opacity": 0.95,
    "transparent": true,
    "backgroundColor": "#00000000",
    "vibrancy": "ultra-dark"
},
```

## Additional

### Cursor Blinking Effect

```json
"apc.stylesheet": {
        ".monaco-editor .cursor": "background: #ffffffaa !important; box-shadow: 0 0 70px 5px #ffffff, #ffffff 0px 0px 34px 1px; color: #161616 !important",
},
"editor.cursorBlinking": "phase",
"editor.cursorSmoothCaretAnimation": "on",
```

### Font with ligatures
You can download FiraCode Font on [this link](https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/FiraCode)
```json
"editor.fontFamily": "'FiraCode Nerd Font Mono', 'FiraCode Nerd Font', FiraCode, Menlo, Monaco, 'Courier New', monospace",
"editor.fontLigatures": true,
```

### UI Animations
There is great extension [VSCode Animations](https://marketplace.visualstudio.com/items?itemName=BrandonKirbyson.vscode-animations). You can use it with [Apc Customize UI++](https://marketplace.visualstudio.com/items?itemName=drcika.apc-extension), but check VSCode Animations custom injection plugin readme section
```json
"apc.imports": [
    "file:///~/.vscode/extensions/brandonkirbyson.vscode-animations-1.0.14/dist/updateHandler.js"
],
```
Example config:
```json
"animations.Enabled": true,
"animations.CursorAnimation": true,
"animations.Command-Palette": "None",
"animations.CursorAnimationOptions": {
    "TrailLength": 10
},
"animations.Tabs": "Slide",
"animations.Active": "Indent",
```

## Theme Details

- **Name**: HJY Transparent Color Theme
- **Version**: 1.0.0
- **VS Code Version**: 1.81.0 and above
- **Keywords**: theme, transparent, macOS, vibrancy, ultra-dark, glass
- **Categories**: Themes
- **Extension Pack**:
  [drcika.apc-extension](https://marketplace.visualstudio.com/items?itemName=drcika.apc-extension)
  [BrandonKirbyson.vscode-animations](https://marketplace.visualstudio.com/items?itemName=BrandonKirbyson.vscode-animations)

## Contributing

If you have any suggestions, bug reports, or feature requests, please
[open an issue](https://github.com/Hyeong-jin/vscode-transparent-color-theme/issues).

## License

This theme is licensed under the [MIT License](LICENSE).
