# Cybernode 2077 Diary

A cyberpunk-themed diary application built as a **solo React project** during the WBS Coding School Full Stack Web & App Development program.

The project combines a component-based React interface with local persistence, modal-driven interactions and a custom visual identity inspired by futuristic data terminals and cyberpunk UI design.

### [▶ Open the live demo](https://cybernode-2077.onrender.com/)

---

## Key Features

- create diary / data-log entries
- title, date, image URL and text content for each entry
- persistent storage in the browser with `localStorage`
- dedicated detail view for individual logs
- delete individual entries or clear the complete log collection
- duplicate-date validation when creating entries
- randomized starter suggestions for new entries
- responsive modal-based UI
- custom cyberpunk visual design
- animated system wipe and restore sequence

---

## Tech Stack

- React
- JavaScript / JSX
- Vite
- Tailwind CSS
- daisyUI
- React Hooks
- localStorage
- ESLint
- Prettier
- pnpm

---

## Application Structure

The interface is split into reusable components for different responsibilities, including:

- header and application controls
- log collection
- individual log cards
- new-log form
- log detail view
- delete confirmation
- empty-state handling
- footer and visual system states

Application state is managed with React hooks.

A custom `useLocalStorage` hook loads saved diary entries when the application starts and persists changes back to the browser whenever the collection changes.

Supporting functions handle tasks such as creating and deleting entries, generating starter content and selecting visual assets.

---

## UI & Interaction

A major focus of the project was creating a distinct visual identity rather than building a generic diary interface.

The UI uses:

- neon-inspired typography and effects
- layered gradients and glow effects
- custom imagery
- modal-based input and detail views
- responsive layouts
- visual feedback for interaction states

The "Delete All" flow also includes a custom **system wipe / restore animation**. The visual transition is coordinated with the actual state change so that clearing the stored data becomes part of the application's cyberpunk presentation rather than only a standard delete action.

---

## Creating Logs

New entries are created through a dedicated modal form.

Each entry can contain:

- a title
- a date
- an image URL
- diary text

The form starts with generated suggestions that can be replaced with the user's own content.

The application also checks whether an entry already exists for the selected date and prevents saving a conflicting entry.

Saved logs remain available after refreshing or reopening the application because the data is persisted with `localStorage`.

---

## Project Context

Cybernode 2077 Diary was developed independently as a **solo project in the WBS Coding School course context** and presented during the program.

The project gave me an opportunity to focus especially on:

- React component structure
- state and event handling
- custom hooks
- client-side persistence
- forms and modal flows
- responsive UI development
- visual design and branding
- translating a strong design concept into an interactive application

Compared with my larger Match-3 final project, Cybernode is intentionally a smaller application and serves primarily as a showcase for **independent React development, UI implementation and visual experimentation**.

---

## Running Locally

Clone the repository and install the dependencies:

```bash
git clone https://github.com/jan-ninh/cybernode-2077-diary.git
cd cybernode-2077-diary
pnpm install
```

Start the development server:

```bash
pnpm dev
```

Create a production build with:

```bash
pnpm build
```
