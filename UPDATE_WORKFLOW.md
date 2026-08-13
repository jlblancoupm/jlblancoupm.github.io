# Update workflow — mandatory human approval

The website must never publish newly discovered content automatically.

## Final intended flow

```text
ORCID / Crossref / OpenAlex / GitHub
                |
                v
        private profile-data
        candidate detection
                |
                v
      Pull Request (private)
                |
                +----> Telegram notification
                |      - new records
                |      - changed records
                |      - attribution warnings
                |      - review link
                v
      HUMAN DATA REVIEW
        reject / approve
                |
                v
      sanitized public export
                |
                v
    website Pull Request
                |
                +----> Telegram notification
                |      - public diff summary
                |      - rendered screenshots
                |      - review link
                v
     HUMAN WEBSITE REVIEW
        reject / merge
                |
                v
              main
                |
                v
         GitHub Pages deploy
```

## Approval semantics

Three distinct decisions are required:

1. **Attribution approval** — the item is genuinely associated with José Luis Blanco Murillo and its metadata are correct.
2. **Visibility approval** — the sanitized representation is acceptable for public disclosure.
3. **Website approval** — the final website change is accepted and merged.

No discovery job is allowed to push directly to `main` in the website repository.

## Telegram

Telegram notification is mandatory for automated candidate/update PRs. Tokens and chat IDs belong only in GitHub Secrets in the private repository. They must never be committed to either repository.

A reminder notification may be added for review PRs that remain pending for a configurable number of days.
