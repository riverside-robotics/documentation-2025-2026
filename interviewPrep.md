# Interview Preparation — Riverside Robotics Team Meltdown

## Overview

The AWT RoboBots interview is a **15-minute conversation** with a panel of **three judges**. It is not a presentation — judges will ask questions and may follow up for clarification. Every team member is expected to participate and speak. The interview is scored on both the **content of your answers** (32 points) and your **delivery** (12 points) for a maximum of **44 points**.

---

## Format Reminders

- Every team member is expected to participate in the interview
- You may still interview even if the bot does not pass the safety check
- You **cannot** participate if documentation is not submitted on time
- Judges ask the same set of questions to every team — answers should be thorough on the first pass
- Supporting documents or visuals may be brought, but time is limited
- The top three teams from the initial round are invited back for a final interview on competition morning

---

## Scored Questions and Suggested Talking Points

### Q1: How did you come up with the design idea for your robot?

**Who should answer:** Design team members (Ayden, Adam P., Jayden)

**Key points to hit:**
- Spinlayden 2.0 is an evolution of last year's Spinlayden, our first meltybrain full-body spinner
- We analyzed Spinlayden 1.0's performance — created a positive/negative analysis of what worked and what didn't
- Watched previous AWT competitions and other combat robotics streams to study what designs succeed
- Whiteboarded ideas, compared advantages and weaknesses of different configurations
- Chose to iterate on the proven hexagonal meltybrain design rather than start from scratch — allowed us to use returning members' knowledge and reuse spare parts
- The hexagonal shape provides structural rigidity from any impact angle and allows mounting six blades

---

### Q2: What most surprised you about the robot building experience?

**Who should answer:** Spread across the team — everyone should have a personal answer

**Key points to hit:**
- How many different disciplines are involved (CAD, software, electronics, machining, documentation, project management)
- The software pivot from Python to C# mid-season — sometimes a major change is worth it for better performance
- How much time manufacturing takes compared to design — waterjet cutting, CNC milling, 3D printing all have their own timelines
- The corrupted Raspberry Pi setback in January — learning to plan for hardware failures
- How important documentation is to the engineering process — not just an afterthought
- The team grew from 8 to ~20+ members, and managing that expansion was a challenge in itself

---

### Q3: What advice would you give a new team just getting started in RoboBots?

**Who should answer:** Returning members and leadership (Tom, Dustin, Sultan, Robert)

**Key points to hit:**
- Start documentation early — don't leave it until the end
- Watch previous AWT competitions to understand what works in the arena
- Don't overcomplicate your first design — a simple, well-built bot beats a complex, half-finished one
- Budget your time carefully — the Build phase (Jan–Mar) goes faster than you think
- Build relationships with sponsors early — Monode, Arc Technology, and Show Studio have been critical to our success
- Make sure everyone on the team has a role and feels ownership over part of the project
- Test early and test often — don't wait until the week before competition

---

### Q4: What do you wish you'd done better? / What would you do differently next year?

**Who should answer:** Honest answers from multiple members

**Key points to hit:**
- Started manufacturing earlier — we didn't begin metal assembly until April
- Could have had a more structured timeline/Gantt chart from the beginning
- The Python-to-C# software rewrite could have been avoided if we'd evaluated languages earlier
- More formal testing procedures — we did informal spin tests but could have done scientific testing (aggression, durability, maneuverability)
- Better integration between the design and software teams earlier in the season
- > TODO: Ask team members for their personal "wish I'd done better" answers — judges value honesty and self-awareness here

---

### Q5: What are the strengths of your robot? If you were going against your bot, where would you avoid?

**Who should answer:** Design and strategy members (Ayden, Adam P., Robert)

**Key points to hit:**
- **Full-body spinner** — the entire bot IS the weapon. There's no safe angle of approach; every side has A516 carbon steel blades
- **645.6 RPM spin speed** creating a ~26.9 mph steel barrier — acts as both offense and defense simultaneously
- **Double-sided design** — operates normally when flipped, recovers in ~2 seconds
- **Hexagonal structural rigidity** — six-sided chassis absorbs impact from any direction
- **78 joules per rotation** of kinetic energy delivered through six blades
- **Where to avoid:** Don't approach from the side — that's where blade tip speed is highest. The spinning steel barrier deflects attacks before they reach the chassis

---

### Q6: What are the weaknesses of your robot? If you were going against your bot, where would you attack it?

**Who should answer:** Design and strategy members — be honest but show you've thought about mitigation

