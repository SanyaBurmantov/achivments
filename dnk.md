# Frontend Developer — Достижения

**Проект:** информационная система ДНК-банка для судебно-генетических экспертиз
(учёт генотипов, аллелей, локусов, аутосомной и митохондриальной ДНК, журналы
экспертиз, сверка и верификация результатов).

**Стек:** Vue 3 (Composition API), Vuetify 3, Pinia, Vue Router, Vite, Axios.

**Масштаб вклада:** ~90 компонентов, 18+ переиспользуемых composables,
клиентская ролевая модель прав, тёмная/светлая темы. 1.5 года, 300+ коммитов.

---

## Ключевые достижения

- **Спроектировал механизм каскадного сохранения сложных форм** (родитель →
  дочерние компоненты) на Pinia через паттерн pub/sub: дочерние формы
  подписываются по ключу и сохраняются единым триггером с родителя. Снизил
  связность компонентов в самом нагруженном модуле — форме экспертизы.

- **Разработал библиотеку из 18+ Vue 3 composables** (работа с формами,
  сравнение данных при сверке, табличные списки с пагинацией, состояние табов,
  синхронизация с local/session storage), что устранило дублирование логики
  в проекте из ~90 компонентов и ускорило разработку новых экранов.

- **Создал переиспользуемый компонент таблицы** с серверной пагинацией,
  настраиваемым размером страницы, поиском, индикаторами загрузки и диалогами
  управления записями — базовый строительный блок для всех журналов системы.

- **Реализовал ввод и редактирование генотипов** для аутосомной и
  митохондриальной ДНК (включая работу со смесями и порядком локусов);
  оптимизировал ввод и редактирование больших наборов данных.

- **Разработал модуль сверки и верификации результатов экспертиз:** модальные
  окна сравнения, мульти-верификация, автоматическая подсветка расхождений
  между объектами.

- **Внедрил ролевую модель прав доступа на клиенте** — разграничение доступа
  к разделам и действиям в зависимости от роли пользователя.

- **Реализовал систему тем оформления** (светлая/тёмная) и клиентскую
  авторизацию с автоматическим обновлением токенов.

---

## Краткая версия (3 строки для резюме)

- Спроектировал на Pinia механизм каскадного сохранения сложных форм
  (родитель→дочерние) через pub/sub, снизив связность компонентов.
- Разработал библиотеку из 18+ Vue 3 composables и переиспользуемый компонент
  таблиц, устранив дублирование кода в проекте из ~90 компонентов.
- Реализовал доменную логику работы с ДНК-генотипами, модуль верификации
  результатов и клиентскую ролевую модель прав доступа.

---
---

# Frontend Developer — Achievements (EN)

**Project:** information system for a forensic DNA bank — management of DNA
genotypes, alleles, loci, autosomal and mitochondrial DNA, expertise journals,
and cross-verification of analysis results.

**Stack:** Vue 3 (Composition API), Vuetify 3, Pinia, Vue Router, Vite, Axios.

**Scope:** ~90 components, 18+ reusable composables, client-side role-based
access control, light/dark theming. 1.5 years, 300+ commits.

---

## Key achievements

- **Designed a cascading save mechanism for complex forms** (parent → child
  components) on top of Pinia using a pub/sub pattern: child forms subscribe by
  key and are persisted by a single trigger from the parent. Reduced component
  coupling in the system's most demanding module — the expertise form.

- **Built a library of 18+ Vue 3 composables** (form handling, data comparison
  for verification, paginated table lists, tab state, local/session storage
  sync), eliminating duplicated logic across a ~90-component codebase and
  speeding up development of new screens.

- **Created a reusable data table component** with server-side pagination,
  configurable page size, search, loading indicators, and record-management
  dialogs — the foundational building block for every journal in the system.

- **Implemented DNA genotype entry and editing** for autosomal and
  mitochondrial DNA (including mixtures and locus ordering); optimized entry and
  editing of large datasets.

- **Developed the results verification module:** comparison modals,
  multi-verification, and automatic highlighting of discrepancies between
  objects.

- **Introduced client-side role-based access control** — gating sections and
  actions based on the user's role.

- **Implemented theming** (light/dark) and authentication with automatic token
  refresh.

---

## Short version (3 lines for a CV)

- Designed a Pinia-based cascading save mechanism for complex parent→child forms
  via pub/sub, reducing component coupling.
- Built a library of 18+ Vue 3 composables and a reusable data-table component,
  eliminating code duplication across a ~90-component codebase.
- Implemented DNA genotype domain logic, a results-verification module, and
  client-side role-based access control.
