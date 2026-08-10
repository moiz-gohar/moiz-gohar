# Setup

Your GitHub profile README is served from the public repository whose name is exactly your username:

`moiz-gohar/moiz-gohar`

## 1. Replace README.md

Copy the included `README.md` into the root of that repository.

## 2. Add the workflows

Copy:

- `.github/workflows/snake.yml`
- `.github/workflows/metrics.yml`

Commit both files.

## 3. Add the Metrics token

The `lowlighter/metrics` workflow needs a GitHub personal access token.

Create a fine-grained/classic token with the least privileges required for the metrics you want, then add it to:

Repository → Settings → Secrets and variables → Actions → New repository secret

Name it:

`METRICS_TOKEN`

If you only want public information, keep permissions minimal. If you later want private contribution/repository information included, expand permissions deliberately.

## 4. Run Actions manually once

Open the repository's **Actions** tab and run:

- Generate contribution snake
- GitHub metrics

After successful runs:

- `github-metrics.svg` will exist in the profile repository.
- the `output` branch will contain the animated snake SVGs.

## 5. Improve the repositories behind the profile

The README is the presentation layer. To make the profile convincing, add/pin 3–6 public repositories that demonstrate:

1. a real AI product
2. a full-stack production build
3. computer vision or ML depth
4. automation / agents
5. a reusable engineering tool

For each flagship repo, add:
- a strong one-sentence value proposition
- architecture diagram
- screenshots/demo GIF
- stack
- local setup
- deployment notes
- key engineering decisions
- roadmap
