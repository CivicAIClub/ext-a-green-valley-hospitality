# Green Valley Hospitality agent guide

## Purpose

This project automates daily sales reporting for Green Valley Hospitality's restaurants so each day's figures reach the company's reporting spreadsheets without being retyped. Student developers in Pomfret School's Civic AI Club build the tool for Green Valley Hospitality, LLC.

## Project rules and private information

- Read `README.md` and `.cursor/rules/ext-a-green-valley-hospitality.mdc` before working here. This is a standalone public repo for an external client; handle its information carefully.
- Recorded status: discovery is complete and Phase 1 has not started. The team is to be assigned, with Cayden Auyang as club lead. When developers are assigned, update the project rule's team line and `.github/CODEOWNERS`.
- Client data never goes in Git. Sales PDFs, exports, spreadsheets, customer lists and email lists stay in the gitignored `data/` folder or in Drive. The sources point to `data/README.md` for details.
- `.gitignore` blocks `data/*` except `data/README.md`, plus `*.pdf`, `*.xlsx`, `*.xls`, `*.xlsm` and `*.csv`. Never suggest `git add -f` to bypass it.
- Keep client contact details, discovery notes and client requirements out of code comments, tests, docs, commit messages and pull request descriptions. Do not put phone numbers, customer names or email addresses in code. Use fabricated values in tests and examples, and label them as fake.
- If client data is staged or committed, stop and tell the developer to contact Cayden. Deleting it in a later commit does not remove it from history.
- Private discovery notes, contacts and client requirements belong in the club's private running doc, linked from Civic AI Club Google Drive. Do not copy them into this repo. If a requirement is missing from code, ask the developer to check the running doc instead of guessing. Implement the requirement without pasting notes, examples or client data into comments.
- In client-facing emails, demos and handover docs, describe the work as a time-saving tool. Do not lead with "AI" or name the school's faculty projects. Do not promise scope or timelines without Cayden.
- Never commit API keys, tokens, mailbox passwords or `.env` files. Every environment variable needs a placeholder line in `.env.example`.
- The README does not specify a stack or setup/run commands. Do not invent them.

## Working with student developers

- Prefer clear code over clever code. If you generate code the developer cannot explain, say so and explain what it does in plain English.
- Paths in this guide are relative to this standalone repository. Each club project has its own repo. Do not edit the archived `Civic-AI-Github-Repository` monorepo.
- For Git, branches, pull requests or merge conflicts, use the Developer Onboarding Guide linked below instead of making up a workflow.
- Check with Cayden before changing `.github/` or `.cursor/rules/`. Keep the README accurate when setup changes.

## Git and pull requests

- Never push directly to `main`. Work on a branch and open a pull request. Merging needs at least one approving review.
- Name branches `feature/<short-description>`, `fix/<short-description>` or `chore/<short-description>`, using lowercase letters and hyphens, with no spaces.
- Make small, frequent commits with plain-English messages.
- Use `.github/pull_request_template.md` for pull requests.
- Never add `Co-authored-by`, `Generated with`, `Made-with`, `Claude-Session` or any other AI attribution line to a commit message or pull request description. When squash merging, delete any such lines GitHub adds to the merge message.

## Beginner quick start

Full guide: https://github.com/CivicAIClub/docs/blob/main/developer-onboarding.md

1. First time: check Git with `git --version`, set your Git name and GitHub email, accept the club invite, and sign in with GitHub Desktop or `gh auth login`. Clone only your project's repo, open its folder, and read its README setup steps.
2. Start each work session from the latest main, then make a branch:

```sh
git checkout main
git pull origin main
git checkout -b feature/short-description
# Make and check your changes before continuing.
git status
git add .
git commit -m "Describe your change"
git push --set-upstream origin feature/short-description
```

Use `feature/`, `fix/`, or `chore/` as appropriate, with lowercase names and hyphens. Commit small working pieces; do not edit or push main directly.
3. Open a PR on GitHub, fill in the template, and get someone else's approval and passing checks where CI exists. Push review fixes to the same branch. After it is merged, pull main again before starting another branch.
4. If stuck, ask in the case chat, then Keke, then Luke or Cayden. Ask before doing anything drastic.

## Sources

- `README.md`
- `.cursor/rules/civic-ai-workflow.mdc`
- `.cursor/rules/commit-messages.mdc`
- `.cursor/rules/ext-a-green-valley-hospitality.mdc`
- [Developer Onboarding Guide](https://github.com/CivicAIClub/docs/blob/main/developer-onboarding.md)
