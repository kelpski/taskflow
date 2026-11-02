# Taskflow

A responsive, local-first task manager in sky blue, white, and hot pink. Built with Vanilla JavaScript, Tailwind CSS 4, and Vite.

## Develop

Requires Node.js 20.19+ or 22.12+.

```sh
npm ci --cache /tmp/taskflow-npm
npm run dev
```

```sh
npm run build
npm run preview
```

## Features

- Four-column drag-and-drop Kanban board; edit a task’s status for a keyboard/touch alternative.
- Monthly/weekly calendar with date-specific task creation.
- Sortable list with bulk completion and deletion.
- Search, priority filters, navigation presets, subtasks, tags, estimates, and light/dark appearance.
- Eight initial tasks dated relative to the first visit. Tasks and theme persist in localStorage (`taskflow-v1`).
- Local assistant: natural-language quick-add, due-date-based prioritization, template-based task breakdown, and task-aware chat. No API calls, external AI model, or credentials are used. Supported date input includes today, tomorrow, weekday names, next week, and YYYY-MM-DD. Time-of-day input remains in the description; dueDate is date-only. Review generated tasks before relying on them.

Data stays in the current browser and is not synchronized across devices. Clearing browser storage removes saved tasks. Sample collaborators are decorative; this app has no authentication or shared workspace backend.

## Validation

Production build and DOM interaction smoke checks passed. Chromium download was blocked by the cloud network policy, so visual browser validation was not performed.
