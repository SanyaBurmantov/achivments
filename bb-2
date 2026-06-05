# Достижения по проекту (для резюме)

Внутренняя корпоративная система управления проектами и трудовыми ресурсами
(ERP-типа): учёт трудозатрат и интенсивности труда, проекты и задачи, совещания,
реестр договоров, проблемные запросы, кадровый учёт (отпуска, переработки,
отсутствия), дашборды руководителя, администрирование (пользователи, роли,
документы), выдача VPN-сертификатов.

**Роль:** единственный / ведущий frontend-разработчик. Спроектировал архитектуру
клиентской части и реализовал весь актуальный код фронтенда.

**Стек:** Vue 3 (Composition API), Vuetify 3, Pinia, Vue Router, Vite, Axios
(+ axios-auth-refresh), date-fns, SCSS/Sass.

---

## Краткое summary (1 абзац — в шапку резюме)

Единолично разработал фронтенд корпоративной ERP-системы на Vue 3 (Composition
API) + Vuetify 3 + Pinia + Vue Router. Спроектировал масштабируемую архитектуру
SPA и собственную библиотеку переиспользуемых UI-компонентов (универсальные
таблицы с фильтрацией, сортировкой и пагинацией, динамические формы и поля),
за счёт чего новые CRUD-разделы собираются из готовых блоков с минимумом кода.
Реализовал слой работы с REST API с JWT-авторизацией и прозрачным авто-refresh
токенов, а также 9+ функциональных модулей: учёт трудозатрат, проекты/задачи,
совещания, реестр договоров, кадровый учёт и аналитические дашборды.

---

## Ключевые достижения (готовые буллеты)

### Архитектура и переиспользование
- Спроектировал архитектуру SPA с нуля: разделение на views / переиспользуемые
  UI-компоненты / composables / слой API / Pinia-сторы — единый подход на всём
  проекте (~175 Vue-компонентов).
- Разработал библиотеку из 20+ обёрток над полями ввода (`B*`-компоненты:
  автокомплиты, селекты с «выбрать всё», даты/месяцы/годы, числа/цены, файлы,
  textarea с «показать ещё» и т.д.) — единый UX и валидация форм во всём приложении.
- Вынес повторяющуюся логику в composables (`useTableList`, `useForm`,
  `useCompareData`, `useSortByField`, `useTabs`, `useMeta`, `useExpandableProjects`
  и др.) — новые списки и формы подключаются несколькими строками.

### Универсальные таблицы и формы
- Реализовал универсальный компонент таблицы (`WwTable`) с server-side
  пагинацией, сортировкой и фильтрацией, синхронизированными с query-параметрами
  URL (состояние таблицы шарится по ссылке и переживает перезагрузку страницы).
- Построил generic CRUD-диалоги (create / update / detail / delete), работающие
  поверх единого описания полей — добавление нового справочника не требует
  написания форм вручную.
- Сделал систему фильтров (`FilterLayout`, типизированные поля фильтров:
  автокомплит, дата, месяц, год) с переиспользуемой конфигурацией.

### Слой API и авторизация
- Спроектировал слой работы с REST API (20+ api-модулей) на Axios с
  интерсепторами: автоподстановка Bearer-токена, централизованная обработка
  ошибок и тостовые уведомления.
- Внедрил прозрачное обновление JWT через axios-auth-refresh: при 401 токен
  тихо рефрешится и исходный запрос повторяется; при неуспехе — авто-логаут и
  редирект на логин. Пользователь не теряет контекст.

### Функциональные модули (реализованы единолично)
- **Учёт трудозатрат / интенсивность труда** — таблицы по дням/месяцам,
  агрегации, детализация.
- **Проекты и задачи** — древовидные проекты с разворачиваемыми подпроектами
  (ленивая подгрузка и кеширование вложенности), этапы, документация.
- **Совещания и поручения** — создание/редактирование, формы с динамическими
  данными.
- **Реестр договоров**, **проблемные запросы**.
- **Кадровый учёт** — отпуска, переработки, отсутствия, сводка трудозатрат.
- **Дашборды руководителя** — задачи, этапы, совещания, дни рождения,
  отсутствия с цветовой индикацией статусов.
- **Администрирование** — пользователи, роли (ролевая модель доступа),
  документы; выдача VPN-сертификатов с асинхронным поллингом статуса.

### Производительность и UX
- Ленивая загрузка и кеширование вложенных данных (подпроекты) — меньше запросов
  и быстрее отрисовка больших деревьев.
- Состояние списков (фильтры/страница/сортировка) в URL — шаринг ссылок и
  корректная работа «назад/вперёд» в браузере.
