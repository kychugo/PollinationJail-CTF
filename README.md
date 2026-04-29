# PollinationJail - CTF Challenge
 - Author: Gameboy612
 - Category: Misc
 - Difficulty: Easy

## Description
WolframAlpha is a powerful computational engine, but it has a lot of limitations... I recently found out Pollinations AI has been giving away free LLM API calls! Why not just make a WolframAlpha clone using Pollinations? It can even execute Python code! Why did no one think of this before?

There are two flags to this challenge, and they are both in the format `pollin{...}`.

## Play Online (GitHub Pages)

A static demo is hosted on GitHub Pages — no Docker required:

| Page | URL |
|------|-----|
| 🏠 Landing / Flag Submission | `https://<user>.github.io/PollinationJail-CTF/` |
| 🎯 Challenge Interface | `https://<user>.github.io/PollinationJail-CTF/chal.html` |
| 📖 Solution / Writeup | `https://<user>.github.io/PollinationJail-CTF/solution.html` |

> **Note:** The GitHub Pages version calls the Pollinations AI API directly from your browser and displays the raw LLM response. Python code execution is server-side only; for the full challenge experience run locally with Docker (see below).

## Local Setup (Full Challenge)
1. Clone the repository and navigate to the project directory.

2. Build and run the Docker container using Docker Compose:

```bash
docker-compose up --build
```

3. Access the application in your web browser at `http://localhost:5000`.

## GitHub Pages Deployment

The `docs/` folder is automatically deployed to GitHub Pages via the included workflow (`.github/workflows/pages.yml`). To enable it:

1. Go to **Settings → Pages** in your GitHub repository.
2. Set **Source** to `GitHub Actions`.
3. Push to `main` — the workflow will deploy the static site automatically.