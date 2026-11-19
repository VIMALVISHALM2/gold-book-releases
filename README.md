# Gold Book — program updates

This repository holds only **finished program files** for the Gold Book desktop app and a **signed version list**.
It contains no source-code history, no keys, no passwords and no account books — the books never leave the computer
they are kept on.

- `latest.json` + `latest.json.sig` — the newest version, signed (Ed25519). Gold Book refuses anything whose signature
  does not match the key built into it.
- `<version>/app.asar` — that version's program code, with its own signed manifest.

Gold Book checks here about once a day while it is open, sends nothing about its books, saves a backup of the books
before a new version first runs, and goes back to the previous version by itself if a new one does not start.
