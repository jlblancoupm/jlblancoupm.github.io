# jlblancoupm.github.io — website V1

First functional Jekyll/GitHub Pages version of the academic profile for José Luis Blanco Murillo.

## Design principles

- Clean academic profile inspired by the structure used by other GAPS researchers.
- Jekyll + YAML data + GitHub Pages; no application server, database or public API.
- The landing page is deliberately short. Detail belongs on internal pages.
- Research, Applied R&D and Transfer are separate concepts; funding source is not used as the primary classification.
- Supervision is a first-level activity, not a subsection of Teaching.
- The public repository must contain public/sanitized data only.

## Pages

- `/` — landing
- `/research/`
- `/applied-rd/`
- `/transfer/`
- `/supervision/`
- `/publications/`
- `/code/`

## Local preview

A pre-rendered preview is included in `preview/`. Open `preview/index.html` directly.

For a real Jekyll build on a machine with Ruby/Bundler:

```bash
bundle install
bundle exec jekyll serve
```

## Publishing rule

The Pages workflow deploys only after content reaches `main`. The intended operating model is:

1. automated discovery happens in the separate private `profile-data` repository;
2. a pull request proposes changes;
3. Telegram notifies the owner;
4. the owner verifies attribution and publication visibility;
5. only approved public data is exported to this repository;
6. the website change is reviewed;
7. merge to `main` triggers GitHub Pages deployment.

The automatic discovery/Telegram workflow is intentionally **not** connected in this V1; it is the next implementation phase.


## Public structure (V2)

Primary navigation is intentionally compact: **About · Research · Supervision · Publications**.

Research is the central section and has two branches:

1. **Research directions** — current methodological/system research, with papers, code and demos attached to the relevant examples rather than collected in a standalone Code page.
2. **Projects & funding** — competitive research, industry-funded R&D, and transfer & innovation.

Standalone `Applied R&D`, `Transfer`, and `Code` sections were removed in V2.
