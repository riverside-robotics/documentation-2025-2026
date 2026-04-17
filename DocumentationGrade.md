# Spinlayden 2.0 Documentation — Grade Report

Graded against the AWT RoboBots 2026 Documentation Scoring Rubric (`Documentation Scoring 2026 (10-20-2025).xlsx`) and the required-sections list (`Documentation Sections 2026.docx`). Evaluation date: 2026-04-17 (1 day before the Apr 18 11:59 PM submission deadline).

---

## Overall Grade

# **C−**

**Raw score: 49 / 68 points (72.1%)**

**One-line summary.** The engineering content (materials selection, FMEA, CAD, drive system, influences) is honest, original, and competition-ready; the score is dragged down primarily by **Testing Results** (deferred to a post-test addendum, which the rubric treats as "covered poorly"), a **Wiring Schematic** that is text + pinout rather than an actual drawn schematic, **Meeting Minutes** that don't follow the official template, and several "covered but not in the rubric-required format" gaps. Fixing the three High-severity items below would move this to a solid **B / B+** before submission.

---

## 1. Rubric Scorecard

Scoring scale: **0** not covered · **1** poorly · **2** adequate · **3** above average · **4** superior.

### Design Motivation / Strategy (4 pts)

| # | Sub-criterion | Max | Awarded | Rationale | Evidence |
|---|---|---|---|---|---|
| 1 | Influences | 4 | **4** | Detailed Spinlayden 1.0 analysis, Table 1 pos/neg, Table 2 problem→solution map, "What Changed" bullets, full history of the previous bot. Clearly tied to team's own prior work. | `main.md:227-301` |

**Subtotal: 4 / 4**

### Team Procedures (16 pts)

| # | Sub-criterion | Max | Awarded | Rationale | Evidence |
|---|---|---|---|---|---|
| 2 | Team Management (meeting minutes) | 4 | **2** | 28 meetings logged Sep 24 → Apr 14 with dates/attendees/notes/decisions, but **does not follow the official Meeting Minute Template** — no explicit *Action Items* with Responsibility + Estimated Completion Date + Status columns, no scribe attribution, and four late-season entries (Mar 17, Mar 31, Apr 3, Apr 11) have an empty **Notes** field. | `meetingNotes.md:414, 433, 450, 491` |
| 3 | Material Management / BoM | 4 | **3** | Full 31-row Bill of Materials by buyer, category, unit price, quantity, total cost. Fabrication methods named. Missing: copies of purchase orders; an explicit "what we fabricated and why" list (material-by-material fab rationale is present but not called out as such). | `main.md:511-545, 610-658` |
| 4 | Accounting / Budget | 4 | **2** | Funding-source totals present (Riverside, Advisors, Team owned, AWT), but no per-line expense log, **no purchase-order summary**, and promotional-material expenses (team shirts) aren't separately called out as promo spend. | `main.md:549-557` |
| 5 | Time Management / Project Scheduling | 4 | **3** | Action Plan (Table 6b) with Lead/Supporting/Deadline and a planned-vs-actual phase timeline (Table 6c) that even documents the March CNC overrun. Good but **not in the official Project Plan template column set** (Item · Priority · Group · Action · Responsibility · Initiation Date · Due Date · Completion Date · Status · Comments). | `main.md:430-466` |

**Subtotal: 10 / 16**

### Design Process (48 pts)

