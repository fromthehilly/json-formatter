# JSON Formatter

A small, dependency-free JSON formatter, minifier and validator. Everything runs in the browser; nothing is uploaded.

**Features:** format / minify, 2 or 4 spaces or tabs, sort keys, error messages with line and column, syntax highlighting, open or drag-and-drop a file, copy, download, light/dark theme.

There is also an XML formatter at `xml.html` (format, minify, well-formedness check with the parser's error message, syntax highlighting, open/drop file, copy, download).

Also included:

- `yaml.html`: format, validate (with line and column), convert to JSON, sort keys. Formatting re-writes the YAML, so comments are not kept.
- `sql.html`: format SQL for many dialects (PostgreSQL, MySQL, SQLite, T-SQL, Oracle, BigQuery and more). It formats only; it does not check that a query is valid for your database.

The YAML and SQL pages use two small libraries that are bundled in `vendor/` (so nothing loads from a CDN): [js-yaml](https://github.com/nodeca/js-yaml) 4.1.0 and [sql-formatter](https://github.com/sql-formatter-org/sql-formatter) 15.4.5, both MIT licensed (licenses included).

## Use locally

Open `index.html` in a browser. There is no build step.

## Publish on GitHub Pages

1. Create a repository (for example `json-formatter`) and push these files to the `main` branch.
2. In the repository go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. After a minute the site is live at `https://<your-username>.github.io/json-formatter/`.
