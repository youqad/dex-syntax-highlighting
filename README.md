# Dex Syntax Highlighting VSCode Extension


Syntax highlighting support for the [Dex language](https://github.com/google-research/dex-lang) in Visual Studio Code.

It is based on Dougal Maclaurin and Alexey Radul's Emacs Lisp Dex syntax highlighting [file](https://github.com/youqad/dex-lang/blob/main/misc/dex.el) and the [Haskell Syntax Highlighting Extension](https://github.com/JustusAdam/language-haskell).

![Screenshot Dex](/images/screenshot.png?raw=true)


# Contributing and Testing

To generate the JSON grammar (expected by VS Code) from the YAML-tmLanguage file, use the Node package `js-yaml`:

```sh
npx js-yaml syntaxes/dex.YAML-tmLanguage > syntaxes/dex.tmLanguage.json
```
Testing can be done with the Node package `vscode-tmgrammar-test`:

```sh
vscode-tmgrammar-test examples/prelude.dx
# ✓ examples/prelude.dx run successfuly.
```
