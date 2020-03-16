# EEx snippets

This extension contains code snippets for Elixir `.eex` and `.html.eex` files for [VS Code](https://code.visualstudio.com/) editor.

**Enjoy!!!**

## Supported languages (file extensions)

- EEx (.eex)
- HTML (EEx) (.html.eex)

## Snippets

Below is a list of all available snippets.

### Basic

|            Trigger | Content                                                                                             |
| -----------------: | --------------------------------------------------------------------------------------------------- |
|               `e=` | render block `<%= %>`                                                                               |
| `ee` <br/> or `e-` | exec block `<% %>`                                                                                  |
|               `e#` | comment `<%# %>`                                                                                    |
|              `end` | end tag `<% end %>`                                                                                 |
|               `lt` | link `<%= link "${1:text}", to: ${2:url} %>`                                                        |
|              `ltb` | link block <br>`<%= link to: ${1:url} do %>`<br>&nbsp;&nbsp;&nbsp;&nbsp;`${2:text}`<br>`<% end %>"` |
|           `render` | render `<%= render "${1:partial}.html", ${2:local_var: @local} %>`                                  |

### Control flow

|  Trigger | Content                              |
| -------: | ------------------------------------ |
|    `for` | for `<%= for $1 <- $1 do %>`         |
|     `if` | if `<%= if $1 do %>`                 |
|    `ife` | if else `<%= if $1 do %> <% else %>` |
|   `cond` | cond `<%= cond do %>`                |
| `unless` | unless `<%= unless $1 do %>`         |

### Forms

| Trigger | Content                                                                         |
| ------: | ------------------------------------------------------------------------------- |
|    `ff` | form_for `<%= form_for @${1:changeset}, ${2:url}, ${3:[]}, fn f -> %>`          |
|    `et` | form error `<%= error_tag ${1:f}, :${2:field} %>`                               |
|    `la` | form label `<%= label ${1:f}, :${2:field}, "${3:Text}" %>`                      |
|    `ti` | form text input `<%= text_input ${1:f}, :${2:field} %>`                         |
|    `pi` | form password input `<%= password_input ${1:f}, :${2:field} %>`                 |
|  `subm` | form submit `<%= submit ${1:Text} %>`                                           |
| `submc` | form submit with class `<%= submit ${1:Text}, class: "${3:btn btn-primary}" %>` |

## Release Notes

Please read the [CHANGELOG](CHANGELOG.md) to see what has changed in this extension over time.

## Known Issues

Not really an issue but I wanted the `e=, e-, e#` snippets to be just a `=, -, #`, but they didn't trigger on these special characters so had to prepend them with `e` letter.

## Disclaimer

Graciously borrowed some of the snippets from the [phoenix-elixir-snippets](https://atom.io/packages/phoenix-elixir-snippets) for Atom and refactored them to work with VS Code.

## Contribution

```
git clone https://github.com/stefanjarina/vscode-eex-snippets
```

And copy the `vscode-eex-snippets` folder into the `<user home>/.vscode/extensions` folder. Restart Code.

## License

[MIT](LICENSE.md) License

Copyright (c) 2017 Stefan jarina