- Загрузка файлов через dropzone с авто-аплоадом и поддержкой множественной
  загрузки.

### Качество и процессы
- Настроил линтинг (ESLint + eslint-plugin-vue) и pre-commit хуки (husky) —
  единый стиль кода и защита от «грязных» коммитов.
- Сборка и dev-окружение на Vite; интеграция в GitLab CI.

---

## Варианты формулировок под разный объём резюме

**Одна строка:**
> Единолично разработал фронтенд корпоративной ERP-системы на Vue 3, Vuetify 3,
> Pinia и Vue Router, включая собственную библиотеку UI-компонентов и слой API
> с JWT-авторизацией.

**Два-три буллета:**
> - Спроектировал и реализовал с нуля SPA внутренней системы управления проектами
>   и ресурсами (Vue 3 / Vuetify 3 / Pinia / Vite), ~175 компонентов.
> - Разработал переиспользуемую UI-библиотеку (универсальные таблицы с
>   фильтрацией/пагинацией, динамические формы, поля), ускорив сборку новых разделов.
> - Внедрил слой REST API с JWT и прозрачным авто-refresh токенов, ролевую модель
>   доступа и аналитические дашборды руководителя.

---

## Что сказать на собеседовании (talking points)

- Почему вынес логику в composables и универсальные таблицы/формы — какую боль
  это убрало (дублирование, скорость добавления разделов).
- Как устроен авто-refresh токенов и почему пользователь не теряет контекст.
- Синхронизация состояния таблицы с URL — зачем и как.
- Ленивая загрузка + кеш для дерева проектов — какой эффект на запросы/скорость.

> Примечание: в git-истории есть коммиты других участников, но актуальный код
> фронтенда — твой (вклад остальных переписан/удалён). Бэкенд писал отдельный
> разработчик — это честно отражает «ведущий/единственный frontend».

---

# English version (for resume)

## Summary (1 paragraph)

Sole frontend developer of an internal corporate ERP-style system for project and
workforce management. Designed the SPA architecture from scratch and built a
custom reusable UI component library (generic data tables with server-side
filtering, sorting and pagination; dynamic forms and field components) on Vue 3
(Composition API), Vuetify 3, Pinia and Vue Router. Implemented a REST API layer
with JWT auth and transparent token auto-refresh, plus 9+ functional modules
including labor-cost tracking, projects/tasks, meetings, contract registry, HR
records and management dashboards (~175 components).

## Key achievements (bullets)

- Architected and built from scratch the SPA of an internal project/resource
  management system (Vue 3 / Vuetify 3 / Pinia / Vite), ~175 components, with a
  clean split between views, reusable UI, composables, API layer and Pinia stores.
- Developed a reusable UI library: a generic data-table component with server-side
  pagination, sorting and filtering synced to URL query params, plus 20+ form-field
  wrappers and generic CRUD dialogs (create/update/detail/delete) — new sections
  are assembled from ready-made blocks with minimal code.
- Extracted shared logic into composables (`useTableList`, `useForm`,
  `useCompareData`, `useTabs`, etc.), drastically cutting duplication and speeding
  up delivery of new list/form screens.
- Built the REST API layer (20+ API modules) on Axios with request/response
  interceptors: automatic Bearer-token injection, centralized error handling with
  toast notifications.
- Implemented transparent JWT refresh via axios-auth-refresh: on 401 the token is
  silently refreshed and the original request retried; on failure the user is
  logged out and redirected — without losing context.
- Delivered 9+ functional modules end-to-end: labor-cost / work-intensity
  tracking, tree-structured projects with lazily loaded & cached sub-projects,
  tasks, meetings, contract registry, problem requests, HR records (vacations,
  overtime, absences), role-based admin (users/roles/documents), VPN-certificate
  issuance with async status polling, and management dashboards.
- Set up tooling and code quality: ESLint (+ eslint-plugin-vue), husky pre-commit
  hooks, Vite build, GitLab CI integration.

## Short variants

**One line:**
> Sole frontend developer of a corporate ERP-style SPA (Vue 3, Vuetify 3, Pinia,
> Vue Router) — built a reusable UI component library and a JWT-authenticated REST
> API layer.

**Two-three bullets:**
> - Designed and built from scratch the SPA of an internal project/resource
>   management system (Vue 3 / Vuetify 3 / Pinia / Vite), ~175 components.
> - Created a reusable UI library (generic tables with filtering/pagination,
>   dynamic forms and fields), accelerating delivery of new sections.
> - Implemented a REST API layer with JWT and transparent token auto-refresh,
>   role-based access control and management dashboards.
