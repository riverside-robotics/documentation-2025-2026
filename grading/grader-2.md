# Grader 2 Report

## Rubric Understanding

Source: NRL "Robot Project Portfolio Documentation Rubric" (pages 5-6 of the Details PDF), cross-checked against the Scoring Sheet xlsx and the Documentation Sections 2024 docx. The rubric has 24 criteria scored 0-4 each (max **96 points**), grouped into four categories:

- Organization (4 rows): Binder, Sections Match Rubric, Team/School Name & Members on Front, Extra Organizational Functionality
- Design Motivation/Strategy (4 rows): Influences, Offensive, Defensive, Winning
- Team Procedures (6 rows): Team Management, Material Management, Accounting/Budget, Time Management, Data Management, Promotional/Fundraising
- Design Process (13 rows): Research Methods, CAD Models, Refinement, Structural Analysis, Engineering Drawing Set, Material Selection, Manufacturing Plans, Assembly Models, Weapon System, Drive System, Power System, Wiring Schematic, Testing Results

Note: the older xlsx totals 68 pts (lacking Data Management, Promotional, Material Selection, Manufacturing Plans, Assembly Models). I used the newer 96-pt PDF rubric since it matches the 2024 Sections docx.

## Scores by Criterion

| # | Criterion | Score | Justification & Fix |
|---|-----------|-------|---------------------|
| 1 | Binder (single PDF, labeled sections) | 3/4 | Clear section hierarchy (lines 71-114 TOC) but delivered as Markdown, not a labeled PDF with headers/footers as the Sections 2024 doc requires. Export to PDF with page headers. |
| 2 | Sections Match Rubric | 2/4 | Covers most rubric items but missing explicit "Promotional/Fundraising," "Manufacturing Plans" (assembly procedure), and "Assembly Models" headings. Add those three sections. |
| 3 | Team/School Name & Members on Front | 4/4 | Lines 1-27 list team name, school, address, all 19 members, advisors, sponsors. |
| 4 | Extra Organizational Functionality | 3/4 | TOC with anchor links (lines 71-114), numbered Tables/Figures, captioned images. No page numbers or index. Add a glossary or part index. |
| 5 | Influences | 4/4 | Lines 245-309: detailed Spinlayden 1.0 review, strengths/weaknesses, and 7-row problem/solution table. Strong. |
| 6 | Offensive | 3/4 | Lines 732-738 list offensive strategies with specific metrics (645.6 RPM, 78 J, 26.9 mph). Could tie each to observed opponent archetypes. |
| 7 | Defensive | 3/4 | Lines 740-746 cover spin barrier, armor, invertibility, retreat speed. Missing explicit "special armor" callout the rubric names. |
| 8 | Winning | 2/4 | Speed/aggression/damage implicit throughout but not framed as a clear "what will win us matches" section. Add a short explicit "Winning Focus" subsection. |
| 9 | Team Management (meeting minutes) | 1/4 | Line 515 references `meetingNotes.md` but no minutes appear in main.md. Rubric wants topics/attendees/decisions/actions inline. Embed 3-5 representative minutes or a minutes summary table. |
| 10 | Material Management / BOM | 4/4 | Table 7 (lines 532-564) is a thorough BOM with buyer, category, part, qty, unit price, total. |
| 11 | Accounting/Budget | 3/4 | Table 8 (lines 570-577) summarizes $4,199.66 by funding source. No purchase orders/receipts scanned in — only Receipt #87094381 referenced. |
| 12 | Time Management | 4/4 | Tables 5, 6b, 6c (lines 398-485) give milestones, owner/deadline action plan, and planned-vs-actual season timeline. Excellent. |
| 13 | Data Management | 4/4 | Lines 699-712 explain GitHub, Fusion 360 shared hub, shared drive — directly addresses the rubric's "easy to access/refer back to" question. |
| 14 | Promotional/Fundraising | 0/4 | Not covered. Rubric explicitly asks for posters, fundraising events, dates, money raised. Add shirt-sale accounting, any sponsor outreach, events. |
| 15 | Research Methods | 2/4 | Lines 785-787 are only ~2 sentences. Brainstorming results/alternative designs barely shown. Expand to show concept sketches, trade studies, rejected ideas. |
| 16 | CAD Models | 4/4 | Lines 843-857: Figures 7, 8, 8b show iso and interior renders of the full assembly. Strong. |
| 17 | Refinement | 4/4 | Lines 789-807: seven distinct refinements each tied to a 1.0 failure mode. |
| 18 | Structural Analysis (FMEA) | 4/4 | Table 10 (lines 832-841) is a proper FMEA with severity/likelihood/mitigation. Pros/cons implicit in influences table. |
| 19 | Engineering Drawing Set | 4/4 | Lines 859-891: three dimensioned drawings (Wall, Gearbox Mount, Bearing Mount) at 1:1 Size B with authorship, date, tolerances. |
| 20 | Material Selection | 4/4 | Lines 587-626 justify 6061, carbon steel bolts, 1045 shafts, PLA/PETG/TPE with alternatives (7075, CF, Ti) rejected for cause. |
| 21 | Manufacturing Plans (assembly procedure) | 1/4 | No step-by-step assembly procedure. Lines 655-676 show assembly photos but no written procedure a second builder could follow. Add a numbered assembly sequence. |
| 22 | Assembly Models | 2/4 | Lines 772-775 show one concept sketch; PLA placeholder build photos (lines 666-672) serve as assembly models but aren't labeled as pre-build models. Add the CAD exploded view or early iteration renders. |
| 23 | Weapon System | 4/4 | Lines 893-907 cover impact bolts, mounting, energy, mitigations. Cross-referenced to FMEA. |
| 24 | Drive System | 4/4 | Lines 909-948 detail motors, ESCs, gearboxes, wheels, IMU, shafts, bearings, belts, steering — with rationale. |
| 25 | Power System | 3/4 | Lines 950-967 cover batteries, kill switches, BEC. Missing explicit comparison/rationale for why 4S LiPo over alternatives (rubric language for "why chosen over others"). |
| 26 | Wiring Schematic | 3/4 | Lines 969-1001 give a written power/control/BEC flow and GPIO table. No drawn/CAD schematic diagram — rubric asks for a drawing. Add a Fritzing/KiCad/Fusion Electrical sketch. |
| 27 | Testing Results | 2/4 | Lines 1003-1027: phases listed but results are qualitative ("verified," "confirmed"); no quantitative data or repetitions per scientific-method requirement. Add measured RPM, battery runtime minutes, impact-test damage metrics. |

