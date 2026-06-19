📚 **Migrating the Unmigrateable - Study Notes | [MtU #02]**  
_A learning-in-public series on legacy ICS migration and CRA compliance_

---

**Your highest CVSS score is not your highest risk. In OT, the most dangerous device in your facility might not even be on your radar yet.**

Here's why that matters.

After Phase 0 you have your asset inventory. Let's say 150 devices. Twelve EOL. Twenty with known CVEs. Six with gaps you didn't expect.

You cannot fix all of it at once. Nobody has that budget. Nobody has that downtime window.

So where do you start?

The wrong answer: whatever scores highest on CVSS.

The right answer: whatever causes the most damage to the physical world if it gets compromised or goes offline.

This is called **consequence-based prioritization**: it's the single biggest mindset shift from IT security to OT security.

---

**A quick example.**

Two PLCs. Same CVE. Same CVSS score of 7.8.

PLC A controls a conveyor belt. It goes down ->  production pauses. Annoying. Recoverable.

PLC B controls a pressure relief valve with no manual override. It goes down -> you have a very different kind of problem. 😬

Same vulnerability. Completely different priority. CVSS doesn't tell you that. Only understanding the physical process does.

---

**Phase 1 scores every asset across three dimensions:**

**① Vulnerability (1–5)**:  CVEs, patch status, authentication, remote access  
**② Consequence (1–5)**: what happens physically if this device fails or gets hijacked  
**③ Exposure (1–5)**: network segmentation, IT/OT bridges, third-party access

Composite score = ① × ② × ③  range 1 to 125.

The scoring isn't perfect. No scoring system is. But it gives you something critical: a **defensible, documented decision** about what gets fixed first and why. When budget is limited and you can't do everything, that documentation protects you.

---

**What Phase 1 produces:**

- Risk Scoring Matrix: every asset scored, prioritized, with actions and owners  
- Zone Map: assets grouped into IEC 62443 security zones, conduits identified  
- Priority Shortlist: the ranked list that becomes your project execution order

In our sample assessment from [MtU #01], the undocumented 4G modem scores 125: maximum across all three dimensions simultaneously. That's not a coincidence. Unknown access is categorically worse than a known vulnerability, because you cannot apply compensating controls to something you don't know exists.

---

**The template is**


_Next: [MtU #03] - The Migration Framework. Six phases, decision gates, and how they connect into a project plan._


**#ICS #OTSecurity #CRA2027 #IEC62443 #SCADA #NIS2 #MtU**
