# Copilot Instructions for mentorship-tracker

## Project Overview
This repository tracks mentorship activities, sessions, and outcomes. The main data is stored in a tabular text file under `mentorship-tracker/tracker details`.

## Architecture & Data Flow
- **Single-file data store:** All mentorship session records are kept in a single table-formatted text file (`mentorship-tracker/tracker details`).
- **No code or automation:** There are currently no scripts, build systems, or automated workflows. All updates are manual.
- **Session records:** Each row in the table represents a mentorship session, including metadata (date, location, students, activities, outcomes, and evidence links).

## Key Conventions
- **Tabular format:** Data is stored as a markdown-like table. Maintain column alignment and headers when updating.
- **Evidence links:** Use direct URLs for evidence. Validate links before adding.
- **Session numbering:** Increment `Session No.` for each new entry.
- **Topics and activities:** Be descriptive and specific in the `Topics Taught` and `Mentoring Activity` columns.

## Developer Workflows
- **Add a session:**
  1. Copy the previous row and increment `Session No.` and `Date`.
  2. Update all relevant columns with new session details.
  3. Ensure the table remains properly formatted.
- **Update outcomes:**
  - Edit the `Outcomes & Improvements` column to reflect new results or improvements.
- **Link evidence:**
  - Add or update the `Evidence Link` column with a valid URL.

## Patterns & Examples
- **Example row:**
  | 2 | 11/25/2025 | ASC - Grazebrook RoboThink UK, Stanmore | 3:15 pm - 4:45 pm | 12 | Build a Simple Robot | Guided group mentoring for 12 students; Focused on teamwork and basic robotics assembly | Robot Kit, Battery | 10 students completed robot; 2 improved teamwork | https://drive.google.com/open?id=EXAMPLE |

## External Dependencies
- None. All data is local and manually managed.

## Directory Reference
- `mentorship-tracker/tracker details`: Main data file
- `.github/copilot-instructions.md`: AI agent instructions
- `README.md`: Project summary

## Guidance for AI Agents
- Focus on maintaining data integrity and clarity in the session table.
- Do not introduce code, scripts, or automation unless requested.
- When in doubt, ask for clarification on session details or formatting.
