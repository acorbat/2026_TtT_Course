# AGENTS.md

## Project goal
Organize the **Taller de Fundamentos en Análisis de Bioimágenes (Formación de Formadores)**, a Train-the-Trainer course on Bioimage Analysis for LATAM, with a strong focus on:
- technical bioimage analysis content,
- pedagogy for training future instructors,
- logistics, budget, and invited-professor coordination,
- maintaining a single up-to-date project planning document.

## Canonical project files
- `COURSE_MASTER_PLAN.md` — main planning and organization file; keep it current.
- `curso_train_the_trainer_bioimagenes.md` — inspiration/source notes from the initial concept; preserve as reference.
- `fundacen_cursos.md` — FUNDACEN application context, scope, instructors, and consolidated budget references.
- `preguntas_presupuesto_fundacen.md` — FUNDACEN budget wording and budget-line details.
- `_quarto.yml` — configuration file for the Quarto-based course website.
- `index.md` — homepage of the course website.

## Planned folder structure only — do not create unless explicitly requested
Use this structure as the organizational plan for future work:
- `admin/`
- `02_program/`
- `03_topics/`
- `04_lectures/`
- `05_invited-professors/`
- `budget-funding/`
- `07_logistics/`
- `08_registration-selection/`
- `09_communications-outreach/`
- `10_materials-datasets/`
- `11_meetings-notes/`
- `12_archive/`

## Working style for this project
- Keep planning documents in **clear operational Markdown**.
- Prefer **English** for structure and management text, but preserve names, institutions, and existing course terminology in their original language when helpful.
- Use **ISO dates** (`YYYY-MM-DD`) whenever possible.
- Separate information into these categories:
  - **Confirmed**
  - **Tentative**
  - **To confirm**
- Do not present assumptions as facts.
- If costs are estimated, label them clearly as **rough estimate** and include currency.

## How to track work
When updating `COURSE_MASTER_PLAN.md`, maintain these sections:
1. **Summary** at the top
2. **Gantt / timeline** with major milestones and deliverables
3. **To-do list** with checkboxes
4. **Organization & logistics**
5. **Topics & program**
6. **Invited professors**
7. **Budget & funding**
8. **Open questions / decisions needed**

## Task tracking conventions
- Use checkboxes for action items.
- For important items, include:
  - owner,
  - target date,
  - dependency,
  - status.
- Suggested inline status markers: `TODO`, `IN PROGRESS`, `BLOCKED`, `DONE`.
- Keep one source of truth per topic; avoid duplicating contradictory information.

## Topic tracking conventions
For each teaching topic, keep:
- why it belongs in the course,
- how it should be taught in train-the-trainer format,
- expected pre-work,
- practical activity idea,
- candidate lecturer/facilitator,
- planned future file path.

## Professor tracking conventions
For each invited professor, track:
- institution and country,
- role in the course,
- invitation status,
- estimated travel and lodging cost,
- proposed funding source,
- deadlines for booking and confirmation.

## Local instructor tracking conventions
For each local instructor or facilitator, track:
- institutional role,
- expected contribution to the course,
- invitation/commitment status,
- preparation and training time required,
- topic assignment,
- rehearsal and coordination milestones.

## Budget conventions
- Keep costs grouped by:
  - travel,
  - accommodation,
  - catering,
  - local logistics,
  - participant support,
  - software/platform/materials,
  - contingency.
- Distinguish between:
  - covered by registration fees,
  - covered by institutional funds,
  - covered by grants/sponsorship,
  - funding source not yet assigned.

## Editing rules for future sessions
- Update existing planning files instead of creating redundant ones.
- Do not create the planned folders unless the user explicitly asks.
- If a new decision changes dates, budget, or scope, reflect it in:
  - summary,
  - Gantt chart,
  - to-do list,
  - relevant detailed section.

## Course website (Quarto)
The project now holds the official course website, which is configured and built using **Quarto**.
- **Configuration**: The website structure, navigation sidebar, theme, and output options are managed via `_quarto.yml`.
- **Render Exclusion**: Internal planning documents like `COURSE_MASTER_PLAN.md`, `AGENTS.md`, and `README.md` are excluded from the site render list in `_quarto.yml`.
- **Local Development**:
  - The Quarto CLI is managed via Pixi in the `quarto` feature environment.
  - To preview changes locally, run: `pixi run -e quarto quarto preview`
  - To render the final static pages into the `_site/` directory, run: `pixi run -e quarto quarto render` (Note: it is not necessary to render quarto manually as this is done automatically).

