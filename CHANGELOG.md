# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2025-10-01

This is the initial public release of the Daily Workflow PWA, combining the efforts of a command-line script and a web interface into a single, cohesive application.

### Added

- **Initial Application:** Created the core Progressive Web App (PWA) structure with HTML, CSS, and JavaScript.
- **Core Features:** Implemented the main productivity modules:
  - Daily Log with sections for priorities, notes, links, and end-of-day review.
  - Task Management with add, toggle, and delete functionality.
  - Analytics dashboard for productivity statistics.
  - Focus Timer for tracking work sessions.
  - Template system with options for standard, meeting, project, and planning days.
  - Full-text search for logs and tasks.
- **Date Navigation:** Added controls to navigate between different days, including a date picker and quick buttons for "Yesterday," "Today," and "Tomorrow."
- **Robust Data Storage:** Implemented IndexedDB using the Dexie.js library for fast, scalable, and asynchronous client-side data storage.
- **AI Insights:** Integrated with Gemini to provide real, data-driven productivity insights based on user activity.
- **Data Portability:** Added functionality to export and import the entire user database as a JSON file.
- **Automated Deployment:** Created a GitHub Actions workflow (`deploy.yml`) to automatically build and deploy the application to GitHub Pages on every push to the `main` branch.
- **Documentation:** Created this `CHANGELOG.md` and a comprehensive `README.md` detailing the application's features, setup, and potential improvements.

### Changed

- **Unified Experience:** Merged the concepts from an original shell script (`daily_workflow.sh`) into the PWA, creating a single, cross-platform solution.
- **Data Backend:** Upgraded the data persistence layer from the simple `localStorage` to the more powerful and asynchronous IndexedDB.
- **AI Feature:** Replaced static, placeholder AI suggestions with a dynamic feature that generates insights on demand by calling a generative model.

### Removed

- **`daily_workflow.sh`:** The original shell script was removed as its functionality is now fully integrated into the PWA, making it redundant.
