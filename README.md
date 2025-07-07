# Hotel Booking Demo

**Hotel Booking** is a dummy SaaS project used to demonstrate GitHub Actions automation
with OpenAI for automated release‑note generation.

## What’s included

* **GitHub Actions workflow** in `.github/workflows/ai-release-notes.yml`
  – triggers on every tag (`v*`), gathers the last 10 commit messages,
  calls GPT‑4 to create release notes, and opens a pull request.
* **docs/** – placeholder folder where the release notes markdown file
  will be created or updated by the workflow.
* **README.md** – this file.

## Quick start

1. Create a new GitHub repo (public or private).
2. Add a repository secret called `OPENAI_API_KEY` with your actual key.
3. Clone the repo locally and unzip this package into the repo folder.
4. Commit and push to `main`:
   ```bash
   git add .
   git commit -m "Initial commit – Hotel Booking demo with AI workflow"
   git push origin main
   ```
5. Tag a release and push the tag:
   ```bash
   git tag v0.1.0
   git push origin v0.1.0
   ```
   GitHub Actions will run and create a pull request with AI‑generated
   release notes in `docs/RELEASE_NOTES.md`.

That's it – merge the PR and your first AI‑powered release notes are live!
