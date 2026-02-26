# OT Tabletop Exercise — Print Packet

**Exercise:** Design Meets Reality: FRCS Commissioning Under Pressure
**Duration:** 75 Minutes | **Format:** Team-based discussion

---

# SCENARIO BRIEFING

A mid-size A/E firm is leading the design and commissioning of a critical infrastructure facility with federal/DoD funding. The facility includes a Facility Related Control System (FRCS). The project is transitioning from design (60–70% complete) into early commissioning.

**Technical environment:** FRCS connected to enterprise reporting. Engineering workstations on VPN. Shared cloud repository with drawings, specs, network diagrams, and controller configurations. Multiple vendors with remote access.

**Who is involved:** Owner/End User, A/E Firm, Controls Integrator, IT/Cybersecurity, General Contractor, Contracting Officer (referenced)

**The gap:** No formal CUI determination has been made. DFARS 252.204-7012 is in the contract, but no marking, scoping, or handling plan was developed. Design files have been shared freely across all parties.

**Starting conditions:** Systems normal. Commissioning on schedule. No prior incidents. No one expects a problem.

---

# YOUR ROLE CARD

*(Circle your assigned role)*

**Incident Lead** — You run the table. Force decisions. Manage time.
- Bias: You want a clean plan. Incidents aren't clean.
- Ask: "Are we deciding or just talking?"

**OT Operations Lead** — You own the controllers, SCADA, FRCS, and the physical process.
- Bias: You resist shutting down. You trust the integrator.
- Ask: "Can we verify controller integrity independently?"

**Engineering / Design Lead** — You own the drawings, specs, and design basis.
- Bias: You see this as an IT problem. Your files are just files.
- Ask: "If our deliverables are CUI, what does that change?"

**IT / Security Lead** — You own enterprise IT, VPN, endpoints, and monitoring.
- Bias: The user clicked the link. That's a people problem.
- Ask: "Do we have logs showing what was accessed and when?"

**Contracts / Compliance Lead** — You own contract obligations, flow-downs, and notifications.
- Bias: CUI marking is the government's job. If they didn't mark it, it's not your problem.
- Ask: "What are our notification timelines, and have we missed one?"

---

# INJECT SEQUENCE

## Inject 1 — The Attachment That Looked Routine
A project engineer opens an attachment from what appears to be the controls integrator. The workstation — connected to the shared repository via VPN — slows briefly. No one reports the email.

- Who would most likely open this? Would they report it?
- What safeguards should prevent one email from becoming project-wide?
- Who gets notified, and how fast?

## Inject 2 — Someone Downloaded Everything
Two days later: compromised credentials used to bulk-download 65% design drawings, network diagrams, specs, and controller configs from the shared repository at 2:00 AM. No alerts triggered.

- Who owns the shared repository?
- Would your project detect this?
- What is your first action?

## Inject 3 — The Network Boundary That Wasn't There
Unusual traffic detected between enterprise IT and OT networks. File-sharing protocol crossing a boundary that shouldn't exist. Integrator admits they "temporarily connected" the networks. No change request filed.

- Who approves network changes on your projects?
- What's the difference between a temporary shortcut and a security gap?
- How do you explain this to the facility owner?

## Inject 4 — The Controller Logic Changed
A controller subroutine has been modified — a timer value affecting a critical process. The change doesn't match any approved revision. Can't determine if it was unauthorized, corrupted, or pushed from the compromised workstation. Facility is actively operating.

- Keep running, shut down, or isolate?
- Who has authority to make that call?
- How do you verify controller logic if you can't trust the workstation?

## Inject 5 — Everyone Wants Answers
Reporter calls the owner. Contracting Officer emails requesting confirmation no controlled information was compromised. Insurance carrier asks if this is a notifiable event. No one has coordinated a response.

- Who speaks to media, KO, and insurer — right now?
- What can you actually confirm vs. what are you guessing?
- What do you wish you'd prepared before today?

## Inject 6 — The Question That Should Have Been Asked at Kickoff
Legal counsel asks: "Has anyone determined whether these project deliverables qualify as Controlled Technical Information under DFARS?" Files were never marked. Repository never assessed. Subcontracts don't mention CUI. If these are CUI, the firm has been non-compliant since day one.

- When should someone have asked the CUI question?
- Who on your real projects is responsible for CUI scope?
- What would a CMMC assessor find tomorrow?

---

# PARTICIPANT WORKSHEET

**Your Role:** ______________________________
**Table:** ________ **Date:** ________________

| Inject | What Happened? | Our Decision | Evidence Needed | CUI? | Who Owns It? |
|--------|---------------|-------------|-----------------|------|-------------|
| 1 | | | | Y/N/? | |
| 2 | | | | Y/N/? | |
| 3 | | | | Y/N/? | |
| 4 | | | | Y/N/? | |
| 5 | | | | Y/N/? | |
| 6 | | | | Y/N/? | |

**Biggest gap identified:** ___________________________________________________

**One action within 30 days:** ________________________________________________

**Responsible:** ________________________ **Date:** __________________________
