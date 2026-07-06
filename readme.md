**Project: DVI Match Assist — Disaster Victim Identification Support Tool**

- **Problem it solves:** After a disaster, families report missing people (ante-mortem data) and forensic teams log unidentified bodies (post-mortem data). Matching the two lists manually is slow and error-prone — this tool speeds that up.

- **Two data intake forms:**
  - Families/police fill in details about a missing person (age, height, dental info, photos, marks/tattoos)
  - Forensic teams log details found on unidentified remains

- **Matching engine (the core logic):**
  - Compares both records feature-by-feature (age range, height, dental chart, marks)
  - Gives each pair a confidence score
  - Shows forensic reviewers a ranked list of "most likely matches" instead of them checking everything manually

- **Dashboard for reviewers:**
  - View ranked matches per case
  - Accept, reject, or flag a match for DNA confirmation
  - Track case status (open, under review, confirmed, closed)

- **Tech stack:**
  - Frontend: React + Tailwind (dashboard + forms)
  - Backend: Supabase or a small Python/FastAPI service for the matching logic
  - Matching: simple rule-based scoring first, optional ML (image similarity) as a stretch goal

- **Important framing:** This is a *decision-support* tool — it narrows down candidates faster. It doesn't replace DNA/fingerprint/dental confirmation, which is legally required for final identification.

- **Why it's a good project:** No real sensitive data needed (use mock data), touches both full-stack and ML skills, and solves a gap the government has openly admitted exists.
