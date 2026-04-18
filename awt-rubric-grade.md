# AWT 2026 Rubric Grade — main.md

Graded against the official AWT references in `AWT Interview & Documentation References-20260414T232350Z-3-001/`:

- `Documentation Scoring 2026 (10-20-2025).xlsx` — the scoresheet
- `Documentation Sections 2026.docx` — the list of required sections
- `Documentation Details.pdf` — the narrative guidance on what "high marks" look like
- `Example Documentation — Final Blue Streak of Death 2023-2024.pdf` — exemplar reference

## Rubric Model (2026 AWT)

17 criteria, each scored 0–4 (0 = not covered, 4 = superior content). **Max = 68 points.**

| Section | Items | Max |
|---|---|---|
| Design Motivation/Strategy | Influences | 4 |
| Team Procedures | Team Management, Material Management/BOM, Accounting/Budget, Time Management | 16 |
| Design Process | Materials Selection, Research Methods, CAD Models, Structural Analysis, Engineering Drawing Set, Weapon System, Drive System, Power System, Wiring Schematic, Manufacturing Plans/Assembly, Testing Results, Design Refinement | 48 |
| **Total** | | **68** |

American letter-grade conversion:

| % | Letter |
|---|---|
| 93–100 | A |
| 90–92 | A- |
| 87–89 | B+ |
| 83–86 | B |
| 80–82 | B- |
| 77–79 | C+ |
| 73–76 | C |
| 70–72 | C- |
| 67–69 | D+ |
| 63–66 | D |
| 60–62 | D- |
| <60 | F |

---

## Scores by Criterion

### Design Motivation / Strategy

| # | Criterion | Score | Evidence in main.md | Notes |
|---|---|---|---|---|
| 1 | Influences | **4/4** | Lines 243–282. Strengths/weaknesses of 1.0 (Table 1), 7-row Problem→Solution table (Table 2), three CAD/photo figures of Spinlayden 1.0, and an explicit "What Was Changed" list. | Exemplary — every 2.0 design choice traces back to a concrete 1.0 failure. |

**Subtotal: 4 / 4**

### Team Procedures

| # | Criterion | Score | Evidence in main.md | Notes |
|---|---|---|---|---|
| 2 | Team Management (meeting minutes) | **4/4** | Table 6e (lines 457–487) — 28 meetings logged with date, phase, attendees, topics, and decisions. Action Plan in Table 6b (lines 413–425). | Fully addresses rubric items: date, attendees, topics, decisions, ongoing action list. |
| 3 | Material Management / Material Selection / BOM | **4/4** | Table 7 BOM (lines 534–568), Material Selection section (lines 591–630) with alternatives rejected for cause (7075, CF, Ti), 3D print materials (PLA/PETG/TPE) justified by use. | Full BOM + clear fabrication rationale. |
| 4 | Accounting / Budget | **3/4** | Table 8 Budget Summary by funding source (lines 574–581); BOM includes unit and total cost; PO 219831 referenced for Riverside portion; Receipt #87094381 referenced for shirts. | Loses one point — no scanned purchase orders/receipts embedded; only numbers referenced. |
| 5 | Time Management / Project Scheduling | **4/4** | Table 5 Key Milestones (lines 364–371), Table 6b Action Plan with leads/deadlines (lines 413–425), Table 6c Planned vs. Actual (lines 433–447) — including the March CNC overrun and how it was absorbed. | Mature PM artifacts; planned-vs-actual is above HS average. |

**Subtotal: 15 / 16**

### Design Process

