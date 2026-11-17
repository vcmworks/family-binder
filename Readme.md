# Family Emergency Binder

A single-file, offline web app that helps a family record the key information a spouse would need if something happened: accounts, insurance, legal documents, digital access, and a first-steps checklist. Adapted for households in Germany and India.

## Features

| Feature | Detail |
|---|---|
| Single file | `index.html`, no dependencies, no server, no tracking |
| Residence profiles | Toggle Germany / India to show relevant fields and checklist items |
| Customisable | Add or remove entries, fields and checklist items; "Other (custom)" in every section |
| Encrypted save | AES-256-GCM, PBKDF2-SHA256 (600k iterations), via the browser Web Crypto API |
| Plain JSON | Optional unencrypted export, with a warning |
| Load | Restores data from encrypted or plain JSON |
| PDF / Print | Print stylesheet, one section per page; use "Save as PDF" |
| Chores sheet | W / H / T ownership table |

## Usage

1. Download `index.html` and open it in a browser.
2. Tick your residence(s), fill in the sections.
3. Click **Save encrypted** and store the file safely.
4. Use **Load JSON** to continue later.

## Security notes

- Data never leaves your device; nothing is stored in the browser.
- Lost passwords cannot be recovered.
- Print and PDF output is unencrypted; handle it accordingly.
- Do not store full passwords or full card numbers. Record where they are kept.
- Do not commit your saved JSON to this repo (see `.gitignore`).

## Disclaimer

The checklist is a starting point, not legal or tax advice. Confirm procedures with a Notar, Steuerberater, or the relevant consulate.

## Credits

Content structure inspired by the "Family Emergency Binder" and "Household Chores 101" templates by @rajsnapz. Confirm you have permission to reuse or redistribute their content before publishing.

## License

MIT (or your choice)
