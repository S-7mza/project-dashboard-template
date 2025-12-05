# Dashboard Project Process Audit – Maturity View (CMMI-style)

Score: **8 / 10**

## Scope of this audit

Reference: a simplified CMMI-style maturity view (from ad-hoc to optimizing) applied to your dashboard project process.

### Maturity scale

- **1 – Initial:** Unpredictable, poorly controlled, reactive.
- **2 – Managed:** Projects planned and tracked; basic discipline.
- **3 – Defined:** Processes documented, standardized and integrated.
- **4 – Quantitatively Managed:** Processes measured and controlled.
- **5 – Optimizing:** Focus on continual improvement using quantitative feedback.

## Scoring barème (out of 10)

The 5 maturity levels are mapped to a 0–10 score as follows:

- Level 1 – Initial: **0–3/10**
- Level 2 – Managed: **4–5/10**
- Level 3 – Defined: **6–7/10**
- Level 4 – Quantitatively Managed: **8–9/10**
- Level 5 – Optimizing: **10/10**

The current **8/10** reflects a strong Level 3 (Defined) baseline with some Level 4 characteristics in planning & tracking, but without fully institutionalized measurement and optimization.

## Assessment by key area

- **Process definition (Level 3 – Defined):**
  - You have a documented, repeatable process with clear artefacts for each phase (workshops, agile delivery, governance, QA, deployment).

- **Project planning & tracking (Level 3–4):**
  - Workshop planner, sprint planning, and trackers show consistent planning and tracking.
  - Quantitative use of those trackers (e.g., trend analysis) is not fully formalized.

- **Quality & risk management (Level 3):**
  - Templates and checklists are present and clear; consistency of application and measurement could be strengthened.

- **Organizational learning (Level 2–3):**
  - Retrospectives and benefits tracking exist, but there is limited explicit process for feeding lessons back into standards and training.

## Overall maturity judgement

- **Overall maturity level:** around **Level 3 (Defined)**, leaning toward Level 4 in planning & tracking.
- **Numeric summary:** considering strengths and gaps, an overall maturity score of **8/10** is reasonable for your current template.

## Suggestions to progress toward Level 4–5

1. **Measurement framework:**
   - Define a minimal set of process KPIs (e.g., cycle time from data discovery to first prototype, defect density per release, missed workshop dates) and how to collect them.

2. **Feedback into standards:**
   - After each project, review retros, issues, and benefits tracker, and record process changes in `docs/BEST_PRACTICES.md` (e.g., a running change log section).

3. **Training & onboarding:**
   - Add a short "How to use this playbook" training script/slide outline in `deliverables/DASHBOARD_USER_GUIDE.md` or a dedicated training file to ensure new PMs/teams use the process consistently.

## Concrete path to 10 / 10

To move from **8/10** (between Defined and Quantitatively Managed) to **10/10** (Optimizing):

1. **Standardize a minimal KPI set for the process itself**
  - Choose 3–5 key process KPIs (e.g., lead time from kickoff to first dashboard version, % of workshops held on time, number of production incidents in first 3 months, UAT defect density).
  - Document these in a small "Process KPIs" section (e.g., in `docs/BEST_PRACTICES.md` or a new `docs/PROCESS_METRICS.md`).

2. **Collect and review metrics across projects**
  - For each project, record these KPIs and review them during retrospectives and benefits reviews.
  - Periodically (e.g., quarterly) compare metrics across projects to identify systemic issues.

3. **Systematically feed metrics into improvements**
  - When metrics indicate recurring delays or defects, create specific improvement actions (e.g., new checklist items, refined workshop agendas) and log them in `docs/BEST_PRACTICES.md`.
  - Track completion of those actions and their impact on subsequent projects.

4. **Institutionalize training and onboarding**
  - Use the training script/user guide to onboard every new PM or team using this playbook.
  - Include examples of metrics and improvements to create a culture of data-driven refinement.

5. **Audit periodically against your own standard**
  - Once or twice a year, re-run these maturity and reference-based audits and compare scores over time.
  - Update the process, templates, and training based on audit findings, closing the loop toward continuous optimization.

---

**Overall maturity view:** a well-designed, defined process that is ready to be measured and optimized across multiple dashboard projects.
