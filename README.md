# Reading list

A curated, prioritized queue of papers I want to read.

**Zotero is the storage warehouse.** This repo is the **active queue** — what to actually read next, sorted by priority and category. Every entry links back to its Zotero item so the metadata only lives in one place.

## How it works

Papers live in category files under [`papers/`](papers/). Inside each file they're grouped by priority:

| Priority | Meaning                                  |
|----------|------------------------------------------|
| **P1**   | Read soon (this week or next)            |
| **P2**   | Read eventually (this semester / project-relevant) |
| **P3**   | On the radar; maybe skim                 |

### Entry format

    - [ ] **Author+Year** — *Title* — one-line why it matters — [arXiv](URL) · [Zotero](zotero://select/library/items/KEY)

Tick the box `[x]` when you've read it. GitHub renders markdown checkboxes, so each file doubles as a visual checklist.

## Categories

- [Gravitational waves](papers/gravitational-waves.md)
- [Cosmology](papers/cosmology.md)
- [High redshift](papers/high-redshift.md)
- [Image reconstruction project](papers/image-reconstruction.md)
- [WFSS project](papers/wfss.md)
- [Human–AI collaboration](papers/human-ai-collaboration.md)

To add a category, copy one of the files above, clear the entries, and add a link here.

## Conventions

- **One sentence on *why* per entry.** If you can't say why you want to read it, you probably don't.
- **Zotero links** use the `zotero://select/library/items/<KEY>` URI. In Zotero: right-click an item → *Copy Item Link* (or the "Better BibTeX" plugin exposes the same thing).
- **When you've read it**, either check the box in place (cheapest, keeps history) or move to the `## Done` section at the bottom of the file.
- **Don't duplicate Zotero metadata** (abstracts, BibTeX, PDFs). This repo is a *queue*, not a second library.

## Deploy to GitHub

This is a plain git repo. To publish:

    cd /Users/zuo/Documents/reading-list
    git init
    git add .
    git commit -m "Initial reading list scaffold"

    # Option A: GitHub CLI (one-shot)
    gh repo create reading-list --public --source=. --remote=origin --push

    # Option B: existing empty repo
    git remote add origin git@github.com:<your-user>/reading-list.git
    git branch -M main
    git push -u origin main

Once it's on GitHub, every checkbox and every link just works in the web UI.
