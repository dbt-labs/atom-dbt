# Atom dbt package

Provides syntax highlighting and a number of snippets for dbt-flavored SQL, YAML and Markdown files in Atom.

## Installation
1. Clone this repo
2. `cd` into the repo and run `apm link`
3. Reload your atom window (`View > Developer > Reload Window`). If the changes do not take effect right away, try quitting and restarting your Atom editor.

## Usage
* Highlighting: SQL, YAML and Markdown files will be highlighted automatically
* Snippets: To use snippets, type one of the prefixes (e.g. `macro`) macro, and then `tab`.
* Commenting: This package overrides the default comment behavior of each language to instead use Jinja comments. Use `Cmd + /` to comment out code.