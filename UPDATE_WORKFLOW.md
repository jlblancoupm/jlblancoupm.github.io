# Update workflow

Automatic discovery must never deploy directly.

Planned flow:

1. ORCID / OpenAlex / Crossref / GitHub detect candidates in private `profile-data`.
2. A private pull request is created.
3. Telegram notification is sent.
4. José Luis reviews attribution and metadata.
5. Approved records enter canonical private data.
6. A sanitized public export proposes a pull request to this repository.
7. José Luis reviews the public change.
8. Only a manual merge to `main` triggers GitHub Pages deployment.
