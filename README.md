This is the website of [L’Équipe Z](https://equipez.github.io).

# How to edit

1. Clone this repository using `git clone git@github.com:equipez/equipez.github.io.git`.
2. Create or edit Markdown files within the repository.
3. Commit and push your changes.

- Add links to the homepage using relative paths without the `.md` extension.
  - Example: `[README](./README)`.
- Refer to the [GitHub Pages documentation](https://docs.github.com/en/pages)
  for more advanced configuration.

## Preview locally

This site uses GitHub Pages and Jekyll. VS Code extensions such as Live Server do not process
Jekyll layouts, Liquid templates, or the GitHub Pages theme, so use the Jekyll development server
for an accurate preview.

1. Install Ruby.
2. Install Bundler if it is not already available:

   ```shell
   gem install bundler -v 2.5.11
   ```

3. From the repository root, install the dependencies:

   ```shell
   bundle install
   ```

4. Start the local server with automatic browser refresh:

   ```shell
   bundle exec jekyll serve --livereload
   ```

5. Open <http://127.0.0.1:4000/>. Press `Ctrl+C` in the terminal to stop the server.

Generated site files, Bundler state, operating-system metadata, and common editor files are ignored
by Git. `Gemfile.lock` is intentionally untracked so that native dependencies can be resolved for
macOS, Linux, and Windows; the `github-pages` gem itself is pinned to the version used in production.

## Add a research update

Add new entries to the top of `/_data/updates.yml`. Keep the date in `YYYY-MM-DD` format and provide
the update type, title, authors, and primary link. The six newest entries appear on the homepage;
the complete list appears on `/updates`.

```yaml
- date: "2026-06-02"
  type: "New preprint"
  title: "Paper title"
  authors: "Author One and Author Two"
  url: "https://example.com/paper"
```

## Edit layouts

Edit `/_layouts/default.html` directly.

Note: This file supports HTML syntax and [Liquid](https://shopify.github.io/liquid/)
syntax, but not Markdown syntax.
