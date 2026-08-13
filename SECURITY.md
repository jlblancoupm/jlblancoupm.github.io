# Public website security/data boundary

This repository is intended to be public and therefore must contain **public information only**.

Never commit:

- full/private CV exports;
- birth date, identity numbers, telephone numbers or private contact data;
- private project notes;
- project amounts or contractual details not explicitly approved;
- confidential partner information;
- CV generation sources/outputs;
- Telegram tokens, chat IDs or other secrets;
- private canonical research/project datasets.

The canonical dataset and automated discovery jobs live in the separate private `profile-data` repository. The website receives a whitelist-based sanitized export only after human review.
