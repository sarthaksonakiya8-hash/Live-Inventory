# Bluefin Insights: Live Skills Inventory (`GEMINI.md`)

## Context
Bluefin Insights is a 25-person consumer-research and analytics firm in Gurugram. Founder Meera Rao needs to assemble a bid team by Friday 2 October for a major Halcyon Bank customer-experience study across Tamil Nadu and Maharashtra, requiring SQL and data work on bank customer data, banking knowledge, survey design, fieldwork in Tamil and Marathi, and strong client presentation skills. Because the existing HR skills register is two years out of date, this project builds a trustworthy, evidence-backed skills inventory from actual project work.

## Files in This Folder
* `README.md`: Explains the Halcyon Bank bid scenario, lists the 20 tracked skills across five groups (Technical, Client, Domain, Languages for fieldwork, Other), and defines the three proficiency levels (**1** basic, **2** working, **3** expert).
* `people.csv`: The current staff roster (name, team, role, manager, joining date, and status such as active or on leave).
* `skills_register.csv`: The outdated October 2024 self-reported HR skills spreadsheet (useful for comparison only, not as sole proof).
* `team_chat.csv`: Three months of internal team chat messages (July–September 2026) with message IDs (such as `M042`), timestamps, channels, chat display names (such as `Lakshmi N.`), and message text.
* `project_notes/`: Six project retrospectives and handover notes written by project leads detailing who delivered what work on recent engagements.

## Technical Rules & Agreed Plan
* **Pure HTML and JavaScript only:** No server, no internet connection, no build step, and no external libraries.
* **Two-file deliverables:**
  * `index.html`: A single local web page that opens directly by double-clicking and loads `data.js` via a standard `<script>` tag.
  * `data.js`: A separate JavaScript data file generated ahead of time from the folder's CSVs and project notes. No AI calls are made from inside the page.
* **Strict taxonomy:** Use only the exact 20 skills and three levels (**1**, **2**, **3**) defined in `README.md`.
* **Required page views:**
  1. **Employee Cards:** One card per current person in `people.csv` showing their details, current availability status, assigned skills and levels, and visible/clickable references to the exact chat message IDs or project note file names proving each skill.
  2. **Skill Filter:** A filter by any of the 20 skills showing matching headcount and highlighting supporting proof.
  3. **Halcyon Bid Team View:** Organises current staff against Meera's five bid requirements, displaying proficiency levels, supporting evidence, and availability flags (such as staff on leave).

## How to Work
* **Plan before building:** Always explain the proposed plan clearly and wait for explicit go-ahead before writing or modifying code.
* **Evidence only:** Never assign a skill or proficiency level without verifiable evidence in `team_chat.csv` (cited by message ID) or `project_notes/` (cited by file name).
* **Flag uncertainty:** State openly when evidence is ambiguous, conflicting, or missing (for example, name collisions or unconfirmed skill depth) rather than guessing.
* **Plain British English:** Explain every change or decision in one or two concise sentences of plain British English.