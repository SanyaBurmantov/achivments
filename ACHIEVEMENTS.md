# Достижения / Achievements

> Проект «Expert Journal» — SPA для ведения и учёта экспертиз (Vue 3, Vuetify, Pinia, Vite; бэкенд Django REST Framework).
> Project "Expert Journal" — SPA for managing and tracking expert examinations (Vue 3, Vuetify, Pinia, Vite; Django REST Framework backend).

---

## 🇷🇺 На русском

- Разработал клиентскую часть системы учёта экспертиз на Vue 3 + Vuetify: 35+ коммитов, более 80 затронутых модулей.
- Спроектировал и сверстал многошаговые мастера создания и редактирования экспертиз (4 шага), включая динамические формы полей на основе метаданных бэкенда.
- Реализовал универсальные компоненты вывода полей из метаданных (WwDetailFieldFromMeta, WwDetailInfoFieldFromMeta), что ускорило добавление новых разделов без правки шаблонов.
- Внедрил серверную пагинацию, хлебные крошки и навигацию по разделам, повысив удобство работы с большими списками экспертиз.
- Оптимизировал отрисовку крупных таблиц: устранил «тяжёлые» ячейки в пагинаторе и добавил состояния загрузки (лоадеры).
- Реализовал плавную загрузку и монтирование страниц (layout SmoothLoadedPage) для бесшовных переходов между разделами.
- Сверстал справочники и административные разделы: отделы и их структура, корреляции, коды, локации, группы специалистов, эксперты, аудит, настройки, отчёты.
- Реализовал экранные действия эксперта: создание, редактирование и детальный просмотр материалов, финализацию экспертиз.
- Разработал визуальный стиль приложения: единая цветовая схема, тени (box-shadow), стили в main.scss.

## 🇬🇧 In English

- Built the client side of an expert-examination tracking system with Vue 3 + Vuetify: 35+ commits across 80+ modules.
- Designed and implemented multi-step wizards (4 steps) for creating and editing examinations, including dynamic, metadata-driven form fields.
- Created reusable metadata-driven field components (WwDetailFieldFromMeta, WwDetailInfoFieldFromMeta), enabling new sections to be added without touching templates.
- Introduced server-side pagination, breadcrumbs, and section navigation, improving usability for large examination lists.
- Optimized rendering of large data tables: removed heavy cells in the paginator and added loading states (loaders).
- Implemented smooth page loading and mounting (SmoothLoadedPage layout) for seamless transitions between sections.
- Built reference and admin modules: departments and their structure, correlations, codes, locations, specialist groups, experts, audit log, settings, and reports.
- Delivered expert action screens: material create, update, and detail views, plus examination finalization.
- Established the application's visual style: unified color scheme, box shadows, and styles in main.scss.
