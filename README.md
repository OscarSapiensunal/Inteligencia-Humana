# Workshop 1 — Ingeniería de Software II

**Universidad Nacional de Colombia — Semestre 2026-II**
**Docente:** Eng. Liliana Marcela Olarte, M.Sc.
**Proyecto:** Plataforma web y móvil de tutorías académicas
**Fecha límite de entrega:** 30 de septiembre de 2026, 23:00

## Integrantes

- Camilo Alejandro Lagos Malaver — Desarrollador Backend
- Oscar Javier Saavedra Montero — Desarrollador Frontend
- Angel Palacio Suarez — Diseñador UX/UI
- Laura Alejandra Cadavid Mendoza — Desarrolladora Frontend / Mobile
- Brahian Camilo Gomez Carvajal — Gestor de proyecto / QA

## Descripción del proyecto

Plataforma web y móvil que conecta estudiantes que requieren apoyo académico con tutores especializados en determinadas materias o temas. Permite buscar tutores, solicitar y gestionar tutorías, calificar el servicio recibido y recibir recomendaciones de tutores mediante un servicio de inteligencia artificial (OpenRouter).

## Contenido de esta entrega

Este Workshop 1 corresponde a la fase de análisis del proyecto de curso y contiene:

1. Descripción general del sistema
2. Problema y objetivos
3. Alcance (incluido y excluido)
4. Actores del sistema
5. Requisitos funcionales (RF-01 a RF-29)
6. Requisitos no funcionales (RNF-01 a RNF-12)
7. Historias de usuario (HU-01 a HU-20) con criterios de aceptación Given/When/Then
8. Mapa de historias de usuario (User Story Mapping), representado como diagrama elaborado con Mermaid (Figura 1)
9. Priorización y releases (Release 1: MVP, Release 2: Operación y confianza, Release 3: Inteligencia y administración avanzada)
10. Trazabilidad de requisitos funcionales → historias de usuario → release
11. Stack tecnológico
12. Referencias

Todo el contenido detallado se encuentra en el archivo `Workshop-1.pdf` incluido en esta carpeta.

## Mapa de historias de usuario

Backbone horizontal con las 8 actividades del usuario; en vertical, las historias de cada actividad ordenadas por prioridad y separadas por release (verde: Release 1 — MVP, amarillo: Release 2, rojo: Release 3). El código fuente del diagrama está en `mapa-historias-usuario.mmd`.

```mermaid
block-beta
  columns 5
  H0["Actividades →"] A1["1. Cuenta y perfil"] A2["2. Gestión de tutor"] A3["3. Búsqueda y selección"] A4["4. Solicitud y programación"]
  R1["Release 1 — MVP"] c11["HU-01 Registro (Alta)<br/>HU-02 Perfil (Media)"] c12["HU-03 Materias (Alta)<br/>HU-05 Disponibilidad (Alta)<br/>HU-04 Experiencia (Media)"] c13["HU-06 Búsqueda (Alta)<br/>HU-07 Perfil tutor (Alta)"] c14["HU-08 Solicitud (Alta)<br/>HU-10 Aceptar/rechazar (Alta)<br/>HU-09 Notificación (Media)<br/>HU-11 Estado (Media)"]
  R2["Release 2 — Operación y confianza"] e21[" "] e22[" "] e23[" "] e24[" "]
  R3["Release 3 — IA y administración"] e31[" "] e32[" "] e33[" "] e34[" "]
  space:5
  H1["Actividades →"] A5["5. Ejecución y seguimiento"] A6["6. Evaluación y reseñas"] A7["7. Recomendación IA"] A8["8. Administración"]
  S1["Release 1 — MVP"] c15["HU-12 Tutorías programadas (Media)"] e16[" "] e17[" "] e18[" "]
  S2["Release 2 — Operación y confianza"] c25["HU-13 Cancelación (Media)"] c26["HU-14 Calificación (Alta)<br/>HU-15 Ver reseñas (Media)<br/>HU-16 Moderación (Baja)"] e27[" "] e28[" "]
  S3["Release 3 — IA y administración"] e35[" "] e36[" "] c37["HU-17 Recomendación IA (Media)"] c38["HU-18 Cuentas (Baja)<br/>HU-19 Materias (Baja)<br/>HU-20 Supervisión (Baja)"]
  classDef act fill:#9dc3e6,stroke:#1f4e79,stroke-width:2px,color:#000,font-weight:bold
  classDef rel fill:#d9d9d9,stroke:#595959,stroke-width:2px,color:#000,font-weight:bold
  classDef r1 fill:#d4edda,stroke:#28a745,color:#000
  classDef r2 fill:#fff3cd,stroke:#d39e00,color:#000
  classDef r3 fill:#f8d7da,stroke:#c82333,color:#000
  classDef empty fill:#fafafa,stroke:#ddd
  class A1,A2,A3,A4,A5,A6,A7,A8,H0,H1 act
  class R1,R2,R3,S1,S2,S3 rel
  class c11,c12,c13,c14,c15 r1
  class c25,c26 r2
  class c37,c38 r3
  class e16,e17,e18,e21,e22,e23,e24,e27,e28,e31,e32,e33,e34,e35,e36 empty
```

## Estructura sugerida en el repositorio

```
Workshop-1/
├── README.md
├── Workshop-1.pdf
└── mapa-historias-usuario.mmd
```

## Stack tecnológico

- Frontend web: React
- Aplicación móvil: Expo
- Backend: Django
- Base de datos: MySQL
- Inteligencia artificial: OpenRouter

## Documento fuente

El documento editable (Google Docs) del cual se exporta `Workshop-1.pdf` se encuentra en:
https://docs.google.com/document/d/1RLOBo4HdvkvIJJ2SXF_64cJODejhgisVgqAobpvDnnc/edit
