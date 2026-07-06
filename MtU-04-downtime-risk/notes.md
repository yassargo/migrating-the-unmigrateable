📚 **Migrating the Unmigrateable - Study Notes | [MtU #04]**  
_A learning-in-public series on legacy ICS migration and CRA compliance_

---

**Every migration plan looks perfect until the change window opens. Phase 3 is where you find out what you didn't know you didn't know.**

This is the phase most people picture when they hear "ICS migration." It's also the one most teams reach too early which is exactly why Phases 0, 1 and 2 exist first.

By Phase 3 you have your inventory, risk scores, segmentation in place, and change management proven. Now you actually replace things.

Replacing a device controlling a live physical process without stopping that process — is one of the hardest things in industrial engineering. I'd call it replacing the engine while the plane is flying. Not hyperbole. In some industries it's almost literally true. ✈️

**Four approaches depending on what you're migrating and what downtime you can tolerate:**

🔹 Parallel Run — new system runs alongside old, same inputs, compare outputs, cut over when confident. Discovers undocumented behaviours in the old system nobody knew existed. Better to find them here than after cutover.

🔹 Hot Cutover: old system offline, new system live, window closes. Highest risk. The change window is not for discovery it's for executing a plan you've rehearsed.

🔹 Incremental / Module-by-Module: migrate one loop at a time. Risk distributed across many small changes. Preferred for large DCS environments.

🔹 Greenfield Alongside: build new infrastructure, migrate processes onto it, decommission old progressively. Rare, expensive, sometimes the only honest answer.

Before any of this touches a live plant: staging environment first. Same hardware, firmware, logic no consequences if something breaks. Every hour in staging saves ten in crisis management. Skipping it is a false economy OT projects pay for at the worst possible moment.

Two Go/No-Go gates sit inside every cutover window. A named individual not a committee makes the call at each one. Under pressure, committees fail. Agree the authority before the window opens.

**Now the part nobody writes about.**

The OT engineer who maintained the legacy system for fifteen years isn't your obstacle. They know where every body is buried every quirk, every undocumented workaround, every near-miss quietly absorbed over the years.

Involve them from Phase 0. Not as a checkbox. As a genuine contributor. Projects that fail in Phase 3 almost always have a people problem underneath the technical one.

**Full template 7 sheets: 
https://github.com/yassargo/migrating-the-unmigrateable/blob/main/MtU-04-downtime-risk/ICS_Migration_Execution_Record_MtU04.xlsx


_Next: [MtU #05] — The vendor problem. EOL hardware, proprietary protocols, and CRA-ready replacements._


**#ICS #OTSecurity #CRA2027 #IEC62443 #SCADA #NIS2 #MtU**
