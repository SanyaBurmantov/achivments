# Resume — Frontend Developer (Vue.js), Middle+

> Draft. Replace [...] placeholders with your data. Technical facts and module
> breakdown come from real code; role wording is honest (see note at the end).

---

**[Full Name]**
Frontend Developer (Vue.js) · Middle+ · Belarus
Email: [email] · Telegram: [@username] · GitHub/GitLab: [link] · LinkedIn: [link]

---

## Summary

Frontend developer with deep specialization in the Vue 3 ecosystem. ~1.5 years
designing and developing large corporate web applications (ERP, government and
industry information systems). I run one of the systems as the sole frontend
developer — from SPA architecture to production and maintenance — while
contributing frontend work to 4-5 other team projects in parallel.

Strengths: designing reusable architecture (composables, generic tables,
metadata-driven dynamic forms), clean REST API layers, and shipping features
end-to-end under high parallel load. Experienced working alongside a Django
backend and in a shared codebase with other developers. Growing my TypeScript
(already used on newer projects) and automated testing skills.

---

## Key Skills

**Core:** JavaScript (ES6+), TypeScript, HTML5, CSS3 / SCSS (Sass), markup from Figma designs

**Vue stack:** Vue 3 (Composition API, `<script setup>`), Vuetify 3, Pinia,
Vue Router, Vite, reactivity, custom composables, component architecture,
reusable UI library design

**Data & APIs:** REST API, Axios (request/response interceptors, centralized
error handling), JWT auth with transparent token auto-refresh, server-side
pagination / sorting / filtering, metadata-driven dynamic forms and filters,
file uploads (dropzone, multi-upload, auto-upload), async status polling

**Architecture & patterns:** logic extraction into composables, generic CRUD
dialogs, URL-synced list state (query params), role-based access control
(permission matrix), Pinia state management, persisted UI state (local/session storage),
Feature-Sliced Design (FSD)

**Testing:** Vitest, unit tests for components and logic (used on newer projects)

**Tooling & process:** Git / GitLab, GitLab CI, ESLint (+ eslint-plugin-vue),
Husky (pre-commit hooks), code review, shared-codebase workflow (branching,
conflict resolution, shared code style)

**Backend context:** confident working against Django / Python REST APIs

**Growing:** TypeScript (in depth), Playwright (e2e), expanding test coverage

---

## Technical Highlights

- **Designed a reusable UI library** the whole app is built on: a generic data
  table with server-side pagination, sorting and filtering (state synced to URL —
  lists are shareable via link and survive a reload), generic CRUD dialogs
  (create / update / detail / delete), and 20+ form-field wrappers with unified
  UX and validation.
- **Built metadata-driven dynamic forms and filters** (`useMeta` composable +
  a universal form): field and filter structure comes from the backend and the
  frontend assembles the form automatically — adding a new reference entity needs
  almost no manual form markup.
- **Extracted shared logic into a composables library**: list handling
  (`useTableList`), forms with server-side validation (`useForm`), form dirty-checking
  (`useCompareData`), sorting (`useSortByField`), persisted tabs (`useTabs`),
  work-time calculations on `date-fns` (`useTodayWorkTime`), etc. — new screens
  are wired up in a few lines.
- **Implemented the REST API layer on Axios** with interceptors: automatic
  Bearer-token injection, centralized error handling with toast notifications,
  and transparent JWT refresh (on 401 the token is silently refreshed and the
  original request retried; on failure, auto-logout without losing context).
- **Optimized work with the project tree** — lazy loading and caching of nested
  sub-projects, reducing the number of requests and speeding up rendering of
  large structures.
- **Set up engineering hygiene** — ESLint, pre-commit hooks (Husky), GitLab CI.

---

## Experience

### Frontend Developer · [Company / WiseWeb] · 2025 — present

Building corporate and government web applications in a product team. Running
several projects in parallel. Frontend on Vue 3 + Vuetify 3 + Pinia + Vite,
backends on Django/Python, workflow on GitLab + CI.

---

#### Corporate ERP system for project & workforce management
*Lead / sole frontend developer · SPA, ~175 components*

Internal system for managing the company's projects, tasks and staff. Designed
the frontend architecture from scratch and implemented all functional modules:

- **Labor-cost & work-intensity tracking** — labor costs by employee and project,
  intensity breakdowns, daily/monthly views, work-time editing, monthly and
  period summary reports.
- **Projects, stages & documentation** — tree-structured projects with lazily
  loaded & cached sub-projects, stage management, project documentation with
  work/report material tabs.