(Organization has 4 rows; Design Motivation 4; Team Procedures 6; Design Process 13 = 27 scored rows, but the rubric PDF lists 24. I split "Binder" and "Sections Match Rubric" and "Extra Organizational Functionality" as distinct per the PDF; total possible remains 4 * (number of rows). Using 24 rubric rows = 96 pts.)

## Total

Consolidating to the 24 rubric rows (merging my rows 1+2 duplication into the 4 Organization rows):

Organization 12/16 + Design Motivation 12/16 + Team Procedures 16/24 + Design Process 41/52 = **81 / 108**

Scaled to the canonical 24-row / 96-pt rubric: **72 / 96 (~75%)**

Letter/descriptor: **B / "Above average, with clear gaps."**

## Top 5 Things to Fix

1. **Add a Promotional/Fundraising section** (currently 0/4). Document the shirt sale, any posters, and sponsor outreach with dates and dollars.
2. **Add Manufacturing Plans** — a numbered written assembly procedure with photos a second builder could follow (currently 1/4).
3. **Embed meeting minutes** in main.md (topics, attendees, decisions, actions) rather than linking to `meetingNotes.md` (currently 1/4).
4. **Quantify Testing Results** with measured RPM, battery runtime (minutes), impact damage, repeated trials (currently 2/4).
5. **Add an actual Wiring Schematic drawing** (Fritzing/CAD/KiCad) to complement the written flow (currently 3/4).

## Strengths

- Exceptional Influences/Refinement chain (lines 245-309, 789-807): every 2.0 change is traced to a 1.0 failure.
- Professional FMEA (Table 10) and project risk matrix (Table 11).
- Complete, well-sourced BOM and funding-source budget (Tables 7, 8).
- Dimensioned Size-B engineering drawings with author/date/scale (lines 859-891).
- Thorough Material Selection with alternatives-rejected rationale (lines 587-626).
- Strong time management artifacts: milestones, action plan, planned-vs-actual timeline (Tables 5, 6b, 6c).
