# Ballot Path Oregon

A free planning guide for people thinking about running for office in Oregon. Enter an address to see every office on your ballot, from precinct committeeperson to U.S. Senate. Pick one and get a dated, step-by-step plan covering eligibility, filing, campaign finance, the voters' pamphlet, campaigning, door knocking, and Election Day. The plan suggests a campaign mix for the office (door knocking, mail, radio, TV, party coordination, and more), and the candidate can add or drop any of it. For federal, statewide, and legislative seats it shows past results and a starting win number.

The **Learn** tab explains how Oregon elections work, defines the terms used in the plan (underlined terms in the plan link to these definitions), and offers fill-in templates filled with the candidate's race: a budget, a fundraising call sheet, contribution cards, volunteer sign-up sheets, a press release, a door script, a county contact list, and more, with Spanish versions of the pieces voters see.

The plan also covers legal checks first-time candidates miss (the federal Hatch Act, employer rules, ethics rules for new officials, complaints, recounts, and write-ins), researching opponents, answering attacks, and working with reporters. Each step shows a rough time estimate. A campaign team can share progress by saving a backup file and merging a teammate's file on the Sources tab.

It's a single web page with no server, accounts, or tracking. Everything a person enters (address, answers, checklist progress, voter files) stays in their own browser.

> **A planning aid, not legal advice.** Election rules change. The official sources have the final word: the filing officer and the current Secretary of State candidate manuals on getting on the ballot, the Elections Division on campaign finance and election law (the FEC for federal races), and the Oregon Government Ethics Commission on ethics.

## What's in this repository

| File | What it is |
|---|---|
| `index.html` | The whole app: page, styles, code, and most of the data |
| `addr/41001.json` … `addr/41071.json` | Street address ranges for each of Oregon's 36 counties, used to match an address to its districts and city. The app loads only the county it needs. |
| `.nojekyll` | Tells GitHub Pages to serve the files exactly as they are |
| `README.md` | This file |

## Put it online with GitHub Pages

1. On GitHub, click **+** (top right), then **New repository**. Name it (for example `ballot-path-oregon`), set it to **Public**, and click **Create repository**.
2. On the new repository's page, click **uploading an existing file**.
3. Drag in `index.html`, `README.md`, `.nojekyll`, and the whole `addr` folder. GitHub keeps the folder structure. Then click **Commit changes**.
   - On a Mac, `.nojekyll` may be hidden in Finder (press **Cmd + Shift + .** to show it). The site works without it; it just keeps GitHub from processing the files.
4. Go to **Settings**, then **Pages** in the left menu. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the **main** branch and the **/ (root)** folder, and click **Save**.
5. After a minute or two, the page shows your site's address, usually `https://YOUR-USERNAME.github.io/ballot-path-oregon/`.

To update the app later, upload the new `index.html` the same way. GitHub replaces the old one, and the site updates within a few minutes.

## Where the information comes from

The **Sources** tab in the app lists every source. In short:

- **Filing rules, fees, deadlines, and forms:** Oregon Secretary of State candidate manuals, ORS chapters 249, 254, 255, and 260, and city charters and candidate packets for 67 cities.
- **Campaign finance:** the Secretary of State's Campaign Finance Manual (rev. 01/2025) and the 2026 contribution-limit legislation page.
- **Voters' pamphlet:** the State Voters' Pamphlet Manual (rev. 08/2026) and the joint county pamphlet rules.
- **Contact lists:** League of Women Voters of Oregon local Leagues and the Oregon Newspaper Publishers Association member directory.
- **Federal and ethics rules:** the U.S. Office of Special Counsel's Hatch Act guidance, ORS chapters 244 (government ethics), 254 and 258 (write-ins and recounts), and 165.540 (recording conversations).
- **Past results:** OpenElections' Oregon files for the November 2022 and 2024 general elections and the May 2026 primary.
- **Districts and addresses:** 2024 Census TIGER/Line address ranges, ODOT city limits (processed September 2026), and the Oregon Blue Book for county offices.
- **School boards and conservation districts:** county election notices and the Oregon Department of Agriculture SWCD directory.
- **Campaign practice:** published field experiments (Gerber and Green; Kalla and Broockman; Green et al. on lawn signs), candidate surveys, and vendor pricing pages checked in October 2026.

Figures marked as estimates or rules of thumb in the app are labeled that way. Items marked **Verify** should be confirmed with the filing officer.

## Keeping it current

The most time-sensitive pieces are:

- Contribution limits that take effect January 1, 2027 (the state is still writing the rules)
- Candidate filing fees and deadlines for each election
- Vendor and tool prices
- City charter rules, which cities can change at any time

## Privacy

The app sends no data anywhere. Address matching runs in the browser against the files in `addr/`. Answers and progress are saved in the browser's local storage, and a voter file loaded on the Voters tab is stored in the browser's own database. Clearing site data removes all of it.
