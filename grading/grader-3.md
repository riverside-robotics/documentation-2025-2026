# Grader 3 Report

## Rubric Understanding

Rubric used: NRL Robot Project Portfolio Documentation Rubric (from `NRL Documentation Details.pdf`, pp. 5–6). Four top-level categories comprising **28 sub-criteria**, each scored 0–4 (0 = not covered, 4 = superior content). **Total possible: 112 points.** The supplementary page-1 "NRL Documentation Details" guide also mentions a 10-point portfolio award, but the actual detailed scoresheet is the 28-row rubric, which is what I scored against.

## Scores by Criterion

### Organization (4 criteria, 16 pts)

| Criterion | Score | Justification | Suggestion |
|---|---|---|---|
| Binder | 3/4 | Delivered as a single long `main.md` plus `main.pdf` (not a physical 3-ring binder). Cover at lines 1–28 is professional and complete. | Print/bind with tabs for each major section; rubric explicitly expects a 3-ring binder. |
| Sections Match Rubric | 2/4 | ToC (lines 73–113) covers most rubric items but **Promotional/Fundraising**, **Accounting/Budget** (as its own section), **Manufacturing Plans** (assembly procedure), and **Assembly Models** are not dedicated sections. | Add dedicated headings for Promotional/Fundraising, Accounting/Budget, Manufacturing Plans, Assembly Models. |
| Team & School Name and Members on Front | 4/4 | Cover (lines 1–27) lists team name, school, address, advisors, sponsors, and all 19 members. | — |
| Extra Organizational Functionality | 3/4 | ToC with anchor links (73–113), section-ownership table (493–516), cross-refs to `meetingNotes.md`, `todo.md`. Strong. | Add page numbers / per-section tabs for print; include a glossary/index. |

### Design Motivation/Strategy (4 criteria, 16 pts)

| Criterion | Score | Justification | Suggestion |
|---|---|---|---|
| Influences | 4/4 | Deep treatment of Spinlayden 1.0 strengths/weaknesses (263–310), problem→solution table (301–309), figures 1–3. | — |
| Offensive | 3/4 | Offensive Strategies bulleted (732–738) with quantified numbers (645.6 RPM, 78 J). | Add a dedicated paragraph on target prioritization / engagement sequencing vs. different opponent archetypes. |
| Defensive | 3/4 | Defensive Strategy (740–746) covers perimeter barrier, retreat, airflow, invertibility. | Explicitly call out "special armor" and maneuverability stats (turn radius, spin-up time). |
| Winning | 2/4 | Covered indirectly via Objectives table (358–362) and strategy bullets, but no dedicated "Winning" subsection weighing aggression vs. speed vs. damage per rubric. | Add an explicit "Winning" section ranking focus among aggression, speed, damage. |

### Team Procedures (6 criteria, 24 pts)

