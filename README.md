
# Zeiterfassung

A browser-based time tracking app for managing projects, tracking work sessions, and exporting timesheet data.

<p align="center">
  <img alt="HTML5" title="HTML5" height="36" src="https://raw.githubusercontent.com/github/explore/main/topics/html/html.png" />&nbsp;&nbsp;
  <img alt="CSS3" title="CSS3" height="36" src="https://raw.githubusercontent.com/github/explore/main/topics/css/css.png" />&nbsp;&nbsp;
  <img alt="JavaScript" title="JavaScript" height="36" src="https://raw.githubusercontent.com/github/explore/main/topics/javascript/javascript.png" />&nbsp;&nbsp;
</p>

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

## Screenshots

### Timer Dashboard

<p align="center">
  <img src="https://github.com/user-attachments/assets/351bf2b0-edff-4075-9fec-0bc93a024ce5" alt="Zeiterfassung Timer Dashboard" width="760" />
</p>

<p align="center">
  <em>
    Clean timer-focused workflow with project selection, task description, date input, and quick actions for starting, pausing, saving, or discarding tracked sessions.
  </em>
</p>

### Project Overview & Work Log

<p align="center">
  <img src="https://github.com/user-attachments/assets/2c1361b5-5dd5-44a6-a4fe-71bbb410e521" alt="Zeiterfassung Project Overview and Work Log" width="1000" />
</p>

<p align="center">
  <em>
    Structured workspace for managing projects, reviewing logged entries, checking totals, and using backup/export actions in a practical local-first time tracking setup.
  </em>
</p>

## Tech Stack

- HTML5
- CSS3
- JavaScript
- Browser LocalStorage
- File System Access API
- JSON / CSV export

## Getting Started

### 1. Clone the repository

```bash
git clone git@github.com:Codenix-1349/Zeiterfassung.git
cd Zeiterfassung
````

### 2. Open the app

This project is a standalone browser app, so no installation is required.

Open the HTML file directly in your browser:

```bash
start Zeiterfassung.html
```

Or simply double-click the file in your project folder.

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

## Storage

The app stores data locally in the browser using `localStorage`.

When supported by the browser, you can also connect a JSON file and enable auto-save to disk.

## Browser Support

### Fully supported

* Chrome
* Edge

### Partially supported

* Firefox
  Local usage works, but file-based auto-save via File System Access API may not be available.

## Project Structure

```text
.
└── Zeiterfassung.html
```

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

## Highlights

* Single-file application
* No backend required
* Fast local usage
* Suitable for personal project tracking and lightweight work logging
* Easy backup and export workflow

## Notes

* Data is primarily stored locally in the browser
* Clearing browser storage may remove locally saved data
* File-based persistence depends on browser support for the File System Access API

````


