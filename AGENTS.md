# AION Lab website: Codex handoff

This file summarizes the decisions from the website editing conversation so a new Codex session can continue the work on another computer. It is a guide to the current site, not a substitute for checking the source files and `git status` before editing.

## Project and setup

- Repository: `https://github.com/yuntae1000/aionlab.git`
- Live site: `https://aionlab.khu.ac.kr/`
- Stack: Jekyll with the `github-pages` gem. The live site is published through GitHub Pages from this repository.
- On Windows, use Git and Ruby+Devkit 3.1. Run `gem install bundler` if needed, then `bundle install` and `bundle exec jekyll serve --livereload`. Preview at `http://127.0.0.1:4000/`.
- See `README.md` for the full setup and file map. The generated `_site/` directory and local Ruby dependencies are ignored by Git and should be rebuilt on the new computer.

## Confirmed content and design decisions

- This should read as an **academic research lab** website, with clean typography and restrained styling. The home slogan is **“Circuits for what matters.”** Inspiration included the KU Selene and KHU EDA lab websites, but the AION Lab site has its own layout.
- The header uses the renewed AION Lab mark and the Kyung Hee University logo. Navigation is Research, Publication, People, Talks, Photo, Contact.
- The home page order is hero, **Notice**, News, Contact. The 2027 spring graduate recruitment notice is prominent; news dates show year and month. The home introduction identifies the lab as **경희대학교 전자공학부 정윤태 교수 연구실**.
- The professor is **Yoontae (Jake) Jung / 정윤태**, Assistant Professor in the **School of Electronic Engineering**. Use **전자공학부** in Korean, not 전자공학과. The original full-resolution portrait is `assets/people/jake.jpg`.
- People shows Professor and Students directly on one page. Student groups are Graduate Students, Co-supervising Students, and Undergraduate Students. The graduate group currently has one “Join AION Lab” recruitment poster; the co-supervising group has Jimin Koo; the undergraduate group includes Heetae Lee and the other listed students. Member data lives in `_data/students.yml`; shared rendering lives in `_includes/student-groups.html`. Heetae is a one-row featured entry with his photo and an incoming M.S. note. Other undergraduates are text entries in a two-column layout without portrait placeholders.
- Publications combine journal and conference entries under **year headings**, newest first. The 2026 list includes the accepted ICCAD “IMC-Diff” paper and the IEEE TBCAS neural digitization and spike sorting paper. Check publication details against authoritative sources before changing factual claims.
- Talks are grouped by year; each entry includes venue or conference, city/country, date, and title. Preserve the distinction between confirmed talks and proposed talks.
- Photo contains a Member gathering post with the event date **24 August 2026**.
- Contact location is **Woojungwon, Room B6096**. Do not add a map unless requested.
- Research includes the **2026–2030 KEIT** project on high-reliability IP for sub-5-nm on-device AI semiconductors.
- Search metadata, canonical URLs, structured data, sitemap, and Search Console verification are already in the site. Search ranking is not guaranteed by these settings.

## Editing map

- `index.md`: home hero, notices, news, contact preview, and Korean affiliation.
- `research.md`, `publications.md`, `talks.md`, `photos.md`, `member-gathering.md`, `contact.md`: page content.
- `people.md`, `professor.md`, `_data/students.yml`, `_includes/student-groups.html`: people content.
- `_includes/header.html`, `_includes/head.html`, `_config.yml`: navigation and site metadata.
- `assets/main.scss`: active styling. Images are under `assets/images/`, `assets/people/`, and `assets/photos/`.

## Continuing on another computer

Clone the GitHub repository, attach the cloned `aionlab` folder as the primary local project in Codex, and read this file plus `README.md`. A Git clone brings the committed site and this handoff; Codex conversation history, local project attachment, account logins, and files outside the repository are separate. Before a new edit, check `git status` and pull the latest changes. Build or preview changes locally, review the diff, and commit and push when the user requests publication.