| Criterion | Score | Justification | Suggestion |
|---|---|---|---|
| Team Management | 2/4 | Assignments table (422–443), action plan (449–461), and reference to `meetingNotes.md` (485) — but no meeting minutes embedded in main.md (topics, attendance, decisions). | Embed a representative sample of meeting minutes directly in main.md, or include the full `meetingNotes.md` as an appendix. |
| Material Management | 3/4 | BOM at lines 532–564 with buyer/category/part/price/qty/total. Solid. | Add "where the part is used in the bot" column per rubric; include any purchase orders. |
| Accounting/Budget | 3/4 | Budget Summary table at 568–577 shows funding sources and totals ($4,199.66 / $2,456.05 new). | Include actual purchase orders / receipts (only receipt #87094381 is noted, 560). |
| Time Management | 4/4 | Key Milestones (400–407) plus excellent Planned-vs-Actual timeline (469–483) with slippage notes. | — |
| Data Management | 3/4 | GitHub + Fusion Hub + shared drive explained (703–712). | Screenshot the repo structure or Fusion version tree; tie to "easy to find items in binder" criterion. |
| Promotional/Fundraising | 0/4 | Not covered. Team shirt is mentioned in BOM (560) and shown (229) but no section on posters, fundraising events, dates, or funds raised. | Add a Promotional/Fundraising section documenting the shirt campaign, any posters, and fundraising dates/amounts. |

### Design Process (13 criteria, 52 pts)

| Criterion | Score | Justification | Suggestion |
|---|---|---|---|
| Research Methods | 2/4 | Brief "Research" (720–728), "Research Methods" (787) and "Analysis and Conceptualization" (766–775). Sparse — Research Methods is two sentences. | Expand with specific competitions reviewed, sources, brainstorm artifacts, and decision matrices. |
| CAD Models | 4/4 | Multiple renders (Figs 7, 8, 8b at 847–857) plus Spinlayden 1.0 renders for comparison. | — |
| Refinement | 4/4 | Refinement section (789–807) lists 8 concrete refinements tied to risk/testing. | — |
| Structural Analysis | 4/4 | Full FMEA table (831–841) with severity/likelihood/mitigation, plus pros/cons in 1.0 comparison. | — |
| Engineering Drawing Set | 4/4 | Three dimensioned drawings (Wall, Gearbox Mount, Bearing Mount) by Robby Rateno 3/3/2026, 1:1 Size B, Figs 9/10/11 (861–891). | — |
| Material Selection | 4/4 | Excellent Material Selection section (587–626) covering 6061, carbon steel, 1045, PLA/PETG/TPE with alternatives considered. | — |
| Manufacturing Plans | 1/4 | Fabrication section (628–676) shows photos and describes processes, but is **not** a step-by-step assembly procedure that someone could follow to rebuild the bot. | Add a numbered written assembly procedure with torque specs and part callouts. |
| Assembly Models | 2/4 | Some in-progress assembly photos (Figs 15, 15b, 16, 16b, 16c, 658–676) including PLA placeholder walls. | Add pre-build physical mockup / prototype photos and exploded-view CAD assembly renders. |
| Weapon System Details | 4/4 | Clear section (895–907) with quantity, material, mounting, energy output, tip speed; advantages/disadvantages addressed in Material Selection (613–614). | — |
| Drive System Details | 4/4 | Comprehensive (911–948) — motors, ESCs, gearboxes, wheels/hubs, IMU, shafts/bearings, power transmission, steering. Includes why chosen. | — |
| Power System Details | 3/4 | Batteries, safety, distribution (950–967). Well done but weaker on "why this choice over others." | Add alternatives considered (Li-ion, LiFePO4, higher-C packs) and rationale. |
| Wiring Schematic | 2/4 | Signal/power flow described textually (971–986) plus GPIO assignment image (Fig 14, 1001). No actual CAD/drawn electrical schematic. | Produce a proper schematic diagram (KiCad/Fritzing/hand-drawn) showing all connections. |
| Testing Results | 2/4 | Testing phases listed (1005–1027) but most results are "planned" — no quantitative data, no repeated trials, no scientific-method writeup. | Complete and document full-speed spin, impact, maneuverability, and runtime tests with quantified results before submission. |

## Total

**85 / 112 — B (≈76%)**

Strong content in design engineering areas (CAD, drawings, FMEA, material selection, drive system), but loses points on several required rubric sections that are missing or thin.

## Top 5 Things to Fix

1. **Add a Promotional/Fundraising section** (line ~525 area) — 0/4 currently; documenting the t-shirt sale and any posters/events recovers up to 4 points.
2. **Complete and publish quantitative Testing Results** before submission (line 1003) — replace "planned" bullets with measured RPM, impact data, runtime; rubric expects scientific-method repeated trials.
3. **Write a step-by-step Manufacturing/Assembly Procedure** — the rubric explicitly says "Someone assembling your bot for the SECOND time should be able to take this procedure and assemble the bot without help"; current Fabrication section (628+) is descriptive, not procedural.
4. **Produce a real Wiring Schematic diagram** — the text flow at 971–986 plus GPIO table is not a schematic; add a drawn/CAD schematic.
5. **Embed Team Management meeting minutes** in main.md (attendance, decisions, action items per rubric) rather than only pointing to `meetingNotes.md` — and add a dedicated "Winning" subsection explicitly ranking aggression/speed/damage focus.

## Strengths

- Exceptional cover page and team roster (1–27).
- Outstanding Influences section with concrete problem→solution mapping (301–309).
- Professional-grade FMEA and project risk matrix (815–841).
- Three proper dimensioned engineering drawings at 1:1 Size B (861–891).
- Thoughtful Material Selection with alternatives considered (587–626).
- Strong Planned-vs-Actual timeline showing mature project management (469–485).
- Clear named contributions throughout (Design Team, Robby Rateno, section-ownership table 493–516) — directly satisfies the "team members' names throughout" NRL guideline.
- Consistent, technically specific language (645.6 RPM, 78 J, 26.9 mph, Loc-Tite, 6061-T6, etc.).
