# AION Lab website

Kyung Hee University AION Lab website, built with Jekyll and hosted on GitHub Pages.

## Local setup (Windows)

1. Install [Ruby+Devkit 3.1](https://rubyinstaller.org/downloads/) and Git. Ruby 3.1 is used because the `github-pages` gem can have compatibility issues with Ruby 3.2 or newer.
2. Open a new terminal in this repository and install Bundler if needed: `gem install bundler`.
3. Install dependencies: `bundle install`.
4. Start the preview: `bundle exec jekyll serve --livereload`.
5. Open <http://127.0.0.1:4000/>. Stop the server with Ctrl+C.

To check the site without starting a server, run `bundle exec jekyll build`.

## Editing guide

- `index.md`: home page
- `research.md`, `publications.md`, `people.md`, `professor.md`, `students.md`, `talks.md`, `photos.md`, `member-gathering.md`, `contact.md`: page content
- `assets/main.scss`: active site styles
- `_includes/header.html`: navigation
- `_includes/head.html`: page head and stylesheet link
- `_layouts/`: shared page structure
- `_config.yml`: site title, theme, and navigation settings
- `assets/images/`, `assets/people/`, and `assets/photos/`: images
- `_data/students.yml`: student groups and member profiles shown on People and Students pages

The header uses `assets/images/aionlab-mark-renewed.png`, a simplified version of the original AION Lab chip-and-neural-circuit mark. The adjacent Kyung Hee University emblem is `assets/images/khu-logo-official.png`, sourced from the [university's official identity page](https://www.khu.ac.kr/eng/user/contents/view.do?menuNo=300017).

Create a branch for changes, preview them locally, and review `git diff` before committing. Pushing a publishing branch can update the live GitHub Pages site.
