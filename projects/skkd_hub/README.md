# Digital Services Platform / Платформа цифровых решений

<details open>
<summary>🇷🇺 Русский</summary>

> Внутренняя монорепа-платформа для промышленных веб-приложений с общим UI, аутентификацией и переиспользуемыми модулями

## Обзор

Платформа объединила несколько независимых сервисов в единую систему с общими архитектурными и UI-принципами, централизованной аутентификацией и переиспользуемыми компонентами.

## Проблема → Решение

| Проблема | Решение |
|---|---|
| Дублирование UI и бизнес-логики | Общая дизайн-система и переиспользуемые компоненты |
| Разрозненная аутентификация | Централизованная auth с ролевой моделью |
| Неоднородный UX | Единый Digital Services Hub как точка входа |
| Медленный запуск новых сервисов | Готовая платформенная основа для новых модулей |

## Структура платформы

### 1. Digital Services Hub
Центральная точка входа: каталог приложений, управление доступами, единый профиль пользователя, общая навигация.

### 2. Сервис расчёта раствора глушения
Инженерный сервис: автоматические расчёты, загрузка данных, генерация отчётов, прозрачная логика формул.

### 3. Сервис обустройства цехов
Визуальная система: интерактивный canvas, управление объектами, визуализация схем, история изменений.

## Архитектура

```
Пользователи
    ↓
Digital Services Hub
    ├── Аутентификация / роли
    ├── Дизайн-система
    ├── Layout / навигация
    └── Каталог сервисов
            ↓
    ┌───────────────────┬──────────────────┐
    │                   │                  │
Сервис глушения   Обустройство цехов   Новые модули
    │                   │
FastAPI + PostgreSQL  FastAPI + PostgreSQL
```

## Стек

| Слой | Технологии |
|---|---|
| Frontend | React, TypeScript, Vite, styled-components, Konva |
| Backend | Python, FastAPI, SQLAlchemy, Pandas |
| Database | PostgreSQL |
| Architecture | Monorepo, shared design system, centralized auth |

## Результат

- Переход от разрозненных сервисов к единой платформе
- Снижение дублирования во frontend и backend
- Унификация пользовательского опыта
- Ускорение разработки новых сервисов

## Скриншоты

### Hub

<p align="center">
  <a href="./assets/hub-main.png"><img src="./assets/hub-main.png" width="45%" /></a>
  <a href="./assets/hub-access.png"><img src="./assets/hub-access.png" width="45%" /></a>
</p>

### Сервис глушения

<p align="center">
  <a href="./assets/jamsheet-main.png"><img src="./assets/jamsheet-main.png" width="45%" /></a>
  <a href="./assets/jamsheet-formula.png"><img src="./assets/jamsheet-formula.png" width="45%" /></a>
</p>

### Обустройство цехов

<p align="center">
  <a href="./assets/field-control-main.png"><img src="./assets/field-control-main.png" width="45%" /></a>
  <a href="./assets/field-control-objects.png"><img src="./assets/field-control-objects.png" width="45%" /></a>
</p>

---

*Проект представлен в обобщённом виде без раскрытия конфиденциального внутреннего содержимого.*

</details>

---

<details>
<summary>🇬🇧 English</summary>

> Internal monorepo platform for industrial web applications with shared UI, authentication, and reusable modules

## Overview

The platform consolidated several independent services into a unified system with shared architectural and UI principles, centralized authentication, and reusable components.

## Problem → Solution

| Problem | Solution |
|---|---|
| Duplicated UI and business logic | Shared design system and reusable components |
| Fragmented authentication | Centralized auth with role-based access |
| Inconsistent UX | Unified Digital Services Hub as single entry point |
| Slow delivery of new internal tools | Ready-made platform foundation for new modules |

## Platform Structure

### 1. Digital Services Hub
Central entry point: app catalog, access management, unified user profile, shared navigation.

### 2. Well Killing Calculation Service
Engineering service: automated calculations, data integration, report generation, transparent formula logic.

### 3. Field Infrastructure Control Service
Visual management system: interactive canvas, object management, infrastructure visualization, change history.

## Architecture

```
Users
  ↓
Digital Services Hub
  ├── Auth / roles
  ├── Design system
  ├── Layout / navigation
  └── App catalog
          ↓
  ┌───────────────────┬──────────────────┐
  │                   │                  │
Well Killing     Infrastructure     Future Modules
Service          Control
  │                   │
FastAPI + PostgreSQL  FastAPI + PostgreSQL
```

## Tech Stack

| Layer | Technologies |
|---|---|
| Frontend | React, TypeScript, Vite, styled-components, Konva |
| Backend | Python, FastAPI, SQLAlchemy, Pandas |
| Database | PostgreSQL |
| Architecture | Monorepo, shared design system, centralized auth |

## Impact

- Transformed separate tools into a unified platform
- Reduced duplication across frontend and backend
- Consistent user experience across all services
- Faster development of new modules

## Screenshots

### Hub

<p align="center">
  <a href="./assets/hub-main.png"><img src="./assets/hub-main.png" width="45%" /></a>
  <a href="./assets/hub-access.png"><img src="./assets/hub-access.png" width="45%" /></a>
</p>

### Well Killing Service

<p align="center">
  <a href="./assets/jamsheet-main.png"><img src="./assets/jamsheet-main.png" width="45%" /></a>
  <a href="./assets/jamsheet-formula.png"><img src="./assets/jamsheet-formula.png" width="45%" /></a>
</p>

### Infrastructure Control

<p align="center">
  <a href="./assets/field-control-main.png"><img src="./assets/field-control-main.png" width="45%" /></a>
  <a href="./assets/field-control-objects.png"><img src="./assets/field-control-objects.png" width="45%" /></a>
</p>

---

*This project is presented in a generalized form without disclosing confidential internal content.*

</details>