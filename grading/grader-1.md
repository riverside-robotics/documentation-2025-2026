# Grader 1 Report

## Rubric Understanding

Primary rubric: the NRL "Robot Project Portfolio Documentation Rubric" (pp. 5-6 of `NRL Documentation Details.pdf`). It lists **23 criteria** in four category groups (Organization, Design Motivation/Strategy, Team Procedures, Design Process), each scored 0-4. **Total possible = 92 points.** I also cross-referenced the NRL Documentation Details narrative (pp. 2-4) for what "superior content" looks like in each row. I treated `main.md` alone as the submission (scoresheet xlsx not opened — proceeding with the PDF rubric, which is identical in criteria).

## Scores by Criterion

### Organization (16 pts)
| # | Criterion | Score | Justification | Fix |
|---|---|---|---|---|
| 1 | Binder | 3/4 | Well-structured markdown with clear hierarchy, TOC (L71-113), figure numbering; but it's a single MD file, not the "3-ring binder" the rubric expects. | Export `main.pdf` with tabbed/labeled sections, or explicitly call out binder organization. |
| 2 | Sections Match Rubric | 3/4 | Most rubric items are addressed; headings mostly aligned. Missing: no "Promotional/Fundraising", no "Manufacturing Plans" or "Assembly Models" headings; "Team Management" not present as a labeled section. | Add the missing section headings verbatim from rubric. |
| 3 | Team & School Name / Members on Front | 4/4 | Cover (L1-27) has team, school, address, full roster, advisors, sponsors, AWT event. | — |
| 4 | Extra Organizational Functionality | 4/4 | TOC with anchors (L71), numbered tables/figures, Documentation Section Ownership table (L492-517), action plan, time management planned-vs-actual. | — |

### Design Motivation / Strategy (16 pts)
| # | Criterion | Score | Justification | Fix |
|---|---|---|---|---|
| 5 | Influences | 4/4 | Strong "Influences" section (L279-318) with two detailed tables comparing 1.0 strengths/weaknesses and problem→solution pairs. | — |
| 6 | Offensive | 4/4 | Explicit "Offensive Strategies" list (L732-738) with quantitative specs (645.6 RPM, 78 J, tip speed). | — |
| 7 | Defensive | 3/4 | "Defensive Strategy" (L740-746) covers spin shield, retreat, invertibility. Missing: explicit "special armor" discussion. | Add a brief "armor" subsection or call out 3/8" 6061-T6 walls as armor. |
| 8 | Winning | 3/4 | Objectives table (L356-362) and strategy sections imply winning focus (aggression, damage). Not a labeled "Winning" section. | Add a dedicated "Winning" subheading that states the primary judged-aspect focus. |

### Team Procedures (24 pts)
| # | Criterion | Score | Justification | Fix |
|---|---|---|---|---|
| 9 | Team Management | 1/4 | No meeting-minutes tables in `main.md`; only a reference at L515 that minutes live in `meetingNotes.md`. Rubric explicitly wants minutes (topics, attendance, date, decisions, actions). | Import or summarize meeting minutes into `main.md` with date/attendance/decisions/actions columns. |
| 10 | Material Management | 4/4 | Full BOM (L532-564) with buyer, category, qty, unit price, total. | — |
| 11 | Accounting/Budget | 4/4 | Budget Summary by funding source (L570-577) plus detailed BOM; includes in-kind, PO#, student reimbursements. | — |
| 12 | Time Management | 4/4 | Key Milestones (L400-407) + Planned vs. Actual season timeline (L471-483) with slippage noted. | — |
| 13 | Data Management | 3/4 | Data Management section (L699-712) describes GitHub, Fusion 360 hub, shared drive. Adequate but brief; no screenshots of folder structure. | Add a screenshot or a file-tree of the repo / drive to show it's easy to navigate. |
| 14 | Promotional/Fundraising | 0/4 | No promotional posters documented and no fundraising events described (only a t-shirt line item in the BOM). | Add a Promotional/Fundraising subsection with posters, recruitment flyers, and any fundraising events (date, amount, method). |