- **Tasks** — task lists, task activities, task uploads, per-user activity tracking.
- **Meetings & assignments** — create / edit / detail views with dynamic forms.
- **HR records** — vacations (calendar, remaining days, requests), overtime
  (daily and monthly), absences (monthly and period, reports).
- **Management dashboards** — tasks, stages, meetings & assignments, birthdays,
  daily and monthly absences with color-coded status indication.
- **Contract registry** and **problem requests**.
- **Administration** — users (including VPN-certificate issuance with async status
  polling), roles with a permission matrix (RBAC), reference dictionaries
  (organizations, positions, document types, contracts & amendments, standard
  working hours and days off).
- **Authentication** — login, JWT, password change.

*Stack: Vue 3 (Composition API), Vuetify 3, Pinia, Vue Router, Vite, Axios.*

---

Alongside the flagship, ran the frontend part of five more projects in parallel,
in a shared codebase with other developers. Maintained and propagated shared
reusable components (generic tables, form fields, filters) between projects.

---

#### Government DNA-examination & DNA-database system
*Frontend developer in a team · one of the key frontend contributors*

Information system for managing DNA examinations, tracking research objects and
reconciling data. Implemented a significant part of the frontend:

- **Examination journal** — research tables and cards, genotype information,
  data on examination objects and subjects.
- **Research object cards** — list, detail view, creation form, entering and
  editing examination results.
- **Verification & data-reconciliation module** — object tabs, result processing,
  send-for-revision, multi-step verification flow.
- **Match notifications**, **DNA data banks**, examination-module routing, navigation.
- Maintained the shared generic-table component.

*Scope: ~270 commits, ~12,000 lines of code (2025–2026). Stack: Vue 3, Vuetify 3, Pinia, Vite, Axios.*

---

#### Educational admin system for tracking academic works
*Frontend developer in a team · Vue 3 + TypeScript*

Admin panel for tracking academic/coursework and student testing.

- **Academic-works module** — multi-step create/edit wizards (settings, student
  data, stages), detail view, work settings.
- **Grading systems**, stage and step management.
- **Uploads** — adding participants and documents to a work.
- **Testing module** — settings, student lists in tests, cards.
- Sidebar navigation; maintained shared table and form-field components.

*Scope: ~310 commits, ~20,000 lines of code (2025–2026). Stack: Vue 3, Vuetify 3, Pinia, TypeScript, Vite.*

---

#### Forensic-examination tracking system
*Frontend developer in a team*

- **Multi-step examination create/edit wizards** (4 steps).
- **Department directory** — lists, org structure, correlations.
- **Logistics & equipment** — specialist groups, methodologies, equipment.
- Library, experts, examination packages and reporting sections; base app setup
  (smooth-loading layout).

*Scope: ~35 commits (2025–2026). Stack: Vue 3, Vuetify 3, Pinia, Vite.*

---

#### Normative-legal-document drafting system
*Frontend developer in a team*

- **Normative-document cards** — creation, motion and accompanying documents,
  registration, merging.
- **Plans & events** — forms, create/edit, tables.
- Statements, simplified interface, reference sections; table component.

*Scope: ~90 commits (2025–2026). Stack: Vue 3, Vuetify 3, Pinia, Vite.*

---

#### New information system (Vue 3 + TypeScript, Feature-Sliced Design)
*Frontend developer in a team · modern stack*

A greenfield project on a current architecture — where I apply the latest practices:

- **Feature-Sliced Design** (app / entities / widgets / pages / shared) on full **TypeScript**.
- **Objects & organizations CRUD** — pages, forms, contacts; entities with
  api / model / types layers; authentication.
- Typed HTTP layer and routing, Vuetify provider.
- **Unit tests with Vitest** (form fields, server-error handling).

*Scope: ~18 commits (greenfield, active stage, 2026). Stack: Vue 3, TypeScript, Pinia, Vuetify, Vite, Vitest, FSD.*

---

Typical work across all team projects: list and form UIs, multi-step wizards,
filters, REST API integration, authentication, merge-conflict resolution, code
review, shared code style, GitLab CI.

---

## Side Projects *(demonstrating end-to-end solo capability)*

- **E-commerce / online stores** — independently built Vue 3 frontends: catalogs,
  cart, markup from designs, API integration.
- **Service projects & API utilities** — small full-stack/service projects where
  I owned everything (REST APIs, integrations, automation).

---

## Education

[Institution, degree, years] *(or courses / self-education)*

## Languages

Russian — native · English — [level, e.g. B1 — technical documentation]

---

> **Honesty note on wording:** "designed / built / led" refers to the flagship
> ERP system, where the frontend is entirely mine. On team projects I owned my
> part of the frontend — reflected by "developed frontend features in a team".
