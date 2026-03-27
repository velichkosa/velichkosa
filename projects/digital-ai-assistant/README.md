# Цифровой помощник (AI-ассистент)

> Production-ready AI система для автоматизации рабочих процессов с использованием LLM и мультиагентной архитектуры

---

<details open>
<summary>🇷🇺 Русский</summary>

### 🚀 Обзор

Цифровой AI-ассистент — это платформа для автоматизации работы с документами, таблицами и базами данных через
естественный язык.

Система объединяет LLM, RAG и мультиагентную архитектуру, позволяя пользователям взаимодействовать с данными без
необходимости писать код или SQL.

---

### 💡 Проблема

- работа с данными требует технических навыков
- ручной анализ документов занимает много времени
- сложно быстро получить ответы из разрозненных источников
- высокий порог входа для бизнес-пользователей

---

### ✅ Решение

Интеллектуальный ассистент, который:

- понимает запросы на естественном языке
- работает с документами (PDF, Excel, текст)
- генерирует SQL-запросы
- агрегирует данные из разных источников
- формирует отчёты и аналитические выводы

---

### 🧠 Возможности

- RAG (работа с документами)
- генерация SQL из текста
- суммаризация и анализ
- мульти-источники данных
- персональные AI-ассистенты
- визуализация данных

---

### ⚙️ Технологии

**Backend / Core:**  
Python (async processing, pipelines)

**AI / LLM:**  
LangChain, RAG, Embeddings

**Обработка данных:**  
Pandas, SQL

**Векторное хранилище:**  
ChromaDB

**Интерфейс:**  
Streamlit

**Архитектура:**  
Мультиагентная система, оркестратор

---

### 🏗️ Архитектура

```text
Пользователь → Оркестратор → Агенты → Данные → Ответ
````

---

### 🤖 Мультиагентная архитектура

* Classifier Agent — определение типа запроса
* Query Refiner — нормализация запроса
* RAG Agent — работа с документами
* SQL Generator — генерация SQL
* Debugger — исправление ошибок
* Chart Agent — построение графиков
* ECharts Agent — визуализация
* Security Agent — проверка безопасности

---

### 🎥 Демо

<p align="center">
  <a href="https://www.youtube.com/watch?v=o1llLmzHkks">
    <img src="./assets/preview.png" alt="Demo Preview" width="70%" />
  </a>
</p>

<p align="center">
  <sub>Нажми на изображение, чтобы посмотреть демо</sub>
</p>

---

### Результат

* снижение ручного труда
* ускорение работы с данными
* повышение эффективности принятия решений

---

### Примечание

Проект представлен в обобщенном виде без раскрытия конфиденциального внутреннего содержимого.

</details>

---

<details>
<summary>🇬🇧 English</summary>

### 🚀 Overview

Digital AI Assistant is a platform for automating knowledge work across documents, tables, and databases using natural
language.

It combines LLMs, RAG, and a multi-agent architecture to enable users to interact with data without writing code or SQL.

---

### 💡 Problem

* working with data requires technical expertise
* manual document analysis is time-consuming
* difficult to extract insights from multiple sources
* high entry barrier for non-technical users

---

### ✅ Solution

An intelligent assistant that:

* understands natural language queries
* processes documents (PDF, Excel, text)
* generates SQL queries
* aggregates data from multiple sources
* produces reports and insights

---

### 🧠 Core Capabilities

* RAG-based document understanding
* natural language → SQL
* summarization and analysis
* multi-source data integration
* personalized AI assistants
* data visualization

---

### ⚙️ Tech Stack

**Backend / Core:**
Python (async processing, pipelines)

**AI / LLM:**
LangChain, RAG, Embeddings

**Data Processing:**
Pandas, SQL

**Vector Storage:**
ChromaDB

**Interface:**
Streamlit

**Architecture:**
Multi-agent system, orchestrator pattern

---

### 🏗️ Architecture

```text
User → Orchestrator → Agents → Data → Response
```

---

### 🤖 Multi-Agent Architecture

* Classifier Agent — request classification
* Query Refiner — query normalization
* RAG Agent — document-based reasoning
* SQL Generator — NL → SQL
* Debugger — error correction
* Chart Agent — visualization
* ECharts Agent — dashboards
* Security Agent — validation

---

### 🎥 Demo

<p align="center">
  <a href="https://www.youtube.com/watch?v=o1llLmzHkks">
    <img src="./assets/preview.png" alt="Demo Preview" width="70%" />
  </a>
</p>

<p align="center">
  <sub>Click the image to watch the demo</sub>
</p>

---

### Impact

* reduced manual work
* faster data access
* improved productivity

---

### Notes

This project is presented in a generalized form without disclosing confidential internal content.

</details>