### Design Process (36 pts)
| # | Criterion | Score | Justification | Fix |
|---|---|---|---|---|
| 15 | Research Methods | 2/4 | "Research Methods" (L785-787) is a 2-sentence paragraph. Brainstorming/whiteboard work mentioned but not shown. | Include whiteboard photos, alternatives-considered table, and brainstorm outputs. |
| 16 | CAD Models | 4/4 | Multiple labeled CAD renders (Figures 7, 8, 8b at L847-857) of full assembly, plus interior view. | — |
| 17 | Refinement | 4/4 | Refinement section (L789-807) lists seven concrete refinements tied to 1.0 failures. | — |
| 18 | Structural Analysis | 4/4 | Formal FMEA table (L832-841) with severity, likelihood, cause, effect, mitigation. | — |
| 19 | Engineering Drawing Set | 4/4 | Three dimensioned drawings (Wall, Gearbox Mount, Bearing Mount) with CAD + drawing pairs (L859-891), 1:1 Size B, dated, authored. | — |
| 20 | Material Selection | 4/4 | Detailed Material Selection section (L587-626) with alternatives considered (7075, carbon fiber, titanium) and quantitative justification. | — |
| 21 | Manufacturing Plans | 1/4 | Fabrication section (L628-676) describes processes and shows assembly photos, but there is no step-by-step written assembly procedure ("someone assembling for the SECOND time could do it unaided"). | Write a numbered assembly procedure with callout photos per step. |
| 22 | Assembly Models | 2/4 | Assembly photos with PLA placeholder walls (Figures 15-16c) partially fulfill this; no pre-build mockups or prototype models explicitly shown as design iterations. | Add photos of the 3D-printed prototype wall sections (referenced at L807) with captions explaining what was learned. |
| 23 | Weapon System Details | 3/4 | Clear weapon description (L893-907) with quantities, energy, RPM. Light on explicit disadvantages/trade-offs. | Add a pros/cons subsection for the hex-bolt weapon choice. |
| 24 | Drive System Details | 4/4 | Detailed drive spec (L909-948): motors, ESCs, gearboxes, IMU, shafts/bearings, transmission. | — |
| 25 | Power System Details | 3/4 | Power System (L950-967) covers batteries, safety, distribution. Does not justify "why this choice over others." | Add alternatives considered (e.g., other battery chemistries/capacities) and rationale. |
| 26 | Wiring Schematic | 3/4 | Narrative power/control paths (L969-1001) plus GPIO pinout figure. No single dedicated schematic drawing. | Produce a proper wiring diagram (e.g., in Fritzing/KiCad) showing all connections on one sheet. |
| 27 | Testing Results | 1/4 | Testing Results (L1003-1027) is almost entirely planned or in-progress — no quantitative aggression/durability/maneuverability results, no repetition. | Run and document quantitative tests (energy output, drive-speed timing, impact-target results) with raw numbers before submission. |

## Total

**79 / 92 — B+ (86%)**

Strong, professional documentation with real technical depth; loses points primarily on rubric items that are either missing outright (Promotional/Fundraising, Manufacturing Plans, Team Management minutes in-doc) or that are still pending at the time of writing (Testing Results).

## Top 5 Things to Fix

1. **Testing Results (L1003-1027)** — biggest single-criterion risk. Execute the planned April 14-24 tests and paste quantitative results (RPM measured, runtime, bolt-hit target damage) before submission.
2. **Promotional/Fundraising (missing)** — add a whole subsection with posters, t-shirt campaign details, and any fundraising events.
3. **Team Management / Meeting Minutes (L515 only)** — pull the minutes from `meetingNotes.md` into `main.md` (or include them as an appendix table) so judges don't have to hunt.
4. **Manufacturing Plans (missing)** — write a numbered, photo-backed assembly procedure a stranger could follow.
5. **Wiring Schematic (L969)** — replace the bullet-list description with a real single-sheet electrical schematic diagram.

## Strengths

- Cover page (L1-27) and team/partner biographies are polished and complete.
- Influences and 1.0→2.0 problem/solution tables (L285-309) are exemplary.
- BOM, budget summary, and season timeline (L532-577, L467-483) are industry-quality.
- Dimensioned engineering drawings with authorship and date (L861, 879, 889) are above what most HS teams submit.
- FMEA and project-level risk matrix (L815-841) show mature engineering discipline.
- Consistent attribution of individual contributions throughout (Section Ownership table L492-517; figure captions credit Mechanical/Software/Design teams).
