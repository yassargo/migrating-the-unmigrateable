
📚 **Migrating the Unmigrateable - Study Notes | [MtU #01]** _A learning-in-public series on legacy ICS migration and CRA compliance_

**Ask a plant manager how many ICS devices are running in their facility.**

They'll give you a number. Confidently 🧠.

They're usually wrong... or 99% wrong unless it is a new facility with very strict change management and continuous monitoring on the network.

Not because they're incompetent, but because OT environments are built incrementally over decades, by different contractors, with different tools, and with exactly one priority: **keep it running.** Documentation was always the first casualty.

This is where every migration project starts, and where most fail before they've really begun.


**Phase 0 is called Asset Discovery. The goal sounds simple:**

_Find out everything that's connected, what version it's running, and what it does._

In IT, this is a Tuesday afternoon. You run a scanner, query Active Directory, check your CMDB, done 🎉.

In OT, it's a different ... way different 🔀.

First problem: **you cannot just run a scanner.** A standard network scan that your IT team runs without thinking twice can freeze a PLC, reboot a controller, or cause a field device to behave unpredictably, as Mr. Scotty (from Star Trek) would say: "She cannae take any more, Captain" 💥 . In a live production environment that's not a inconvenience, that's a potential incident. So active scanning is off the table until you know exactly what you're dealing with.

**So Phase 0 uses three methods in combination:**

**1.  Passive Network Monitoring** You connect a sensor to a network span port and listen. No packets sent. No interaction with any device. You build your inventory from traffic you observe there are tools that would do this automatically, identifying devices, protocols, and communication patterns.

Limitation: you only see devices that are actively talking during your monitoring window. Silent devices get missed.

**2.  Manual Walkdown** Someone physically walks the facility, clipboard/tablet in hand, and documents every device they can see and access. This sounds primitive. It is irreplaceable.

Because passive monitoring misses air-gapped devices, legacy serial connections, and anything not on an IP network. Eyes catch what software can't.

**3.  Documentation Review** You collect everything that exists — old network diagrams, maintenance records, vendor contracts, P&IDs and cross-reference it against what monitoring and walkdown found.


**Here's the thing that will make you uncomfortable:**

On almost every real assessment, the walkdown finds something that isn't in any documentation.

The classic examples and it happens more than anyone admits are:
-  **4G modem** installed years ago by a maintenance vendor for remote support access. Nobody documented it. The vendor contract expired. The modem is still there. Still connected. Still accepting incoming connections.
- Rogue PoE devices hiding in ceilings or cabinets
- Dual-homed systems that violate segmentation


**At the end of Phase 0 you should have three things:**

- **Asset Inventory:** every device, every firmware version, every protocol, every EOL date, in one place
- **Network Topology Map:** how everything connects, including the connections that shouldn't exist
- **Initial Risk Flags:** EOL devices, known CVEs, undocumented access paths

Without these three documents, everything that follows is guesswork.

**Template for this:**

A proper ICS Asset Inventory workbook 5 sheets, covering asset discovery, network topology, risk flags, and a reference guide with IEC 62443 and CRA alignment baked in.

Check it out here: https://github.com/yassargo/migrating-the-unmigrateable/blob/main/MtU-01-asset-discovery/ICS_Asset_Inventory_MtU01.xlsx

If you're an OT engineer, a consultant, or an asset owner starting to think about CRA compliance this is your starting point.

Next in the series: [MtU #02] Not all legacy is equal. How do you score risk across your inventory and decide what to migrate first?

_What did I get wrong or oversimplify? I'm learning this in public — corrections from practitioners are genuinely welcome in the comments._

**#ICS #OTSecurity #CyberResilience #CRA2027 #SCADA #IEC62443 #NIS2 #MtU**
