# Smart Service

> Платформа реального времени для управления транспортной логистикой и координации бригад

---

<details open>
<summary>🇷🇺 Русский</summary>

### 🚀 Обзор

**Smart Service** — распределенная система для управления транспортом и координации полевых бригад в реальном времени.

Платформа объединяет веб-интерфейс диспетчера и Telegram-интерфейс исполнителей, обеспечивая непрерывное управление
задачами и синхронизацию статусов.

---

### 💡 Проблема

- отсутствие прозрачности загрузки транспорта
- неэффективное распределение задач
- отсутствие контроля этапов выполнения
- простой бригад и техники
- разрозненные каналы коммуникации

---

### ✅ Решение

Платформа из двух ключевых модулей:

**1. Модуль диспетчера (Web):**

- мониторинг транспорта
- назначение и планирование задач
- контроль выполнения
- визуализация загрузки

**2. Модуль исполнителя (Telegram / WebApp):**

- мгновенное получение задач
- принятие в работу
- пошаговое обновление статусов
- передача данных обратно в систему

---

### 🧩 Возможности

- контроль жизненного цикла задач в реальном времени
- двусторонняя коммуникация
- мобильный доступ через Telegram
- централизованный дашборд
- синхронизация состояния системы
- автоматические уведомления

---

### ⚙️ Технологии

**Backend:**  
Python, Django DRF

**Frontend:**  
React, TypeScript

**Интеграции:**  
Aiogram (Telegram Bot API), RabbitMQ

**Данные:**  
PostgreSQL, Redis

---

### 🏗️ Архитектура

```text
Диспетчер (Web)
        ↓
Backend (Django DRF)
        ↓
Очередь сообщений (RabbitMQ)
        ↓
Telegram Bot
        ↓
Исполнители
        ↓
Обновление статусов
        ↓
Dashboard
````

---

### Процесс работы

1. Диспетчер создает задачу
2. Исполнитель получает её в Telegram
3. Обновляет этапы выполнения
4. Статус мгновенно отображается в системе

---

### Результат

* повышение эффективности использования транспорта
* сокращение простоев
* прозрачность процессов
* ускорение координации

---

### Эффект

* снижение непроизводительного времени до **10%**

---

### Примечание

Проект представлен в обобщенном виде без раскрытия конфиденциального внутреннего содержимого.

</details>

---

<details>
<summary>🇬🇧 English</summary>

### 🚀 Overview

**Smart Service** is a distributed system for managing transport logistics and coordinating field crews in real time.

The platform integrates a dispatcher web interface with a Telegram-based execution layer, enabling seamless task
management and real-time synchronization.

---

### 💡 Problem

* lack of real-time visibility of transport availability
* inefficient task distribution
* no control over execution stages
* downtime of crews and equipment
* fragmented communication

---

### ✅ Solution

A system consisting of two modules:

**1. Dispatcher Module (Web):**

* fleet monitoring
* task assignment and scheduling
* execution tracking
* workload visualization

**2. Execution Module (Telegram / WebApp):**

* instant task delivery
* task acceptance
* step-by-step status updates
* feedback to dispatcher system

---

### 🧩 Key Features

* real-time task lifecycle tracking
* bidirectional communication
* mobile-first via Telegram
* centralized dashboard
* synchronized system state
* automated notifications

---

### ⚙️ Tech Stack

**Backend:**  
Python, Django DRF

**Frontend:**
React, TypeScript

**Messaging / Integration:**
Aiogram (Telegram Bot API), RabbitMQ

**Data / State:**
PostgreSQL, Redis

---

### 🏗️ Architecture

```text
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
Status Updates
        ↓
Dashboard
```

---

### Workflow

1. Dispatcher assigns a task
2. Worker receives it via Telegram
3. Updates execution stages
4. Status is synced in real time

---

### Value

* better transport utilization
* reduced downtime
* real-time visibility
* faster coordination

---

### Impact

* up to **10% reduction in non-productive time (NPT)**

---

### Notes

This project is presented in a generalized form without disclosing confidential internal content.

</details>