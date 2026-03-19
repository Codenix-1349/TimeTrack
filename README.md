
# Zeiterfassung

A browser-based time tracking app for managing projects, tracking work sessions, and exporting timesheet data.

<p align="center">
  <img alt="HTML5" title="HTML5" height="36" src="https://raw.githubusercontent.com/github/explore/main/topics/html/html.png" />&nbsp;&nbsp;
  <img alt="CSS3" title="CSS3" height="36" src="https://raw.githubusercontent.com/github/explore/main/topics/css/css.png" />&nbsp;&nbsp;
  <img alt="JavaScript" title="JavaScript" height="36" src="https://raw.githubusercontent.com/github/explore/main/topics/javascript/javascript.png" />&nbsp;&nbsp;
</p>

---

## Overview

Zeiterfassung is a lightweight local-first time tracking app built as a standalone browser application.  
It helps you manage projects, record work sessions, add manual entries, review totals, and export your data without requiring a backend or external service.

---

## Features

- Live timer with start, pause, resume, save, and discard actions
- Project-based time tracking
- Manual time entry support
- Daily, weekly, and total time summaries
- Project overview with total hours and man-day calculation
- Color-coded project management
- Searchable work log
- JSON backup export
- JSON backup import
- CSV export for timesheet data
- Local persistence via browser localStorage
- Optional file-based auto-save via File System Access API
- Responsive single-page layout

---

## Screenshots

### Standard View

![Zeiterfassung Standard View](https://github.com/user-attachments/assets/2c1361b5-5dd5-44a6-a4fe-71bbb410e521)

*Main workspace with project overview, timer section, entry management, totals, and export and backup actions in a clean local-first dashboard.*

<br>

### New Project View

![Zeiterfassung New Project View](https://github.com/user-attachments/assets/351bf2b0-edff-4075-9fec-0bc93a024ce5)

*Focused project creation flow for adding a new project with custom name, color, and working-day settings before tracking begins.*

---

## Tech Stack

- HTML5
- CSS3
- JavaScript
- Browser LocalStorage
- File System Access API
- JSON / CSV export

---

## Getting Started

### 1. Clone the repository

```bash
git clone git@github.com:Codenix-1349/TimeTrack.git
cd TimeTrack
````

### 2. Open the app

This project is a standalone browser app, so no installation is required.

Open the HTML file directly in your browser:

```bash
start Zeiterfassung.html
```

Or simply double-click the file in your project folder.

---

## Usage

### Track time

* Select or create a project
* Enter a task description
* Choose a date
* Start the timer
* Pause or resume as needed
* Save the entry when finished

### Add manual entries

* Open the manual entry form
* Select a project
* Enter description, date, and duration
* Save the entry

### Export data

* Export all entries as JSON backup
* Import a JSON backup to restore data
* Export entries as CSV for spreadsheet usage

---

## Storage

The app stores data locally in the browser using `localStorage`.

When supported by the browser, you can also connect a JSON file and enable auto-save to disk.

---

## Browser Support

### Fully supported

* Chrome
* Edge

### Partially supported

* Firefox
  Local usage works, but file-based auto-save via File System Access API may not be available.

---

## Project Structure

```text
.
└── Zeiterfassung.html
```

---

## Data Model

### Project

```json
{
  "id": "p12345",
  "name": "Client Project",
  "color": "#f5c842",
  "hpd": 8
}
```

### Entry

```json
{
  "id": "e12345",
  "projectId": "p12345",
  "date": "2026-03-19",
  "desc": "Frontend implementation",
  "start": "09:00",
  "end": "11:30",
  "durationSec": 9000
}
```

---

## Highlights

* Single-file application
* No backend required
* Fast local usage
* Suitable for personal project tracking and lightweight work logging
* Easy backup and export workflow

---

## Notes

* Data is primarily stored locally in the browser
* Clearing browser storage may remove locally saved data
* File-based persistence depends on browser support for the File System Access API

````

