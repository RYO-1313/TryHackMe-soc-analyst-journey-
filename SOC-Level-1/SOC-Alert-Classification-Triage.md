# 🛡️ SOC Alert Classification & Triage — TryHackMe Writeup

**Platform:** TryHackMe
**Path:** SOC Level 1
**Category:** Security Operations
**Difficulty:** Easy

---

## 🔍 What the room covered

Introduction to SOC alert handling — what alerts look like, how they're structured (fields, statuses, classifications), and how an L1 analyst is expected to interact with them. The room also serves as preparation for the SOC Simulator and the SAL1 certification exam.

---

## 🧠 What I actually learned

**Alert prioritization comes first.** When an alert lands in the queue, the first move is checking its severity — Critical, High, Medium, or Low — so attention goes to the most dangerous potential threats first. The room focused on *who* to prioritize, not a full step-by-step triage procedure.

**Alert classification is a core L1 responsibility.** Every alert eventually gets labeled:
- **True Positive** — a real, confirmed threat
- **False Positive** — noise, not an actual threat

Getting this right matters because true positives that slip through become undetected attacks, and too many false positives lead to alert fatigue — analysts start missing things when they're drowning in noise.

**Alert statuses track the lifecycle of a ticket:**
- **Open** — alert is in the queue, no one has picked it up yet
- **In Progress** — an analyst has taken ownership and is investigating
- **Closed** — investigation is complete

**The L1 escalation trigger is simple:** if it looks like a real threat (true positive), escalate to L2 SOC. L1 doesn't resolve attacks — L1 filters and routes.

**Biggest mindset shift:** Before this room, the assumption was that SOC analysts are the ones actively fighting attackers. The reality is different — SOC analysts are filters. Their job is to sift through alert queues, separate real threats from noise, and make sure the right things reach the right people. The quality of what L2 receives depends entirely on how well L1 does this work.

---

## 💡 Key concept to remember

**L1 analysts are filters, not fighters.** The value of the role is in accurate triage — correctly classifying alerts and escalating real threats without flooding L2 with false positives or missing actual incidents.

---

## 🔑 How this connects to the SOC Analyst role

Every alert that enters a SOC queue needs someone to decide: *is this real, and how urgent is it?* That decision is L1's job. Severity determines order of attention. Classification determines what happens next. Status keeps the team coordinated. Getting these three things right is the foundation of effective SOC operations — and it's exactly what this room introduced.
