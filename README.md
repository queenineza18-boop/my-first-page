# my-first-page

One HTML file, built in one Freebuff session on 18 November 2026. No framework, no build step, no dependencies. It opens in any browser straight from disk.

Live repo: https://github.com/queenineza18-boop/my-first-page

## What's in here

`index.html` is the whole page. CSS sits in one `<style>` block at the top, with colours as variables (`--accent` is the button). Nine lines of JavaScript at the bottom bump a counter on click.

## Run it

Double-click `index.html`.

Add anything that loads data later (`fetch()`, ES modules) and a `file://` URL will block it under same-origin rules. Then you need a server:

    python -m http.server 8000

Python 3 is on this machine; Node.js and npm are not (`node -v` fails, no `C:\Program Files\nodejs`), so the repo deliberately avoids npm tooling.

## Edit it

- Change the `<h1>` text: that's HTML.
- Change `--accent: #7c9cff;` to `#ff8a5c`: one variable drives the badge and the button.
- Add `<li>` items inside the `<ul>`: the list is markup, nothing to register.

Save and reload. No compile step.

## Git

The folder tracks `origin/main`, with `user.name` and `user.email` set locally (Queen Ineza / queenineza18@gmail.com) so other projects keep their own.

    git clone https://github.com/queenineza18-boop/my-first-page.git
    git log --oneline

History: `59c77c2` from GitHub, `a4fe42f` for the page.

Pushes go through the bundled credential manager (`git config --get credential.helper` says `manager`). No credential is cached on this machine yet, so your first `git push` opens a browser sign-in. Keep personal access tokens out of this repo: public repo, public token.

## Using Freebuff

Freebuff is a coding agent from Freebuff, Inc., the team behind Codebuff. It runs on your machine, edits files in the folder you open, and runs commands there. This repo came out of the desktop app; a CLI exists too (`npm install -g freebuff`, then `freebuff` in a project) and needs Node first.

Advertisers pay for it. Ads are labelled "Sponsored", and sponsored suggestions need an Accept click. Free use is counted in hours: sessions run about an hour with unlimited messages, and the daily allowance depends on your country. Paid plans start at $8/month. Figures from freebuff.com/plans, November 2026.

What it looked like here: "I'm a beginner trying Freebuff" produced the file and a live preview. "Push this on my GitHub" created a public repo and committed to it. Two messages, no commands typed by hand.

Prompts that get somewhere: "Change the heading to my name and add a section about what I'm studying." "Explain this file line by line, then I'll ask for changes." "Add a second page and link to it." Vague requests like "make it better" cost an extra round trip and free hours.

Two habits: read the diff before accepting a change, because the agent can edit any file in the folder. And push when something works rather than at the end.
