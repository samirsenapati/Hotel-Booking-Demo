# Hotel-Booking-Demo

## Hotel Booking

**Hotel Booking** is a dummy SaaS project used to demonstrate automated documentation workflows with GitHub Actions and OpenAI.

This repository shows how to:

1. Trigger a workflow on every new git tag (`v*`) pushed to the repo.
2. Use OpenAI GPT-4 to generate release notes from commit messages.
3. Commit those notes to `docs/` in a new branch.
4. Open an automated Pull Request for human review.

## Prerequisites

* A GitHub repository (this one or your fork).
* An `OPENAI_API_KEY` saved under **Settings > Secrets and variables > Actions**.

Once the secret is in place, tag any commit (e.g. `git tag v0.1.0 && git push origin v0.1.0`) and watch the workflow create AI-generated release notes for **Hotel Booking**!
