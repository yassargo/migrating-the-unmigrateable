📚 **Migrating the Unmigrateable - Study Notes | [MtU #03]**  
_A learning-in-public series on legacy ICS migration and CRA compliance_

---

**The most dangerous moment in an OT environment isn't a cyberattack. It's a well-intentioned engineer making a network change without knowing what depends on what.**

Phase 2 lives in that risk. Here's why.

Phase 0 found everything. Phase 1 scored everything. Phase 2 means touching a live environment (M.C. Hammer's song: "U Can't Touch This", is your best friend 🤣)

Why not just replace legacy devices and skip the fix straight away?

Three reasons: 
1. Budget (rip-and-replace can be expensive, vey expensive in some instances).
2. Zero downtime tolerance on critical processes.
3. Risk sequencing: Migrate systems in stages instead of all at once, so any issue stays limited rather than affecting the whole plant.

Segmentation is the bridge. It buys time while reducing risk on what can't be replaced yet.

**Four techniques do the work:**

🔹 VLAN isolation: group assets by zone so an attacker can't move laterally  
🔹 OT-aware firewalls / data diodes: physically enforce one-way traffic at IT/OT boundaries  
🔹 Remote access hardening: every vendor VPN, every RDP session, every forgotten modem gets documented, MFA'd, or disconnected  
🔹 Compensating controls: for devices that can't move yet: isolate, whitelist, monitor, lock the cabinet, formally document the accepted risk with a committed fix date

Here's the constraint that makes OT segmentation harder than IT: you can't just push a config change. A PLC talking to a field device may have millisecond timing requirements. Firewall latency invisible in IT can cause a process fault in OT. Every change goes through a formal Management of Change process: documented, reviewed, scheduled, verified, rollback plan ready before anyone touches anything.

One thing that surprised me: most people think they have until December 2027.

They don't.

NIS2 is already in force. Operators of essential services: energy, water, transport are required to have segmentation and access controls in place now. CRA gets the headlines. NIS2 is already enforceable. 😬

Phase 2 produces: a Segmentation Design, a Conduit & Firewall Rule register, a Remote Access Register, a Change Management Log, and a Compensating Controls register for what's still pending migration.

**Full template 7 sheets**

_Next: [MtU #04]  Migrating without killing the plant. Executing the cutover with a 99.9% uptime requirement breathing down your neck._


**#ICS #OTSecurity #NIS2 #CRA2027 #IEC62443 #SCADA #MtU**
