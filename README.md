# Equation Lab (interactive)

**Live page:** https://claude.ai/artifact/T4bbGVW1LrmNtniPeC4FFn
**Source file:** `claude/equation-lab-interactive.html` (single self-contained page; open in any browser)
**Time:** about 5 to 8 minutes per station, 17 stations, roughly two class periods. Use one grade card for a shorter run.

Based on the 17 equations in Ian Stewart's *In Pursuit of the Unknown*. Each station: hook, one playable experiment, one check question, one open "Think about it" prompt (notes saved in the student's own browser), and a teacher note (toggle at top right).

## Layout (v4, multi-page like the Memory and Neurochemical labs)
- **Main page:** hero with garden progress, the Standards Match key, and four large grade cards in a 2x2 grid (7th, 8th, Secondary Math I, Secondary Math II), plus a link to the Lab notebook.
- **Grade pages** (`#g7`, `#g8`, `#s1`, `#s2`): one section per grade. Stations are large cards grouped under colored Standards Match pills (Direct fit, Good connection, Stretch, Pure enrichment), ranked by fit to THAT grade's Utah Core standards. A station can appear in more than one grade.
- **Station pages** (for example `#g7-eq-7`): one station per page. Order: big number and title, one-line hook, the equation in plain words, Standards Match list, Play, Check, Think about it with notes, teacher note, then Back / Main page / Next.
- **Navigation:** the left rail (a top bar on phones) always shows a "Main page" button and the four grade sections with progress; the open grade expands to list its stations. Every subpage also has a "Main page" button in the breadcrumb at the top and in the pager at the bottom. Old `#eq-N` links still work.

| Grade | Ranked stations (d = direct, l = connection, f = enrichment) |
|---|---|
| 7th | d: 7 Normal distribution, 14 Schrödinger, 12 Second law, 10 Navier-Stokes, 11 Maxwell. l: 17 Black-Scholes, 15 Information, 4 Gravity. f: 6 Euler |
| 8th | d: 1 Pythagoras, 13 E = mc², 2 Logarithms, 5 i, 11 Maxwell. l: 3 Calculus, 8 Wave, 16 Chaos. f: 9 Fourier |
| Secondary I | d: 2 Logarithms (doubling, F.LE.1-3). l: 16 Chaos (F.IF.3, F.BF.2), 5 i (rotations, G.CO.2, 4-5), 1 Pythagoras (G.GPE.7) |
| Secondary II | d: 5 i (N.CN.1-2). l: 1 Pythagoras (G.SRT.8) |

Placement notes: logarithms (F.LE.4), periodic functions (F.TF) and normal-distribution fitting (S.ID.4) are Secondary Math III, so those stations are placed in lower grades and noted in the standards map. Secondary codes were checked against the Utah high school standards document. Utah is reviewing a revised P-12 math draft (fall 2026), so verify on uen.org.

The full code-by-station table is in the teacher-only Google Doc "Equation Lab: Standards Map (Teacher)": https://docs.google.com/document/d/19_PUe9HG-Hy2mkpAVF9TYVaY6_zJE8Vv7UqNSuHSgx4/edit. The text copy in `claude/equation-lab-standards-map.md` is the current version; the Google Doc still shows the earlier three-group layout until it is refreshed.

## Notebook Google Doc
Near the top of the page script is `const NOTES_DOC='';`. Paste your Google Doc link (or just the ID) there. Students then get a link ending in `/copy`, which forces them to make their own copy. Set the doc to "Anyone with the link can view" first or the copy link will not work. Until it is filled in, students see a "link will appear here" message and the Teacher notes toggle shows a reminder. Template text to paste into the doc is in `claude/equation-lab-notebook-template.md`.

## Teacher notes
- Honest simplifications: Navier-Stokes station shows only the continuity consequence (area x speed constant); Maxwell voltage model uses made-up units; Schrödinger uses the 1D particle-in-a-box; Black-Scholes is the one-step "average payout" toy version, not investment advice.
- Progress and notes live in the student's browser only (localStorage). "Copy my notebook" at the bottom gathers all notes.
- Animations respect reduced-motion (start paused with a Play button).
- Answer keys and discussion prompts are in the Teacher notes toggle (students can switch it on, so use it for projection or print the page separately if that matters).

## Sources
- Stewart, I. (2012). *In Pursuit of the Unknown: 17 Equations That Changed the World.*
- UEN Online Core Resource, Mathematics Grade 7, Grade 8, Secondary I-III: https://www.uen.org/core/math/
- Clay Mathematics Institute, Navier-Stokes Millennium Prize problem.


## Layout update (multi-page, matches the Memory and Neurochemical labs)
- **Main page:** hero with garden progress, the Standards Match key, and four large grade cards in a 2x2 grid (7th, 8th, Secondary Math I, Secondary Math II), plus a link to the Lab notebook.
- **Grade pages** (`#g7`, `#g8`, `#s1`, `#s2`): one section per grade. Stations are listed as large cards grouped under the Standards Match pills (Direct fit, Good connection, Stretch, Pure enrichment).
- **Station pages** (for example `#g7-eq-7`): one station per page, in this order: big number and title, one-line hook, the equation in plain words, Standards Match list, Play, Check, Think about it with notes, teacher note, Back / Main page / Next.
- **Navigation:** the left rail (top bar on phones) always shows a "Main page" button and the four grade sections with progress; the open grade expands to list its stations. Every subpage also has a "Main page" button in the breadcrumb at the top and in the pager at the bottom.
- Old `#eq-N` links still work. The Google Doc standards map is unchanged and still needs a refresh.
