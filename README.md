# custom-vscode-themes README

I like the default syntax highlighting of vscodes Dark+ theme so I just converted a couple themes that I liked into having the default syntax highlighting. I don't know if this is the complete default syntax highlighting but it's as close as I could get.

## Usage

Clone the repository into the extensions folder. In Windows that folder is `C:\Users\Your_Username\.vscode\extensions`. The name of the cloned folder may need to represent the package version. Eg. look in package.json and if the package number is 0.0.1 then your folder should be named `custom-vscode-themes-0.0.1`.

### Customizing your own themes

Add a theme to the `theme` folder and then in `package.json` make sure the add it to the `contributes.themes` like so:

```json
{
    "label": "Your Theme Name",
    "uiTheme": "vs-dark",
    "path": "./themes/path-to-theme.json"
},
```

If you like the default syntax like me then you can just include the `./syntax.json` file in your theme.

**Enjoy!**
