# Talent pipeline — operating rules

This folder is Ubanthu Robotics' **private talent-scouting knowledge base**. Goal: build and maintain a ranked list of great people who could build NORM's **cleaning intelligence**: robot learning, manipulation, sim-to-real (see `ROLE.md`, v2 since 2026-11-24). People dump messy material here (LinkedIn screenshots, links, CVs, notes). Claude's job: **input → organise → assess → rank → keep documents current.**

The conversation is NOT the knowledge base. The files are.

**Owner:** Ruthwik (with Vishal, founder) · **Started:** 2026-11-21

## Files and folders

| Path | Purpose |
|---|---|
| `ROLE.md` | The role: must-haves, nice-to-haves, scorecard (how candidates are scored). Change only when the founders change the brief. |
| `CANDIDATES.md` | **Master list / hub.** One row per person: tier, score, current role, location, why, availability, status, link to profile. Keep it short. Change log at the bottom. |
| `profiles/<firstname-lastname>.md` | One file per person with more than a name: person card, evidence, scorecard, open questions, outreach notes. |
| `people/<firstname-lastname>.png` | Cropped profile photos (PIL), only when useful. |
| `screenshots/` | Original evidence (screenshots, LinkedIn PDFs, CVs, papers). **Always name files `<firstname-lastname>_<type>_<detail>.<ext>`** (e.g. `jane-doe_linkedin-export_2026-11.pdf`, `jane-doe_paper_<short-title>_arxiv-<id>.pdf`), using the same slug as the profile file. CVs with contact details get the suffix `_LOCAL-ONLY`. |
| `SOURCES.md` | Source register: `H001`, `H002`… (H = hiring, to avoid clashing with the competitor KB's S-IDs). |
| `SEARCH_LOG.md` | Where we have looked (labs, companies, events, repos, queries) and what came out, so searches aren't repeated. |
| `_inbox/` | Drop zone (files also often land in `people/` as `Profile (2).pdf`). After processing, rename by person and move to `screenshots/`. |

## Processing any new input

1. Identify the person(s). Check `CANDIDATES.md` for duplicates; merge, don't duplicate.
2. Extract **professional facts only**: current/previous roles, education, projects, papers, repos, talks, skills, location, public links.
3. Register the source in `SOURCES.md` (ID, what, URL/file, date of source, date added, who provided it).
4. Write/update the profile card (template below) and score against `ROLE.md`.
5. Update the row in `CANDIDATES.md` and add a change-log line.
6. Tag confidence: `[V]` verified/seen (repo, paper, video, profile) · `[CC]` self-claim (CV/LinkedIn/site) · `[3P]` third party · `[INF]` Claude's assessment · `[INT]` team opinion (name + date) · `[UNV]` rumour.
7. **Separate evidence from inference.** "Has a ROS 2 Nav2 repo with 40 commits" is evidence; "probably strong at navigation" is `[INF]`.

## Person card template

```markdown
# Jane Doe
<img src="../people/jane-doe.png" width="110">

| Field | Value |
|---|---|
| Current role | … (since …) |
| Location / willing to move | … |
| Education | … |
| Previous | … |
| Links | [LinkedIn](…) · [GitHub](…) · [Site](…) · [Scholar](…) |
| Sources | H00x … |

## Evidence by requirement
| Requirement (ROLE.md) | Evidence | Tag |
|---|---|---|

## Three-axis summary
| Axis | Result | Basis |
|---|---|---|
| Reputation | x/10 (A–D) | Edu · Employer · Signal |
| Can we get them? | High/Medium/Low/Very low | … |
| Technical (v2) | x/100, Tier … | score below |
| Contact priority | P1/P2/P3 | ROLE.md rule |

## Score
| Criterion | Weight | 0–5 | Why |
|---|---|---|---|
**Total:** x / 100 → Tier A/B/C/X (v2 weighted rubric in ROLE.md) · confidence High/Medium/Low

## Availability signals
## Concerns / gaps
## Outreach notes (who knows them, warm intro path, status)
## Open questions
```

## Tiers

Tier definitions and thresholds live in `ROLE.md` (v2, 2026-11-24): **A** ≥70 + gate (learned policy on a real robot) · **B** 50–69 · **C** <50 or junior · **X** not a fit (keep the row with a one-line reason, so we don't re-research them).

## Rules

- **Private folder.** Never push to the public competitor repo (`ruthwik-coder/Norm-competitors`). If this becomes a git repo, keep it private.
- **Professional information only.** No personal phone numbers, personal emails, home addresses, family, health, age, religion, salary history. If a CV contains contact details, keep the CV file local and do not copy those details into the notes.
- **Public sources only.** LinkedIn (as seen by us), GitHub, papers, personal sites, talks, press. No pretexting, no scraping behind logins, no using confidential competitor material (e.g. competitor investor decks) for outreach.
- **Don't send anything** (LinkedIn messages, emails) on anyone's behalf. Claude drafts; Ruthwik/Vishal send.
- **People already in the competitor KB** (`../competitors/`, e.g. Nolon, Origin, Hivebotics staff): competitor-related questions are answered in that KB. Here, keep only the **candidate view** (fit, score, availability) and link to their competitor-KB card instead of duplicating it.
- Every claim about a person needs a source ID. Never invent roles, degrees or skills. Mark unreadable things as "not visible".

## Answering questions

- Search `CANDIDATES.md`, `profiles/`, `SOURCES.md` first. Say what's missing and how to find it.
- When asked "who's best for X", answer from the scorecard and say how confident the evidence is.

## Style

Practical and direct. Dense over verbose. When material is dumped, process it — don't ask how to organise it.