| # | Sub-criterion | Max | Awarded | Rationale | Evidence |
|---|---|---|---|---|---|
| 6 | Materials of Construction Selection | 4 | **4** | Each material justified on strength, weight, machinability, cost, corrosion. Explicit alternatives rejected: 7075 / Carbon Fiber / Titanium for chassis; AR500 / Tool Steel / Hardened SS for blades. | `main.md:567-609` |
| 7 | Research Methods | 4 | **2** | "Research Methods" subsection is literally two sentences. Brainstorm results not documented as results (only that whiteboarding happened). Better content lives in Analysis & Conceptualization but isn't labelled as research results. | `main.md:767-769, 744-757` |
| 8 | CAD Models | 4 | **4** | Three full-assembly renders (isometric, silver, interior-with-top-removed) plus Fusion 360 shared-hub workflow described. | `main.md:825-839` |
| 9 | Structural Analysis | 4 | **4** | FMEA (Table 10, 8 failure modes with severity/likelihood/mitigation) **plus** a separate project-level Risk Matrix (Table 11, 8 risks). Offensive/defensive strategies listed separately. | `main.md:791-823, 714-728` |
| 10 | Engineering Drawing Set & Models | 4 | **3** | Dimensioned drawings for Wall, Gearbox Mount, Bearing Mount at 1:1, Size B, each authored and dated by Robby Rateno on 3/3/2026. Motor / screw / bearing specs captured in BoM. **Missing dimensioned drawings for the top/bottom hex plates and the A516 blade** — all three are fabricated parts. | `main.md:841-873` |
| 11 | Weapon System Details | 4 | **3** | Quantified: 6 blades, 6.33 oz each, A516 Grade 70, spike geometry, ~78 J/rotation, 645.6 RPM, ~26.9 mph tip speed, interlocking + Loc-Tite mounting. Minimal explicit **disadvantages** of the full-body spinner choice (e.g., controllability trade-off, self-damage on impact). | `main.md:875-891` |
| 12 | Drive System Details | 4 | **4** | Motors, ESCs, gearboxes, wheels, hubs, IMU, shafts, bearings, belts, steering strategy, and rationale for meltybrain drive all covered with part numbers and ratings. | `main.md:893-932` |
| 13 | Power System Details | 4 | **3** | Batteries, voltage, connector, capacity, symmetric placement for balance, kill switches, BEC path. **No explicit "alternatives considered" section** (e.g., 6S vs 4S, Li-ion vs LiPo, single pack vs parallel). | `main.md:934-951` |
| 14 | Wiring Schematic | 4 | **2** | Power/Control/BEC signal flow is described as a numbered text path, and a GPIO pin assignment table + Pi4J pinout reference are included. **But the rubric specifically asks for "a drawing of electrical wiring (CAD or other software)"** — no block/ladder schematic exists. Fig 13c is pulled from pi4j.com, not drawn by the team. | `main.md:953-985` |
| 15 | Manufacturing Plans / Assembly Process | 4 | **2** | Fabrication methods (waterjet, CNC, 3D print) are described and five build-progression photos (Figs 15–16c) are captioned well. **There is no numbered written assembly procedure** ("Step 1 … Step 2 …") and no explicit commentary on ease/difficulty of assembly and disassembly, both of which the rubric requires. | `main.md:610-658` |
| 16 | Testing Results | 4 | **1** | Low-power spin test stated qualitatively only ("verified software reads gyro"). Assembly/integration tests are listed but not quantified. **Full-speed, impact, maneuverability, and battery-runtime tests are explicitly deferred to a "post-test addendum"** — the rubric requires quantifiable, repeatable, documented testing results *in* the documentation. This is the single biggest point loss. | `main.md:987-1011` |
| 17 | Design Refinement | 4 | **3** | Eight refinements listed, each naming the 1.0 issue and the 2.0 fix (weight reduction, component repositioning, blade geometry, Pi housing, Python→C#, controller, counterweight removal, 3D-printed prototyping). Refinements **aren't explicitly cross-referenced back to FMEA rows or test trials**, which the rubric language asks for ("from risk analysis and/or testing"). | `main.md:771-789` |

**Subtotal: 35 / 48**

### Grand Total

| Section | Score |
|---|---|
| Design Motivation / Strategy | 4 / 4 |
| Team Procedures | 10 / 16 |
| Design Process | 35 / 48 |
| **TOTAL** | **49 / 68 (72.1%)** |
| **Letter Grade** | **C−** |

---

## 2. Issues Table — Everything That Isn't Good

Severity key: **H**igh (≥2 pts at risk) · **M**edium (1–2 pts at risk) · **L**ow (<1 pt at risk or presentation-only).

| # | Issue | Rubric Category | Location | Severity | Pts at Risk |
|---|---|---|---|---|---|
| 1 | Full-speed spin / impact / maneuverability / battery-runtime tests deferred to post-test addendum. Rubric requires quantifiable, repeated, documented results **in** the documentation. | Testing Results (#16) | `main.md:1005-1011` | **H** | 3 |
| 2 | No wiring schematic drawing. Text flow + GPIO pin table + third-party pinout are not a schematic. | Wiring Schematic (#14) | `main.md:953-985` | **H** | 2 |
| 3 | No numbered written assembly procedure. Photos tell what was built but not how to assemble it step-by-step. No ease-of-assembly commentary. | Manufacturing Plans (#15) | `main.md:610-658` | **H** | 2 |
| 4 | Meeting minutes do not follow official template. Missing Action Items with Responsibility / Estimated Completion / Status columns; no scribe attribution. | Team Management (#2) | `meetingNotes.md` (all entries) | **H** | 2 |
| 5 | Four late-season meeting entries (Mar 17, Mar 31, Apr 3, Apr 11) have an empty **Notes** field — only the task table is filled. | Team Management (#2) | `meetingNotes.md:414, 433, 450, 491` | M | rolled into #4 |
| 6 | Meeting note contradicts main doc: Jan 14 entry says "Selected carbon fiber" but `main.md` material selection is 6061 aluminum (carbon fiber explicitly rejected). Creates a broken decision trail. | Team Management (#2) / Materials Selection (#6) | `meetingNotes.md:274` vs `main.md:582` | M | 1 |
| 7 | Budget has funding-source totals but no purchase-order summary and no itemized expense log tying specific POs to line items. | Accounting / Budget (#4) | `main.md:549-557` | **H** | 2 |
| 8 | Project plan columns don't match the official Project Plan template (Item · Priority · Group · Action · Responsibility · Initiation Date · Due Date · Completion Date · Status · Comments). | Time Management (#5) | `main.md:430-466` | M | 1 |
| 9 | BoM has prices and totals but no copies or references to actual purchase orders, and fabricated-parts list isn't explicitly called out with "we fabricated X because Y" rationale. | Material Management / BoM (#3) | `main.md:511-545` | M | 1 |
| 10 | Research Methods subsection is two sentences. Brainstorming results not documented. | Research Methods (#7) | `main.md:767-769` | **H** | 2 |
| 11 | Engineering drawing set covers only Wall, Gearbox Mount, Bearing Mount. Missing dimensioned drawings for top/bottom hex plates and A516 blade — all fabricated parts. | Engineering Drawing Set (#10) | `main.md:841-873` | M | 1 |
| 12 | Weapon System narrative lacks explicit **disadvantages** of the full-body spinner choice. | Weapon System (#11) | `main.md:875-891` | L | 1 |
| 13 | Power System narrative lacks an "alternatives considered" section (4S vs 6S, LiPo vs Li-ion, single vs parallel packs). | Power System (#13) | `main.md:934-951` | L | 1 |
| 14 | Design Refinements aren't cross-referenced back to specific FMEA rows or test trials that drove them. | Design Refinement (#17) | `main.md:771-789` | M | 1 |
| 15 | 8 team-member biographies marked "Remaining team member bios will be added as they are submitted" — unfinished content visible to judges. | Presentation (all rubric rows) | `main.md:189` | M | 1 (cross-cut) |
| 16 | Team photo is a placeholder SVG labeled "(photo pending)". | Presentation | `main.md:9-11` | L | <1 |
| 17 | Deliverables checklist at the top of Project Overview has every box **unchecked** (`[ ]`), including deliverables that are clearly done. | Presentation / Time Management | `main.md:369-375` | L | <1 |
| 18 | Submission format — the rubric expects a single PDF. Current documentation is Markdown with no PDF export pipeline in the repo. Not a rubric deduction by itself, but a failed submission would zero the whole thing. | Submission format | repo root | **H** | 0 (process risk) |

---

## 3. Fix Instructions

Each fix is an instruction the team can execute without further investigation. Items are grouped by rubric category and ordered roughly by points recoverable. **You asked me not to make these edits — that's intentional; these are for the team to do.**

### Highest-impact fixes (worth 9 points combined; moves C− → B+)

#### Fix A — Testing Results (Issue #1, +3 pts)

1. Between now and the Apr 18 deadline, run as many of the rubric-required tests as physically possible: **aggression**, **durability**, **maneuverability**. These three words come straight from the rubric and judges look for them by name.
2. For each test, record in the doc:
   - **Setup** — what hardware, what power level, what arena/surface.
   - **Procedure** — numbered steps so the test is reproducible.
   - **Trials** — at least **3 trials per test** (the rubric calls out "multiple tests run to ensure repeatability").
   - **Quantitative result** — numbers, not adjectives. Examples: *spin-up time from 0 to 645.6 RPM (seconds)*, *measured tip speed (mph via high-speed video frame count or gyro log)*, *translational speed while spinning (ft/s, measured across a taped line)*, *impact count to visible deformation on a 1/4" plywood target*, *turn radius at full spin (inches)*, *battery runtime to 20% remaining voltage (minutes on a full pack)*.
   - **Pass/Fail vs. target** — state the target *before* the trial ("Target: >3 min runtime on one pack") so pass/fail is unambiguous.
3. If a test genuinely cannot be run by Apr 18 (e.g., arena-level impact test), **still** report: the low-power spin-test results that *have* been run with actual numbers (what RPM, what gyro drift measured, what latency from controller input to motor response). Replace `main.md:996-998` qualitative bullets with quantitative ones.
4. Delete the line "*Full-speed spin results, impact-test outcomes, and measured runtime will be compiled into a post-test addendum*" (`main.md:1011`) and put whatever numbers you have *in the doc*, even if partial. Judges cannot score a future addendum.
5. **Acceptance test:** every one of {aggression, durability, maneuverability} has at least 3 trials with numeric results against a pre-stated target.

#### Fix B — Wiring Schematic drawing (Issue #2, +2 pts)

1. Produce an actual wiring schematic. Options from lowest to highest effort:
   - Draw it in **Fritzing** (free, easy — your team already uses a Pi).
   - Draw it in **KiCad** (also free; looks more professional).
   - Draw it by hand on paper with a ruler, photograph cleanly, and caption it as a hand-drawn schematic.
2. Required nodes: 6× LiPo packs → paralleled bus → 2× MS-05 kill switches → 2× EZRUN MAX10 ESCs → 2× EZRUN 3660 motors; ESC BEC → Pi 4B + USB radio receiver; Pi UART → WT901 IMU; Pi GPIO → ESC signal wires (with pin numbers).
3. Embed as a new figure in the **Wiring Schematic** subsection. Keep the existing text flow and pinout table — the schematic is additive, not replacement.
4. **Acceptance test:** a technician who has never seen the bot could wire it up from the schematic alone.

#### Fix C — Manufacturing Plans / Assembly Procedure (Issue #3, +2 pts)

1. Add a new subsection under Fabrication titled **Assembly Procedure** containing a numbered step-by-step list — write it while physically assembling or disassembling the bot one time, so the steps reflect what actually happens. Example step skeleton (each step gets a photo if possible):
   1. Bolt the four BaneBots P61 gearboxes to the 6061 bottom plate using #10-24 × 3/8" hex socket button-heads with Loc-Tite (torque to X in-lb).
   2. Install 1045 drive shafts into R8-2RS bearings in the bearing mounts …
   3. Seat the symmetric 6× LiPo pack array in the PLA battery bracket, dressing XT60 leads toward the ESC side of the chassis …
   4. … (continue through motor wiring, kill-switch routing, Pi/IMU housing install, blade bolt pattern with Loc-Tite, top-plate capture, final kill-switch test).
2. Add a paragraph on **ease/difficulty of assembly/disassembly**: which steps are fastest, which are the pain points (e.g., seating the WT901 under the Pi), and what the team would change next season. The rubric explicitly asks for this.
3. **Acceptance test:** a Documentation teammate who did not build the bot can follow the procedure to take it apart and reassemble it without asking a Mechanical teammate.

#### Fix D — Meeting Minutes template (Issues #4, #5, #6, +2 pts)

1. Add these columns to every meeting's task table (rename/extend the existing "Tasks and Goals | Decisions" table):
   **Action · Responsibility · Estimated Completion Date · Status**
   The official Meeting Minute Template specifies exactly these columns.
2. Add a **Scribe:** line under each meeting header naming who took the minutes.
3. Fill in the four blank **Notes** fields: Mar 17 (`meetingNotes.md:414`), Mar 31 (`:433`), Apr 3 (`:450`), Apr 11 (`:491`). Even 1–2 sentences per meeting is a huge improvement over blank.
4. Resolve the Jan 14 "Selected carbon fiber" contradiction (`meetingNotes.md:274`): edit that entry to reflect what *actually* happened — either the carbon-fiber selection was later reversed (add a follow-up decision noting the reversal and why), or the note is wrong and should be corrected to the actual material decided that day. Do not leave a decision trail that conflicts with `main.md`.
5. **Acceptance test:** every meeting has Attendees, Topics (Notes), Decisions, and a task table with all four template columns filled.

#### Fix E — Budget / PO summary (Issue #7, +2 pts)

1. Add a new sub-subsection under **Team Procedures → Material Management** titled **Purchase Order Summary**. Include a table with columns: **PO # · Vendor · Line Items · Total Cost · Funding Source · PO Date · Status**.
2. If the team has receipts/POs in email or shared drive, list the PO numbers (or order confirmation numbers). If POs don't exist as formal documents, at minimum list every order with vendor, date, order number from the confirmation email, and total.
3. Break out promotional-material expenses (the Vistaprint team shirts at $239.09) as a separate budget line — the rubric explicitly calls out "include all material purchases and promotional material expenses".
4. **Acceptance test:** a finance auditor could reconcile every dollar in Table 8 back to a listed PO or order.

### Medium-impact fixes (worth 5 points combined; moves B+ → A−)

#### Fix F — Research Methods section (Issue #10, +2 pts)

1. Rewrite `main.md:767-769`. Two sentences is not enough. Include:
   - Competitions/streams actually watched (list specific event names, bots, years).
   - For each whiteboarded design alternative: name it, describe the idea in one line, and state why it was rejected or accepted. Turn whiteboarded results into a table.
   - At minimum 3–5 design alternatives considered (drum spinner, vertical disk, wedge, horizontal bar, meltybrain — whichever were actually discussed).
2. **Acceptance test:** a reader can answer "what other robot designs did the team seriously consider this season, and why did they land on a meltybrain?" directly from this subsection.

#### Fix G — Project Plan template format (Issue #8, +1 pt)

1. Keep Tables 6b and 6c. Add a third table formatted per the official **Project Plan template** with columns: **Item · Priority · Group · Action · Responsibility · Initiation Date · Due Date · Completion Date · Status · Comments**.
2. Populate it from the existing Action Plan + Season Timeline data — this is formatting work, not new content.
3. **Acceptance test:** the new table has all ten template column names as written in the `.docx` template, and every action has all ten fields filled.

#### Fix H — BoM fabricated-parts rationale (Issue #9, +1 pt)

1. Immediately after Table 7, add a short **Fabricated vs. Purchased** subsection listing each fabricated part (hex top plate, hex bottom plate, perimeter walls ×6, bearing mount, gearbox mount, blades ×6, 3D-printed battery bracket, 3D-printed Pi/IMU housing) with one sentence on *why* it was fabricated rather than purchased (no commercial equivalent, weight budget, custom geometry, etc.).
2. Reference or embed copies of ordering confirmations if available for POs.
3. **Acceptance test:** the reader sees, at a glance, which parts were made vs. bought and the reason for each fabricated part.

#### Fix I — Engineering Drawing completeness (Issue #11, +1 pt)

1. Add dimensioned drawings for the remaining fabricated parts: **top hex plate**, **bottom hex plate** (waterjet-cut), and the **A516 blade**. Use the same 1:1, Size B format as the existing three.
2. **Acceptance test:** every fabricated part has a dimensioned drawing in the Engineering Drawing Set section.

#### Fix J — Design Refinement cross-references (Issue #14, +1 pt)

1. For each of the 8 refinement bullets in `main.md:773-789`, append a parenthetical pointer like "(addresses FMEA row: *Side Walls — Deformation inward*)" or "(validated via 3D-printed prototype fitment test, Feb–Mar 2026)".
2. **Acceptance test:** every refinement cites either a specific FMEA row or a specific test that motivated the change.

### Low-impact fixes (worth ~3 points combined; polish to full A)

#### Fix K — Weapon System disadvantages (Issue #12, +1 pt)

Add a **Disadvantages** bullet list to the Weapon System subsection: controllability trade-off during spin-up, self-damage potential on hard impacts, wheel exposure during rotation, startup-window vulnerability. Rubric asks for "description of the weapon with advantages **and possible disadvantages**".

#### Fix L — Power System alternatives considered (Issue #13, +1 pt)

Mirror the format used in Material Selection (Fix style of "Alternatives considered"): add 4S vs 6S LiPo, LiPo vs Li-ion, single pack vs parallel 6-pack, each with a 1-sentence rejection rationale.

#### Fix M — Presentation polish (Issues #15, #16, #17)

1. **Bios (#15):** fill in the missing 8 bios or remove the "will be added as they are submitted" line. A visible unfinished line costs presentation points on every rubric row. At minimum replace the line with the list of missing-bio names or delete it.
2. **Team photo (#16):** swap the placeholder SVG for a real group photo. Even a casual photo is better than "(photo pending)" at the top of the cover.
3. **Deliverables checklist (#17):** `main.md:369-375` has every checkbox unchecked. Check off the ones that are clearly done (sponsor info, robot design spec, design ideas, manufacturing procedure) or remove the checklist if it's not being maintained.

### Process risk — Fix N (Issue #18, 0 rubric pts but potentially fatal)

The rubric expects submission as a single PDF. If no PDF is submitted on Apr 18, the score doesn't matter. Export `main.md` to PDF before the deadline:

- **Easiest:** `pandoc main.md -o Spinlayden_2.0_Documentation.pdf --pdf-engine=xelatex --toc` (requires pandoc + TeX Live or MiKTeX).
- **Alternative:** open `main.md` in VS Code with the Markdown-PDF extension, "Export (pdf)".
- **Fallback:** render `main.md` to HTML (e.g., with `grip` or GitHub's preview), open in a browser, Ctrl-P → Save as PDF.

Whatever tool is used, verify: (a) every embedded image actually renders, (b) tables don't overflow the page, (c) the TOC links work, (d) `meetingNotes.md` is either appended to the same PDF or submitted as a clearly-named second PDF. **Acceptance test:** print-preview the PDF end-to-end before submission and make sure no figures are clipped.

---

## 4. If You Only Fix Three Things

Deadline is ~30 hours away as of this grade. If there is no time for everything, fix these three first — they move the grade from **C−** to solidly into **B** territory for ≈5 hours of work total:

1. **Fix A — Testing Results.** Run at least one real durability trial, one real maneuverability trial, and one battery-runtime trial tonight/tomorrow and put the *numbers* in `main.md`. Even partial quantitative results score vastly higher than a deferred-addendum note. (+3 pts)
2. **Fix D — Meeting Minutes template.** Add the four missing template columns to the task table, fill the four blank Notes fields, fix the carbon-fiber contradiction. Pure formatting + small edits. (+2 pts)
3. **Fix N — PDF export.** Non-optional. Do it last, verify render quality, submit. (0 pts but eliminates submission-format risk.)

---

## Appendix A — Rubric Source

All scoring in this report derives from:

| Source | Contents | File |
|---|---|---|
| AWT RoboBots 2026 Documentation Scoring Rubric | 17 sub-criteria across 3 sections, each scored 0–4; max 68 pts | `AWT Interview & Documentation References-20260414T232350Z-3-001/AWT Interview & Documentation References/Documentation Scoring 2026 (10-20-2025).xlsx` |
| Documentation Sections 2026 | Required section list and hierarchy | `AWT Interview & Documentation References-20260414T232350Z-3-001/AWT Interview & Documentation References/Documentation Sections 2026.docx` |
| Documentation Details | High-level judging criteria: professional presentation, original writing specific to the team's current robot, team-member contribution attribution, clearly labelled drawings/specs, correct technical terminology | `AWT Interview & Documentation References-20260414T232350Z-3-001/AWT Interview & Documentation References/Documentation Details.pdf` |
| Meeting Minute Template | Required fields: Date · Attendees · Topics Covered · Decisions · Action (Action / Responsibility / Estimated Completion Date / Status) | `AWT Interview & Documentation References-20260414T232350Z-3-001/AWT Interview & Documentation References/Meeting Minute Template.docx` |
| Project Plan Template | Required columns: Item · Priority · Group · Action · Responsibility · Initiation Date · Due Date · Completion Date · Status · Comments | `AWT Interview & Documentation References-20260414T232350Z-3-001/AWT Interview & Documentation References/Project Plan template.docx` |
| Example Documentation (reference only, not scored) | 2023–2024 Blue Streak of Death documentation and 2025 Spinlayden documentation (Riverside Robotics) as exemplars | `AWT Interview & Documentation References-.../Example Documentation- Final Blue Streak of Death Documentation 2023-2024.pdf`, `Copy of Spinlayden 2025 _ Documentation _ Riverside Robotics.pdf` |

## Appendix B — Letter-Grade Scale Used

| Percentage | Letter |
|---|---|
| 93–100% | A |
| 90–92% | A− |
| 87–89% | B+ |
| 83–86% | B |
| 80–82% | B− |
| 77–79% | C+ |
| 73–76% | C |
| **70–72%** | **C−** ← this report |
| 67–69% | D+ |
| 63–66% | D |
| 60–62% | D− |
| <60% | F |

Standard US high-school letter-grade scale. At 72.1%, Spinlayden 2.0 is 0.9 points below a C (which would require 73% / 49.64 / 50 pts). Fix A alone (+3 pts) crosses into B territory.
