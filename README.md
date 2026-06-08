# 🏭 Migrating the Unmigrateable
### A practical, open-source toolkit for legacy ICS migration and CRA compliance

> *"Most facilities don't have an asset inventory problem. They have a confidence problem.  
> The gap between what they think they have and what's actually there is where breaches happen  
> and where migration projects fail before they start."*

---

## What This Is

This repository is the living companion to the **Migrating the Unmigrateable — Study Notes** LinkedIn series.

It is a **learning-in-public project**. I am not a 20-year OT veteran. I come from IT support, application management, vulnerability patching, and cybersecurity monitoring. When I looked seriously at the OT and ICS world, one thing hit me immediately:

> Everything the IT world learned the hard way about security over 20 years, OT is about to learn all at once — under regulatory pressure, with zero downtime tolerance.

I couldn't find a single practical, honest resource explaining step-by-step how you actually migrate a legacy ICS environment without destroying your uptime, your budget, or your sanity.

So I'm building that resource. In public. Post by post. Commit by commit.

---

## Why This Matters Now

**December 2027.** The EU Cyber Resilience Act takes full effect.

Manufacturers of PLCs, SCADA systems, and HMIs are preparing. They'll ship CRA-compliant products. They'll be fine.

The harder problem sits with the **asset owners** — the facilities running equipment installed in 2005, 2009, 2012. Equipment designed for 25-year lifespans, with no patch mechanism, no authentication, no encryption, running protocols that predate the assumption that these systems would ever touch a network connected to the outside world.

Those devices aren't going anywhere. And they're now under pressure from:

- 🇪🇺 **CRA** : Cyber Resilience Act (Dec 2027)
- 🇪🇺 **NIS2** : Already in force for operators of essential services
- 🛡️ **Cyber insurance** requirements tightening
- 🏢 **Client and procurement** security requirements increasing

Most asset owners face the same three constraints simultaneously:
- No budget for full replacement
- No downtime window to execute it even if they had budget
- No clear methodology for how to approach it in phases

This toolkit is for them and for the engineers and consultants helping them.

---


---

## Standards Reference

| Standard | Scope | Relevance |
|----------|-------|-----------|
| **IEC 62443** | Industrial Automation & Control System security | Primary OT security framework. Templates aligned to this. |
| **NIST SP 800-82** | Guide to OT Security | Practical US companion to IEC 62443. Freely available. |
| **EU CRA** | Cyber Resilience Act | Applies to manufacturers selling in EU from Dec 2027. Indirect pressure on asset owners. |
| **EU NIS2** | Network & Information Security Directive 2 | Already in force. Applies to operators of essential services NOW. |
| **Purdue Model** | ICS network architecture reference | Used throughout for zone definitions and asset classification. |

---

## How to Use These Templates

1. **Start with MtU #01** — Asset Inventory. You cannot migrate what you don't know you have.
2. **Fill in the Cover sheet** with your facility details and classification level.
3. **Run passive monitoring** first (Claroty, Nozomi, Dragos, or Tenable OT) before touching any device.
4. **Conduct a manual walkdown** — passive monitoring misses air-gapped and serial-connected devices.
5. **Cross-reference documentation** against what you found. Every gap is a finding.
6. **Populate Risk Flags** from your inventory — these drive Phase 1 prioritisation.

> ⚠️ **Important:** These templates are starting points, not finished deliverables. Every OT environment is different. Adapt to your context. If you're working on a safety-critical environment (SIL-rated systems, nuclear, water treatment) involve qualified functional safety and cybersecurity professionals.

---

## Contributing

Corrections, improvements, and additions from practitioners are genuinely welcome.

This is a learning-in-public project. If I've oversimplified something, missed a real-world constraint, or got something wrong — open an issue or submit a PR. That kind of feedback makes this more useful for everyone.

**Especially welcome:**
- Real-world edge cases these templates don't handle
- Additional standards alignment (ISA/IEC, NERC CIP, sector-specific)
- Translation of templates into other languages
- Sector-specific variants (water, energy, manufacturing, pharma)

---



## Disclaimer

These templates and notes are educational resources produced as part of a personal learning project. They are not professional security consultancy advice. For critical infrastructure, safety systems, or regulated environments, always engage qualified OT cybersecurity professionals.

The author is not affiliated with any vendor, tool, or standards body mentioned in this repository.

---

## License

**Creative Commons Attribution 4.0 International (CC BY 4.0)**

Free to use, adapt, and redistributeincluding commercially with attribution.

> *"Migrating the Unmigrateable — Study Notes" by Yassar Al-Buhaisi, https://www.linkedin.com/in/yassar-al-buhaisi/*


