# jlblancoupm.github.io

Public academic profile of José Luis Blanco Murillo.

## Structure

- `JL` — landing
- `About`
- `Research`
- `Supervision`
- `Teaching`
- `Publications`

The site is generated with Jekyll and deployed through GitHub Pages.

## Data

Public content is stored under `_data/`. This repository must contain public/sanitized data only.
Private canonical data, automatic discovery and approval workflows belong in the separate private `profile-data` repository.

## Contact form

See `FORM_SETUP.md`. The public repository contains no recipient email address.

## V4.2 navigation

Top navigation links open in a new browser tab (`target="_blank"`) so the current page remains open.

## V4.3 supervision catalogue

Public student names follow the privacy convention **first-name initial + first surname only**. The public `_data/supervision.yml` intentionally contains no full student names. Filtering is client-side by level, degree, year (where available), research field, status, topic/method and free-text title/topic search. Research-field and topic assignments are editorial classifications derived from thesis/project titles; missing source metadata is left blank.

## V4.3.2 publications

Publications now default to a unified chronological **All** view.

Publication type codes:
- `J` — journal article
- `C` — conference contribution

Users can switch between All, Journal articles and Conference contributions.
Search, year and research-area filters work across the unified catalogue.

## V4.4 work-with-us flow

The supervision catalogue no longer embeds the application form.

- `Supervision` contains the catalogue, filters, open topics and a compact CTA.
- `Work with us` lives at `/work-with-us/`.
- The sidebar `Contact` link points directly to `/work-with-us/`.
- The form success and error messages are hidden on initial page load and are shown only by Formspree after submission.
- `Work with us` is intentionally not added to the top navigation.
