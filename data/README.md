# data/ — local only, never committed

This folder is where client files live **on your own computer** while you work on this project: daily sales reports, the client's spreadsheets, exports, and CSVs.

Everything in this folder except this README is gitignored. `*.pdf`, `*.xlsx`, `*.xls`, `*.xlsm`, and `*.csv` are also ignored everywhere else in the repo.

**Never commit client data.** This repository is public. Anything pushed to GitHub can be copied or indexed within minutes, and it stays in the history even if the file is deleted in a later commit.

- Keep real files here or in the club's Google Drive (ask Cayden where). Nowhere else.
- Never use `git add -f` to force a file from this folder into a commit.
- Tests and examples that live in the repo use fabricated numbers you typed yourself, clearly labeled as fake.
- If client data is ever committed or pushed by mistake, stop and tell Cayden right away. Do not try to fix it yourself with another commit.