| # | Criterion | Score | Evidence in main.md | Notes |
|---|---|---|---|---|
| 6 | Materials of Construction Selection | **4/4** | Full Material Selection section (lines 591–630). Chassis (6061-T6), bolts (1/2" carbon steel), shafts (1045), 3D print (PLA/PETG/TPE-83A). Each material has strength/weight/machinability/cost justification. Alternatives (7075, CF, Ti) explicitly rejected for cause. | Top-tier — matches "superior content" wording in rubric. |
| 7 | Research Methods | **3/4** | Research section (lines 739–754) names three sources — Spinlayden 1.0 baseline, AWT footage, OpenMelt — and lists four findings that shaped the design. One hand-drawn concept sketch (Figure 6). Research Methods subsection (lines 815–817) itself is only two sentences. | Loses a point — no decision matrix / trade-study table, no brainstorm artifacts (whiteboard photos), minimal "other designs considered". |
| 8 | CAD Models | **4/4** | Figures 7, 8, 8b (lines 877–887) — full isometric render, silver-finish iso, interior cutaway on the hex bottom plate; plus Spinlayden 1.0 comparison renders (Figs 1–2). | Multiple views, interior visible, comparison with prior-year platform. |
| 9 | Structural Analysis | **4/4** | Table 10 FMEA (lines 862–872) — 8 components × Failure Mode / Cause / Effect / Severity / Likelihood / Mitigation. Table 11 Project-Level Risk Matrix (lines 845–854) covers schedule, manufacturing, and competition risks. Pros/cons of 1.0 → 2.0 carried forward via Influences. | Formal FMEA is above HS norm. |
| 10 | Engineering Drawing Set | **4/4** | Four dimensioned CAD drawings — Wall Plate, Gearbox Mount, Bearing Mount (Figures 9a/10a/11a — Robby Rateno, 3/3/2026), and Top-Bottom Plate (Figure 11c — Adam Pakeltis, 4/18/2026) at 1:1 Size A/B. Each has author and date; PDF link for the top-bottom plate (line 933). | Includes motor/bolt specs in Drive/Weapon sections. Authorship throughout. |
| 11 | Weapon System Details | **3/4** | Weapon System (lines 935–949) — quantity, material, mounting (Loc-Tite + jam nut), KE, RPM, tip speed. Field replaceability called out. Advantages/disadvantages discussed in Material Selection (lines 617–618). | Loses one — rubric explicitly asks to "elaborate upon offensive/defensive/winning design strategies in this section." Strategy lives in its own section (732–772) and isn't repeated or cross-linked here. |
| 12 | Drive System Details | **4/4** | Drive System (lines 951–990) — motors, ESCs, gearboxes (with reduction), wheels/hubs, IMU (WT901 with figures 12, 12b), shafts/bearings, belt, steering. Each component has chosen part + why. | Complete and technically specific. |
| 13 | Power System Details | **3/4** | Power System (lines 992–1010) — 4× Liperior 3S 3200 mAh in parallel, MS-05 kill switch upstream, BEC wiring detail (left only to avoid paralleled regulators), wiring safety. | Loses one — rubric wants "choice over others." No comparison to Li-ion / LiFePO4 / higher-C packs or larger-capacity alternatives considered. |
| 14 | Wiring Schematic | **4/4** | Actual schematic diagram at `Images/wiring_schematic.png` (Figure 14b, line 1020). Full pin-by-pin GPIO table (lines 1039–1052). Pi boot-config overlays documented. Separate power path and signal path described; grounds explained. | Above rubric — includes both the drawn schematic AND narrative rationale (why two voltages, why four grounds). |
| 15 | Manufacturing Plans / Assembly Process | **3/4** | Assembly Process (lines 660–673) — 7 numbered steps with two parallel sub-assemblies called out. Backed by Figures 15–16c (photos of wiring-integration build with PLA placeholder walls). Fabrication sub-sections (lines 636–657) document waterjet, CNC, and FDM. | Loses one — no torque specs per fastener, no callout-numbered photos tied to each step, no explicit "ease / difficulty of (dis)assembly" statement. |
| 16 | Testing Results | **1/4** | Testing Results (lines 1094–1116) is mostly *planned* or *in progress*. Qualitative "verified," "confirmed." No measured RPM, no runtime minutes, no impact damage data, no repetitions. | Biggest single-criterion risk. Rubric requires scientific method, quantitative results, repeated trials across aggression / durability / maneuverability. Currently covered = 1 (covered but poorly). |
| 17 | Design Refinement | **4/4** | Refinement section (lines 821–837) — 8 concrete refinements (weight reduction, component repositioning, weapon redesign, Pi housing, Python→C#, Bluetooth→2.4 GHz, counterweight removal, 3D-printed prototyping). Each tied to a 1.0 failure mode or a risk-analysis finding. | Strong. |

**Subtotal: 41 / 48**

---

## Total

| Section | Score | Max |
|---|---|---|
| Design Motivation / Strategy | 4 | 4 |
| Team Procedures | 15 | 16 |
| Design Process | 41 | 48 |
| **Total** | **60** | **68** |

**Percentage: 88.2 %**

## Letter Grade: **B+**

Strong documentation with real engineering depth. Influences, FMEA, engineering drawings, material selection, time management, meeting minutes, and the wiring schematic are all at or near rubric ceiling. Points are lost almost entirely on **Testing Results** (the only 1/4) and on single-point gaps in Research Methods, Accounting/Budget, Weapon System strategy cross-link, Power System alternatives, and Manufacturing assembly detail. Nothing is categorically missing; everything flagged below is reachable before the 4/18 submission or — at worst — before the 4/25 judge interview.

---

## Strengths Worth Keeping

- Cover page (lines 1–27) — team name, school, full address, all 19 members, advisors, industry advisor, sponsors, event.
- Influences chain (lines 243–282) is exemplary — every 2.0 change traces to a specific 1.0 failure.
- Meeting Minutes (Table 6e) — 28 meetings × date/phase/attendees/topics/decisions — fully satisfies rubric inline.
- Full BOM + funding-source budget (Tables 7–8) with in-kind value tracked separately.
- Planned-vs-Actual timeline (Table 6c) with slippage noted — mature PM signal.
- FMEA + project-level risk matrix (Tables 10–11).
- Four dimensioned engineering drawings at 1:1 with author/date (Figures 9a, 10a, 11a, 11c).
- Wiring schematic drawing + pin-by-pin GPIO table + boot-config overlays.
- Named contributions throughout (Section Ownership table at lines 494–519, CAD credits, photo credits).
- Technically specific language consistently: 645.6 RPM, 78 J, 26.9 mph, Loc-Tite, 6061-T6, 1045, OMAX 5555, etc.

---

## TODO — What to Fix (ordered by point-recovery potential)

### High-impact (biggest score swing)

- [ ] **Testing Results (lines 1094–1116) — currently 1/4.** Execute and document quantitative tests before submission. Rubric explicitly requires scientific method, quantifiable results, and repeated trials. Add:
  - Measured RPM at full throttle (tachometer or gyro log) with at least 3 trials
  - Measured battery runtime from fresh charge to brownout (minutes), 3 trials
  - Impact test: bolt-head damage vs. a sacrificial target (photo + damage metric)
  - Maneuverability test: stop-to-stop drive time across a fixed distance in both wheel mode and melty mode, 3 trials each
  - Spin-up time: 0 → 645.6 RPM (seconds), 3 trials
  - If results land after the 4/18 PDF freeze, state "post-test addendum — see competition interview packet" and deliver at 4/25. The rubric rewards repeatability and numbers.

### Medium-impact (each of these is one point)

- [ ] **Research Methods (line 815) — currently 3/4.** The "Research Methods" subsection is two sentences. Expand with:
  - A concept sketches / brainstorm photo set (mention of whiteboarding exists at line 800 — show the photos)
  - A short "designs considered and rejected" trade-study table: alternatives like vertical spinner, wedge, drum — with a sentence on why meltybrain won
  - The specific AWT match footage reviewed (year, match, observations)
- [ ] **Accounting/Budget (lines 574–581) — currently 3/4.** Embed or reference scanned purchase orders / receipts (Riverside PO 219831, Custom Ink #87094381, parts orders). A screenshot appendix is fine.
- [ ] **Weapon System (lines 935–949) — currently 3/4.** Rubric says "elaborate upon offensive/defensive/winning design strategies in this section" for weapon, drive, and power. Either:
  - Drop a short "Offensive / Defensive / Winning" paragraph inside the Weapon System section, OR
  - Cross-link to the Strategy section with a one-line summary of how the weapon embodies each strategy.
- [ ] **Power System (lines 992–1010) — currently 3/4.** Add "alternatives considered" — e.g., Li-ion 18650 packs, LiFePO4, higher-C LiPo — and why 3S 3200 mAh LiPo won on C-rating × weight × kit availability.
- [ ] **Manufacturing Plans / Assembly Process (lines 660–673) — currently 3/4.** Add:
  - Torque spec per fastener class (#10-24 cap screws, 1/2"-13 impact bolts, gearbox-to-mount bolts)
  - Callout-numbered photos (1, 2, 3 …) keyed to the 7 assembly steps
  - One sentence per step on "ease/difficulty of (dis)assembly" — rubric names this explicitly

### Polish (not point-bearing but easy wins)

- [ ] Add page numbers / footer labels when exporting `main.pdf` — the AWT Sections doc recommends headers/footers on every page so judges know what they're reading.
- [ ] Add a brief "Promotional/Marketing" callout (team shirt photo at line 193 already in-doc; the shirt receipt and student reimbursement flow are also logged). Not scored in the 2026 xlsx rubric but recommended by Documentation Details guidance and common in the AWT example doc.
- [ ] Cross-link the Section Ownership table (494–519) from the main Table of Contents so judges can find attribution quickly.
- [ ] Confirm every figure is referenced by number in prose (spot-check a few — most already are).

### Verify before submission

- [ ] All image paths resolve when main.md is rendered to PDF (especially `Images/wiring_schematic.png`, `Images/Engineering Drawings/*`, and paths with spaces).
- [ ] Drawing PDF link at line 933 opens correctly from the exported PDF.
- [ ] Final weight re-measured and stated in Key Stats — current text says 13.5 lbs base, 15 lbs target. If competition ballast is installed before 4/18, update the number.
- [ ] The "That's a Wrap!" closing (line 1120) stays last; no dangling TODOs after it.

---

*Grade issued 2026-04-18 against AWT 2026 Scoring Sheet (DD/DLC 10/20/2025).*
