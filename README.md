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

Below is a list of all available snippets.

### Basic
| Trigger  | Content |
| -------: | ------- |
| `e=`     | render block `<%= %>`|
| `e-`     | exec block `<%- %>`|
| `e#`     | comment `<%# %>`|
| `end`    | end tag `<% end %>`|
| `lt`     | link `<%= link \"${1:text}\", to: ${2:url} %>`|
| `render` | render `<%= render \"${1:partial}.html\", ${2:local_var: @local} %>`|

### Control flow

| Trigger   | Content |
| -------:  | ------- |
| `for`     | for `<%= for $1 <- $1 do %>`|
| `if`      | if `<%= if $1 do %>`|
| `ife`     | if else `<%= if $1 do %> <% else %>`|
| `cond`    | cond `<%= cond do %>`|
| `unless`  | unless `<%= unless $1 do %>`|

### Forms

| Trigger  | Content |
| -------: | ------- |
| `ff`     | form_for `<%= form_for @${1:changeset}, ${2:url}, ${3:[]}, fn f -> %>`|
| `et`     | form error `<%= error_tag ${1:f}, :${2:field} %>`|
| `la`     | form label `<%= label ${1:f}, :${2:field}, \"${3:Text}\" %>`|
| `ti`     | form text input `<%= text_input ${1:f}, :${2:field} %>`|
| `pi`     | form password input `<%= password_input ${1:f}, :${2:field} %>`|
| `subm`   | form submit `<%= submit ${1:Text} %>`|
| `submc`  | form submit with class `<%= submit ${1:Text}, class: \"${3:btn btn-primary}\" %>`|


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
