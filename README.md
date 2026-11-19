# Reviewer candidate finder

One web page for handling editors of the journal Delirium. It searches PubMed for people who have recently published on a topic and lists up to 20 reviewer candidates.

Live page: https://amaclullich.github.io/reviewer-finder/

## How it works

- The whole tool is one file, `index.html`. There is no server, no database and no login.
- The editor picks MeSH topic terms. The page sends them to PubMed from the editor's own browser.
- The page contacts two US National Library of Medicine services and nothing else. It stores nothing.
- No manuscript content goes in. The page accepts MeSH terms and up to two short runs of exact words, such as the name of a tool or a drug.
- The editor can choose a study design, choose first or last authors, shortlist people and copy or download the shortlist.
- The journal badge is stored inside the file, so the page loads nothing from other sites.

## How to change it

Replace `index.html` with a new version. GitHub publishes the change within a few minutes.

The settings are at the top of the script in `index.html`: the journal line, the minimum number of papers (50) and the list size (20).

## Upkeep

Run one search every six months to confirm that PubMed's services still answer.
