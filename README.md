# Atom dbt package
Provides syntax highlighting and a number of snippets for dbt-flavored SQL, YAML and Markdown files in Atom.

## Configuration
After installing, set Atom to use Jinja-flavored Markdown/SQL/YAML by default:
1. Open your `config.cson` file (`Atom` from the menu bar, and then `Config`).
2. Add the following snippet:
```cson
"*":
  core:
    customFileTypes:
      "source.sql.jinja": [
        "sql"
      ]
      "source.gfm.jinja": [
        "md"
      ]
      "source.yaml.jinja": [
        "yml"
      ]
```
If you have packagess that that are enabled for one of the above languages, such as `markdown-preview` or `spell-check`, you will need to add the jinja-flavored language to that package:
1. Use the shortcut `Cmd + ,` to go to the Settings View
2. Navigate to `Packages`, and select the relevant package.
3. Add `source.gfm.jinja` (or relevant grammar) to the `grammars` section

## Usage
* Highlighting: SQL, YAML and Markdown files will be highlighted when using the Jinja-flavored grammar.
* Snippets: To use snippets, type one of the prefixes (e.g. `macro`), and then `tab`.
* Commenting: This package overrides the default comment behavior of each language to instead use Jinja comments. Use `Cmd + /` to comment out code.