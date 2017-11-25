# EEx snippets

This extension contains code snippets for Elixir `.eex` and `.html.eex` files for [VS Code](https://code.visualstudio.com/) editor.

## Installation

In order to install an extension you need to launch the Command Pallete (Ctrl + Shift + P or Cmd + Shift + P) and type Extensions.
There you have either the option to show the already installed snippets or install new ones. Search for **'EEx snippets'** and install it.

**Enjoy!!!**

## Supported languages (file extensions)
* EEx (.eex)
* HTML (EEx) (.html.eex)

## Snippets

Below is a list of all available snippets and the triggers of each one. The **->** means the `TAB` key.

### Import and export
| Trigger  | Content |
| -------: | ------- |
| `e=→`   | render block `<%= %>`|
| `e-→`   | exec block `<%- %>`|
| `e#→`   | comment block `<%# %>`|

TODO: Document here all the snippets

## Release Notes

### 0.0.1

Initial release of first snippets

## Known Issues

Not really an issue but I wanted the `e=, e-, e#` snippets to be just a `=, -, #`, but they didn't trigger on these special characters so had to prepend them with `e` letter.

## Disclaimer

Graciously borrowed some of the snippets from the [phoenix-elixir-snippets](https://atom.io/packages/phoenix-elixir-snippets) for Atom and refactored them to work with VS Code.

## Contribution

```
git clone https://github.com/florinpatrascu/vscode-elixir-snippets.git
```
And copy the `vscode-elixir-snippets` folder into the `<user home>/.vscode/extensions` folder. Restart Code.

## License

[MIT](LICENSE.md) License

Copyright (c) 2017 Stefan jarina