## Course material conventions
For course materials (presentations and workshops), follow these conventions:

### General workflow

- **Slides & Presentations:** The goal is to publish all slides in Zenodo containing both the raw source files (`.tex` or `.ppt`) and the rendered `.pdf` files. The rendered view (PDF link) must be linked in the corresponding page in the [presentaciones](file:///C:/Users/corba/Documents/2026_TtT_Course/presentaciones) folder, along with its Zenodo citation.
- **Workshops & Practicals:** Workshops must be published in GitHub, using `pixi` tasks to set up the workspace. A release of the workshop should be published in Zenodo and cited in the workshop page. Inside the [practicos](file:///C:/Users/corba/Documents/2026_TtT_Course/practicos) folder, there should be a link pointing to the workshop repository on GitHub, the data (if necessary), and the Zenodo citation.

### Presentation page layout
Every presentation file in [presentaciones](file:///C:/Users/corba/Documents/2026_TtT_Course/presentaciones) must follow this structure:

#### English
1. **Quarto Frontmatter:**
   ```yaml
   ---
   title: "¿Qué es Análisis de Bioimágenes?"
   subtitle: "Una introducción formal a qué es el análisis de bioimágenes."
   format: html
   ---
   ```
2. **Learning Objectives Callout:**
   ```markdown
   ::: {.callout-tip}
   ## Objetivos de Aprendizaje
   Al finalizar la sesión, los alumnos deberán ser capaces de:
   - <objective_1>
   - <objective_2>
   :::
   ```
3. **Slides Section (HTML iframe for Zenodo PDF viewer):**
   ```markdown
   ## Slides
   <iframe src="https://docs.google.com/viewer?url=https://zenodo.org/records/<RECORD_ID>/files/<FILENAME>.pdf&embedded=true" width="100%" height="600" style="border: 1px solid #dee2e6;"></iframe>
   ```
4. **Citation Section:**
   ```markdown
   ## Citation
   <Citation text including Zenodo DOI link>
   ```

### Practical page layout
Every practical/workshop file in [practicos](file:///C:/Users/corba/Documents/2026_TtT_Course/practicos) must follow this structure:

#### English & Español
1. **Quarto Frontmatter:**
   ```yaml
   ---
   title: "Version Control with Git and Environment Management with Pixi"
   author: "Mauro Silberberg"
   date: "04 August 2026"
   format: html
   ---
   ```
2. **Learning Objectives Callout:**
   ```markdown
   ::: {.callout-tip}
   ## Objetivos de Aprendizaje
   Al finalizar la sesión, los alumnos serán capaces de:
   - <objective_1>
   :::
   ```
3. **Prerequisites Section (Software, Data, and Knowledge):**
   ```markdown
   ## Prerequisitos
   ### Programas instalados
   - Git
   - Pixi
   ### Datos descargados
   - [Link a datos](<data_url>)
   ### Conocimientos previos
   - <prior_knowledge_requirements>
   ```
4. **GitHub Link to Workshop Section:**
   ```markdown
   ## Link al taller
   [Link al taller](<github_workshop_url>)
   ```
5. **Citation Section:**
   ```markdown
   ## Citation
   [Add citation here]
   ```

## Compact project snapshot
- Workshop name: **Taller de Fundamentos en Análisis de Bioimágenes (Formación de Formadores)**.
- Course type: Train-the-Trainer in Bioimage Analysis for LATAM.
- Confirmed course dates: **2026-08-03 to 2026-08-07**.
- Confirmed format: **on-site only**, with required pre-course lectures and in-person Q&A/pedagogy workshops.
- Working language: **English**.
- Confirmed classroom: **Aula 1306, Pabellón 0+Infinito, Facultad de Ciencias Exactas y Naturales**.
- Planned participant count: **24**.
- Main coordination areas: program, pre-course lectures/topics, invited professors, local instructor preparation, logistics, registration, budget, communications.
- Funding context from FUNDACEN materials: AR$ 10.004.000 requested for the broader proposal; only AR$ 2.000.000 is available for now, so priorities and allocation must be tracked explicitly.
- Main working document: `COURSE_MASTER_PLAN.md`.
- Folder plan exists conceptually but must **not** be created yet.