**Key points to hit:**
- **Spin-up time** — before the bot reaches full RPM, it's vulnerable. An aggressive rush before we spin up could be effective
- **Raspberry Pi dependency** — onboard computing is a single point of failure. If the Pi is damaged, the meltybrain control system goes down (though we added a dedicated housing this year to mitigate this)
- **Translational speed** — at 1-2 ft/s while spinning, we're not the fastest bot in the arena. A fast wedge bot could outmaneuver us
- **Top/bottom plates** — the 1/8" aluminum plates are thinner than the 3/8" walls. A vertical spinner hitting the top could be dangerous
- Show that you understand the weaknesses but have designed mitigations for each

---

### Q7: How was the work divided on your team?

**Who should answer:** Management (Sultan) and multiple team members confirming their roles

**Key points to hit:**
- Team Meltdown has ~16 members split into functional groups:
  - **Mechanical/Design:** Ayden, Adam P., Jayden, Alexander — CAD in Fusion 360, chassis design, blade design
  - **Software:** Tom, Dustin, Vincent, Xayden — meltybrain control system (C#), Raspberry Pi setup, gyroscope integration
  - **Electrical:** Lukas D., Yash, Jayden — ESC wiring, motor setup, power distribution
  - **Documentation:** Tom, Jason, Mher, Daniel, and the 8th grade team members
  - **Management/Finance:** Sultan — parts list, budget tracking, team coordination
  - **Operations/Driver:** Robert — bot operator during competition
- Highlight that many members contributed across multiple areas
- 8th grade JuniorBots members merged with the team in February, bringing fresh energy and perspectives
- Advisors Jack and Adam Carbone guide the team but students drive the decisions

---

### Q8: What one thing did you learn from this experience that you will use in your future?

**Who should answer:** Every member should have a personal answer ready

**Key points to hit (examples — personalize these):**
- **Engineering process:** How to take an idea from concept through CAD design to physical manufacturing
- **Problem-solving under pressure:** When the Pi got corrupted or the software needed a full rewrite, we had to adapt quickly
- **Teamwork and communication:** Coordinating 16+ people across design, software, electrical, and documentation
- **Manufacturing skills:** Waterjet cutting, CNC milling, 3D printing, soldering — real-world skills that translate directly to careers
- **Project management:** Budgeting $3,500+, managing timelines, working with sponsors
- **Documentation:** Learning that keeping accurate records is a critical professional skill, not just a school requirement
- > TODO: Each team member should prepare their own personal answer to this question before the interview

---

## Delivery Scoring (12 Points)

The judges also score your team's delivery on three criteria:

| Criteria | What Judges Look For | Tips |
|----------|---------------------|------|
| **Organization** | Does the interview cover the major sections of the documentation requirements? | Know your documentation inside and out. Be able to reference specific sections if asked. |
| **Delivery** | Did all team members speak? Good presentation skills? | Make eye contact, speak clearly, don't mumble. Every person must contribute at least one answer. Avoid having one person dominate. |
| **Effectiveness** | Did it convey how involved the team was and their knowledge of the design/build process? | Show genuine knowledge — don't just read memorized lines. Judges can tell when someone truly understands vs. when they're reciting. |

---

## General Tips

- **Arrive early**, look professional, greet the judges confidently
- **Review the documentation** thoroughly before the interview — know where every section is
- **Practice as a team** — rehearse common questions so responses flow smoothly and consistently
- **Don't talk over each other** — decide in advance who leads each question, then others add detail
- **Be honest** — if you don't know something, say so. Judges respect honesty over bluffing
- **Show passion** — the judges want to see that you genuinely care about robotics and engineering
- **Bring a copy of your documentation** for quick reference if needed

---

## Practice Schedule

> TODO: Set up at least 2 practice sessions before competition day (April 25). Have an advisor or parent act as a judge and ask the 8 questions. Time yourselves — you only have 15 minutes.

---

## Quick Reference Card

Take these stats into the interview so anyone can reference them:

| Stat | Value |
|------|-------|
| Bot Name | Spinlayden 2.0 |
| Weight Class | 15 lbs |
| Chassis Weight | ~12.6 lbs |
| Weapon Weight | 38 oz (6 blades x 6.33 oz) |
| Spin Speed | 645.6 RPM (~26.9 mph tip speed) |
| Kinetic Energy | ~78 J per rotation |
| Translational Speed | 1-2 ft/s while spinning |
| Motor Power | ~0.75 hp combined |
| Chassis Material | 6061-T6 Aluminum |
| Blade Material | A516 Grade 70 Carbon Steel |
| Brain | Raspberry Pi 4B (8 GB RAM) |
| Software | C# (meltybrain control) |
| Drive | 2x EZRUN 3660 SL G2 motors, 21:1 gear reduction |
| Total Budget | $3,554.48 ($2,199.25 new this year) |
| Team Size | ~16 members (Team Meltdown) |
| Season | September 2025 – April 2026 |
| Documentation Due | April 18, 2026 (11:59 PM) |
| Competition | April 25, 2026 |
