📚 **Migrating the Unmigrateable - Study Notes | [MtU #06]**  
_A learning-in-public series on legacy ICS migration and CRA compliance_

---

**"We did a migration two years ago" is not a compliance posture. It's a historical event. NIS2 wants to know what you did last month.**

Phase 5 is where the project becomes a program. Everything before this was about reaching a better place. Phase 5 is about staying there and continuously showing that you are, whenever anyone asks.

**Five pillars hold it up:**

📡 **Vulnerability Management**: new CVEs are published every day. A device clean at validation in April may have a critical vulnerability by July. Monthly CVE checks, quarterly passive scans, annual full assessments, immediate ICS-CERT advisory response. Results feed back into the Phase 1 risk register. It's a loop, not a line.

🔔 **Continuous Monitoring**:  your OT monitoring tool should do three things: discover new assets before you find out the hard way, detect behavioral deviations from baseline, match traffic against known ICS threat signatures. Alerting not just logging.

🔑 **Access Control Review**:  quarterly, not annual. Vendor contracts expire and access isn't removed. Engineers leave and accounts aren't disabled. MFA exceptions get made "temporarily" and never reversed.

📊 **Asset Management**:  your inventory from Phase 0 ages from day one. A contractor replaces a switch. A vendor pushes firmware. Our quarterly passive scan found a new undocumented device on VLAN 10. Again. Because it never stops.

📅 **Compliance Reporting**:  monthly vulnerability log, quarterly dashboard, annual evidence pack. What you hand a NIS2 competent authority, a cyber insurer, or a board. Not intentions. Evidence.

**Now the question nobody wants to answer:**

Who actually owns OT security in your organization?

IT says it's OT's problem. OT says it's IT's problem. The CISO says they don't have OT visibility. Plant management says they're responsible for production, not cybersecurity.

That ambiguity is itself a critical risk finding and the first thing a competent authority will ask about.

Phase 5 requires one named individual accountable for the program. Not "the OT team." One person. Authority. Reporting line to senior management. Quarterly review meeting with minutes and actions.

**Full template: 7 sheets: vulnerability log, alert register, access control review, security dashboard, compliance calendar

https://github.com/yassargo/migrating-the-unmigrateable/blob/main/MtU-06-cra-nis2-compliance/ICS_Operate_Monitor_Programme_MtU06.xlsx



_Next: [MtU #07] - The budget conversation. Building a business case for migration that actually gets approved._

**#ICS #OTSecurity #NIS2 #CRA2027 #IEC62443 #SCADA #MtU**
