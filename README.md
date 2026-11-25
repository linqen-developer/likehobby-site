# LikeHobby Sudoku

[Play Sudoku](https://www.likehobby.com/sudoku.html).

This repository previously hosted hobby recommendation and demo account/subdomain pages. Those pages, their stylesheet, old social image and Google Tag Manager loader have been removed from the current branch.

## Hosting

The current Sudoku application runs on Vercel and is maintained separately in the operator's verified release workspace. This cleanup does not publish that operational source, credentials or saved player data to this repository.

The small `likehobby-site/vercel.json` disables Git-triggered deployments so a cleanup commit cannot replace the working Vercel release. It is a guard for this retired source tree, not an application build. Continue releasing production from the verified operational workspace.

The root `_config.yml` excludes `likehobby-site` and this README from GitHub Pages. Root `index.html` and `404.html` forward visitors to canonical Sudoku without loading tracking code. Forwarding is restricted to this GitHub Pages project's hostname/path, keeps valid QA markers and standard UTM parameters, and ignores user-supplied redirect destinations. The old nested addresses still initially return HTTP 404; the browser then navigates to Sudoku. With JavaScript disabled, use the visible link. These are static forwarding pages, not HTTP 301/308 rules or an account-wide Pages disable.

The current Sudoku assets, licenses, domain verification records, analytics and collector infrastructure remain in their existing operational locations.

## Repository history

The cleanup is a normal forward commit. Earlier commits remain available in Git history; the cleanup does not claim to erase previous commits, clones or external caches. The local pre-cleanup clone and release receipts remain available to the operator for rollback and audit.
