# jlblancoupm.github.io — V4.6

Stable public academic website for José Luis Blanco Murillo.

## Public structure

Top navigation: `JL · About · Research · Supervision · Teaching · Publications`. Top-menu links open in a new browser tab.

Supervision includes the PhD/MSc/BSc catalogue, abbreviated public student names, and client-side filters. Publications defaults to a combined journal/conference view and uses `J` / `C` type codes.

## Contact

V4.6 deliberately contains no public contact mechanism while the final private-contact architecture is being decided. The sidebar exposes ORCID and GitHub only. The Supervision page keeps a short “Interested in working with us?” section describing the documents normally needed for student enquiries.

## Private operational layer

Availability checks and GitHub repository-traffic history are maintained separately in the private `profile-data` repository.

## V4.6+

V4.6+ keeps the public website identical to the clean V4.6 baseline.
The "+" refers to the optional private operational layer in `profile-data`.

No Gmail address, recipient address, SMTP credential, token or contact form is
contained in this public repository.

## V4.7 contact
Contact is active through Google Apps Script. No recipient email address or mailto link is present in the public repository. Student enquiries use the same contact channel
but do not upload personal documents.

## V4.8

- redesigned Contact page;
- student-specific document uploads;
- optional attachment for other professional contact;
- early Student Opportunities CTA on Supervision;
- lower Student Opportunities anchor and direct student-enquiry link.

## V4.8.1

Contact feedback has been moved next to the Send action. Success and error
messages now appear directly below the Send button and no longer trigger
automatic page scrolling.


## V4.9

- Supervision rebuilt from the reviewed master catalogue.
- Supervision records now support multiple research fields through `fields:`.
- Human Communication & Behaviour renamed to Human Interaction & Behaviour.
- Documented years/dates incorporated; unknown MSc dates remain intentionally blank.
- Jaime Fernández López-Romero remains excluded from the public catalogue.
- Internal site links no longer open new tabs.
- Contact links go directly to `#contact-form`.
- Mobile profile/header now appears above the navigation tabs, with text on the left and avatar on the right.
- Contact / ORCID / GitHub are visually explicit profile actions.
- Normal mobile Contact is compact; optional attachment is collapsed until requested.
- Verified Apps Script endpoint retained in `_data/contact.yml`.

## V4.10

Full visual refresh based on the validated V4.9 structure:

- Blue academic visual system aligned more closely with the GAPS identity.
- Full-width landing hero on desktop, with no duplicated Research/Supervision/Publications preview blocks.
- Integrated JL / About / Research / Supervision / Teaching / Publications navigation retained.
- New line icons for the three landing research directions.
- Updated avatar: warmer medium-brown skin, lighter blue polo, compact green/yellow/red audio equalizer motif.
- Subtle signal-wave background artwork on the landing page.
- Contact remains the primary action; ORCID and GitHub are secondary but clearly clickable external links.
- Internal links stay in the same tab; external links stay in a new tab.
- Supervision uses the reviewed multi-field taxonomy and now renders areas as restrained editorial labels instead of large pills.
- Mobile keeps the profile header above the navigation tabs and the compact one-screen-oriented Contact layout from V4.9.
- Existing verified Google Apps Script contact endpoint retained unchanged.
