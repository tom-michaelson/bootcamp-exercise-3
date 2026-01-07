# Product Requirements Document (PRD) - TODO App Upgrade: Due Dates, Priorities, Filters

## 1. Overview

We are upgrading the basic TODO app to support due dates, priorities, and filter views so users can better organize tasks and quickly focus on what matters today or is overdue. The solution remains front-end only and uses local storage, enabling a simple, teachable MVP without backend changes.

---

## 2. MVP Scope

- Data model: `title` required; `priority` is one of "P1", "P2", "P3" with default "P3"; `dueDate` optional ISO date (`YYYY-MM-DD`).
- Validation: Invalid `dueDate` values are ignored and treated as absent.
- Filters: Provide tabs/views for All, Today, Overdue.
- Filter behavior: Today and Overdue show only incomplete tasks; All includes completed tasks.
- Storage: Local storage only; no backend or external persistence.

---

## 3. Post-MVP Scope

- Overdue highlighting: Visually emphasize overdue tasks (e.g., red highlight/badge).
- Sorting rules: Overdue first → by priority (P1→P3) → due date ascending → tasks without due date last.
- Priority badges: Color-coded badges for priority levels (e.g., P1 red, P2 orange, P3 gray).

---

## 4. Out of Scope

- Notifications.
- Recurring tasks.
- Multi-user features.
- Keyboard navigation or specialized accessibility features beyond defaults.
- External storage or backend persistence (no server-side changes).
