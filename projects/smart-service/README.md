# Smart Service

<details open>
<summary>🇷🇺 Русский</summary>

> Платформа реального времени для управления транспортной логистикой и координации бригад

## Обзор

Распределённая система, объединяющая веб-интерфейс диспетчера и Telegram-интерфейс исполнителей для непрерывного управления задачами и синхронизации статусов в реальном времени.

## Проблема → Решение

| Проблема | Решение |
|---|---|
| Нет прозрачности загрузки транспорта | Централизованный дашборд с мониторингом флота |
| Неэффективное распределение задач | Назначение и планирование в единой системе |
| Разрозненные каналы коммуникации | Единый поток: веб-диспетчер ↔ Telegram-исполнитель |
| Простой бригад и техники | Реальное время статусов и автоуведомления |

## Как это работает

```
1. Диспетчер создаёт задачу (Web)
2. Исполнитель получает её в Telegram
3. Обновляет этапы выполнения
4. Статус мгновенно отображается в системе
```

## Модули

**Модуль диспетчера (Web)**
— мониторинг транспорта, назначение задач, контроль выполнения, визуализация загрузки

**Модуль исполнителя (Telegram / WebApp)**
— получение задач, принятие в работу, пошаговые статусы, обратная связь

## Архитектура

```
Диспетчер (Web)
    ↓
Backend (Django DRF)
    ↓
Message Broker (RabbitMQ)
    ↓
Telegram Bot (Aiogram)
    ↓
Исполнители
    ↓
Обновление статусов → Dashboard
```

## Стек

| Слой | Технологии |
|---|---|
| Backend | Python, Django DRF |
| Frontend | React, TypeScript |
| Messaging | RabbitMQ, Aiogram (Telegram Bot API) |
| Database | PostgreSQL, Redis |

## Результат

- Снижение непроизводительного времени до **10%**
- Повышение эффективности использования транспорта
- Прозрачность процессов и ускорение координации

---

*Проект представлен в обобщённом виде без раскрытия конфиденциального внутреннего содержимого.*

</details>

---

<details>
<summary>🇬🇧 English</summary>

> Real-time platform for transport logistics management and crew coordination

## Overview

A distributed system combining a dispatcher web interface with a Telegram-based execution layer for seamless task management and real-time status synchronization.

## Problem → Solution

| Problem | Solution |
|---|---|
| No real-time transport visibility | Centralized dashboard with fleet monitoring |
| Inefficient task distribution | Unified task assignment and scheduling |
| Fragmented communication channels | Single flow: web dispatcher ↔ Telegram worker |
| Crew and equipment downtime | Real-time status tracking and auto-notifications |

## How It Works

```
1. Dispatcher assigns a task (Web)
2. Worker receives it via Telegram
3. Updates execution stages step by step
4. Status is synced in real time to the dashboard
```

## Modules

**Dispatcher Module (Web)**
— fleet monitoring, task assignment, execution tracking, workload visualization

**Execution Module (Telegram / WebApp)**
— task receipt, acceptance, step-by-step status updates, feedback loop

## Architecture

```
Dispatcher (Web UI)
    ↓
Backend API (Django DRF)
    ↓
Message Broker (RabbitMQ)
    ↓
Telegram Bot (Aiogram)
    ↓
Field Workers
    ↓
Status Updates → Dashboard
```

## Tech Stack

| Layer | Technologies |
|---|---|
| Backend | Python, Django DRF |
| Frontend | React, TypeScript |
| Messaging | RabbitMQ, Aiogram (Telegram Bot API) |
| Database | PostgreSQL, Redis |

## Impact

- Up to **10% reduction in non-productive time (NPT)**
- Improved transport utilization
- Real-time process visibility and faster coordination

---

*This project is presented in a generalized form without disclosing confidential internal content.*

</details>