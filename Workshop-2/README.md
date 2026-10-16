# Workshop 2 — Design Artifacts and System Modeling

**Software Engineering II — Universidad Nacional de Colombia — Semester 2026-II**
**Lecturers:** Eng. Liliana Marcela Olarte, M.Sc. · Carlos Andrés Sierra, M.Sc.
**Project:** Web and mobile academic tutoring platform (Inteligencia Humana)

## Team

- Camilo Alejandro Lagos Malaver
- Oscar Javier Saavedra Montero
- Angel Palacio Suarez
- Laura Alejandra Cadavid Mendoza
- Brahian Camilo Gomez Carvajal

## Deliverable

All the design artifacts of this workshop are compiled in a single PDF: [`Workshop-2.1.pdf`](./Workshop-2.1.pdf).

## Contents

| # | Section | Where | Summary |
|---|---------|-------|---------|
| 1 | System domain | PDF, page 1 | System context (request-based flow: a student publishes a tutoring request, tutors apply, the student picks one application and the session is scheduled), scope, actor characterization (Student, Tutor) and business rules BR-01 to BR-10. |
| 2 | CRC cards | PDF, page 2 | One card per core class — `Estudiante`, `PerfilTutor`, `SolicitudTutoria`, `Postulacion`, `Tutoria` — with its responsibilities and collaborators. |
| 3 | Class diagram | PDF, page 3 | UML class diagram of the five core classes with attributes, methods, multiplicities, the composition `Estudiante ◆— PerfilTutor`, the supporting enumerations and the rules applied when a session is confirmed. |
| 4 | Relational database model | PDF, page 4 | MySQL schema normalized to 3NF in crow's-foot notation: tables, primary/foreign/unique keys, indexes, enumerations, business rules and the class-diagram → table mapping. |
| 5 | Mockups | PDF, page 5 | Mobile wireframes: sign-up, interest selection, mentor and learner views, create/edit tutoring, and screens to check confirmed and pending sessions and reviews. |
| 6 | Business model processes (BPMN / activity diagram) | Pending | Not included in the current version of the PDF. |
| 7 | Architecture diagram | Pending | Not included in the current version of the PDF. |

## Repository structure

```
Workshop-2/
├── README.md
└── Workshop-2.1.pdf
```

## References and tools

- UML class diagrams overview — https://www.uml-diagrams.org/class-diagrams-overview.html
- What is BPMN — https://www.visual-paradigm.com/guide/bpmn/what-is-bpmn/
- How to draw architectural diagrams — https://www.lucidchart.com/blog/how-to-draw-architectural-diagrams

### Use of AI

**Claude** (Anthropic) was used to support the planning and structuring of the diagrams (CRC cards, class diagram, relational database model and the other design models). All outputs were reviewed, adjusted and validated by the team.
