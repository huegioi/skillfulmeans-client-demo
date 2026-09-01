# SkillfulMeans Client Demo

The presenter screen used on SkillfulMeans prospect calls: the Canva deck,
then a walkthrough of the platform, then next steps. 27 steps, about 27
minutes for a full run.

**Live:** https://huegioi.github.io/skillfulmeans-client-demo/

## What's in here

A single self-contained file.

- `index.html` — the entire demo. All CSS, JavaScript and images are inline;
  there is no build step, no dependencies and nothing to install.

## Hosting

GitHub Pages serves `index.html` from the root of `main`. Every push to
`main` rebuilds the site, which takes about a minute.

## Updating it

The source of truth is the Claude artifact copy, not this repo. To publish a
new version:

1. Export the current demo from the artifact.
2. Replace `index.html` with it.
3. Commit and push to `main`.
4. Wait about a minute, then load the live URL with a hard reload
   (Cmd+Shift+R) — a normal reload often serves the cached previous version
   and makes a good deploy look like a failed one.

The full procedure, including the presenter notes and the rules about which
"Open live" buttons are safe to show on a call, lives in the project doc
`claude/client-demo-flow.md`.

## A note on visibility

This repo is public and the demo file contains the presenter notes —
objection handling, positioning, tier pricing. No client data is in it, but
it is the sales playbook. Treat the URL accordingly.
