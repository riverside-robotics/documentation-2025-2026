# Documentation Fixes — 4-18-26

Consolidated list of everything `main.md` still needs before submission, pulled from the three independent grader reports in `grading/` (scores: 79/92, 72/96, 85/112 — consensus ~B, ~79%).

All three graders agreed on the same five gaps. Ordered by point impact.

---

## 1. Testing Results — highest impact

Currently written as "planned." Needs measured numbers.

Collect and paste into the Testing Results section:

- [ ] **Full-speed RPM** — tip / chassis RPM at full throttle (tachometer, high-speed-video frame count, or ESC telemetry)
- [ ] **Runtime** — minutes on a full battery pack at spin-up / idle
- [ ] **Impact test** — weapon bolt strike on a test target; note damage to target and any bot-side failures
- [ ] **Drive test** — translate-while-spinning meltybrain behavior; note drift or control issues
- [ ] **Date** each test was run and **who** ran it
- [ ] Photos or frame grabs of each test

Video of any test run is enough — I can pull frame-count RPM from it.

---

## 2. Promotional / Fundraising section — missing entirely

Add a new section under Project Overview. Cover:

- [ ] Team shirts / apparel (already in the BOM as a line item — call it out here as promo spend)
- [ ] Any social-media presence (Instagram, TikTok, etc.) or demo-day appearances
- [ ] Sponsor outreach: how Monode / Arc Technology / Show Studio were approached
- [ ] Fundraising totals and how funds were used
- [ ] Photos of the team in shirts or at an event

---

## 3. Manufacturing Plans / Assembly Procedure — missing

Add a step-by-step assembly procedure section. Cover:

- [ ] Order of assembly (chassis walls → gearbox mounts → motors → bearings → top plate → electronics)
- [ ] Tools required at each step
- [ ] Torque specs for the impact-weapon bolts and chassis fasteners
- [ ] Calibration / commissioning steps (IMU zeroing, ESC arming, meltybrain calibration)
- [ ] Photos of the partially-assembled bot at 2–3 stages

---

## 4. Meeting Minutes — pull into main.md

Currently only in `meetingNotes.md`. Judges want them in the main document.

- [x] Copy a summarized minutes table (date, attendees, topics, decisions) into `main.md` under Team Procedures or Time Management
- [x] Keep it tight — table format, not transcripts
- [x] Cross-reference `meetingNotes.md` for the long form

---

## 5. Wiring Schematic — needs to be a diagram

Currently a bulleted list. Judges want a real schematic.

- [ ] Draw a wiring diagram: battery → kill switch → BEC → Pi → ESCs → motors, plus IMU and receiver
- [ ] Fusion 360 Electronics, KiCad, or even a hand drawing photographed cleanly is acceptable
- [ ] Include fuse / kill-switch callouts (safety judges look for this)

---

## Smaller drawing fixes — ASME compliance

Our engineering drawings (`Images/Engineering Drawings/*.pdf`) use ASME Y14.5, inch units, ANSI B-size (11×17). Two gaps:

- [ ] Add a **third-angle projection symbol** to the title block on each drawing
- [ ] Add an **"UNLESS OTHERWISE SPECIFIED: ±.01"** tolerance note (or whatever tolerance the team is holding)
- [ ] Any new drawing: match the existing ASME style + ANSI B-size

---

## Deadline

Competition: April 25, 2026. Submission window closes before that.

Testing Results (#1) is the single highest-leverage fix — all three graders flagged it, and Grader 1 estimated it alone swings us from B+ to A.
