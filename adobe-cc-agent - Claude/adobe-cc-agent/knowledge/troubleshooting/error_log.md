# Error Log — Running Record of Issues and Fixes

Add an entry each time you encounter a recurring or significant error.
Over time this becomes a personal troubleshooting database specific to your setup and workflow.

---

## Log Format

Date — App — Short description of the error
What happened:
What caused it:
How I fixed it:
Prevention going forward:

---

## Example Entry 1

2026-01 — InDesign — Print PDF export, blues shifted to purple on magazine cover
What happened: Client magazine cover printed with purple tones on a bright blue logo element.
What caused it: RGB Illustrator logo placed in InDesign, PDF exported without colour conversion — RGB values passed straight through to the printer unchanged.
How I fixed it: Re-exported with Output tab set to Convert to Destination — FOGRA39. Blues rendered correctly on reprint.
Prevention going forward: Always check the Output tab colour conversion setting before any print PDF export. Added to magazine export checklist.

---

## Example Entry 2

2026-01 — Photoshop — Layered master PSD accidentally flattened during delivery
What happened: Client requested a revision after the flat delivery copy was accidentally saved over the layered master.
What caused it: Used File > Save instead of File > Save a Copy. The flattened version replaced the layered master file.
How I fixed it: Recovered from Time Machine backup.
Prevention going forward: Never use Save or Save As to create a flat delivery copy. Always use File > Save a Copy and name it clearly with FLAT in the filename. Archive layered masters immediately on project completion.

---

## Your Entries Below
