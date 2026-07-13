📚 **Migrating the Unmigrateable - Study Notes | [MtU #05]**  
_A learning-in-public series on legacy ICS migration and CRA compliance_

---

**Most migration projects validate that the process works. Almost none validate that the security controls work and document it in a format a regulator or insurer will accept.**

That gap is where the project becomes a liability instead of an asset.

Phase 4 is the phase most teams deprioritize. Plant is running, everyone breathes out, the next urgent thing lands and documentation gets quietly parked. But in a NIS2 and CRA world, undocumented work is invisible work. An auditor doesn't care that you replaced your legacy PLCs. They care that you can prove it.

**Phase 4 has two jobs:**

**① Technical validation: four layers, all signed:**

🔹 Functional: control loops, alarms, interlocks, HMI, historian tags verified against staging baseline  
🔹 Security:  firmware CVE check, firewall rules verified, monitoring confirmed, zero unauthorized traffic  
🔹 Performance: cycle time, latency, uptime. Performance regression on modern platforms is real and under-warned  
🔹 Integration: every dependent asset from Phase 0 verified. Not assumed. Integration failures are the most common source of post-migration incidents

**② Compliance documentation: the evidence that answers the six questions every auditor will ask:**

→ Do you know what's in your environment? (Phase 0)  
→ Have you assessed the risks? (Phase 1)  
→ Are you managing them? (Phase 2)  
→ Are changes controlled? (Phase 3)  
→ Can you prove the controls work? (Phase 4 — this phase)  
→ Is this ongoing? (Phase 5 — next)

Those six questions map directly onto the six phases of this framework.

The Compliance Evidence Summary sheet is the one I'm most proud of. One page per asset: risk finding → controls → segmentation reference → migration record → validation evidence → NIS2 Article 21 clause. Everything an auditor needs, in one place.


**Full template:



_Next: [MtU #06] — Operate & Monitor. Proving this isn't a one-time exercise._


**#ICS #OTSecurity #NIS2 #CRA2027 #IEC62443 #SCADA #MtU**

---


