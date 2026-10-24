
# React CRUD App

A responsive user management application built with React 19, JavaScript, and Vite as part of CSC322 Web Programming at Sullivan University.

## Overview

This project demonstrates the four fundamental CRUD (Create, Read, Update, Delete) operations using React functional components and Hooks.

The application allows users to manage a collection of records through a simple, interactive interface. It uses React state to handle data and update the interface without requiring a backend or database.

The project is based on Tania Rascia's [Build a CRUD App in React with Hooks](https://www.taniarascia.com/crud-app-in-react-with-hooks/) tutorial, adapted for React 19 and Vite. The interface features custom responsive styling designed to match my software developer portfolio.

## Features

- **Create:** Add users by entering a name and username.
- **Read:** Display existing users in a dynamically updated table.
- **Update:** Select and edit an existing user's information.
- **Delete:** Remove users from the table.
- **React Hooks:** Manage application state with `useState` and synchronize the edit form with `useEffect`.
- **Unique IDs:** Generate user IDs without reusing existing IDs after records are deleted.
- **Responsive Design:** Adapt the layout to different screen widths, including embedded displays.
- **Custom Styling:** Use a dark charcoal and slate color scheme with muted blue accents.

## Technologies Used

- React 19
- JavaScript (ES6+ and JSX)
- Vite
- HTML5
- CSS3

## Getting Started

### Prerequisites

- Node.js
- npm

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/s-scoville/react-crud-app.git
   ```

2. Navigate to the project directory:

   ```bash
   cd react-crud-app
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Start the development server:

   ```bash
   npm run dev
   ```

5. Open the local URL displayed in the terminal.

## How It Works

The application loads with three sample user records.

Users can add new records through the input form, edit existing records by selecting the Edit button, or remove records using the Delete button. The interface updates automatically whenever the underlying React state changes.

The application uses separate components for the user table, adding users, and editing users. The main application component manages the shared state and passes the necessary data and functions to its child components.

### Data Storage

All user records are stored in React state. The application does not use a database, backend API, or persistent storage.

Any changes made during a session are reset when the page is refreshed.

## Responsive Design

The application uses a custom dark theme consistent with my software developer portfolio.

CSS Grid and media queries allow the interface to adjust based on the available viewport width. On wider screens, the user form and table appear side by side. On narrower screens, they stack vertically to maintain readability and usability.

The layout is also designed to work within an iframe, allowing the application to be embedded into an existing website while maintaining its responsive behavior.

## Project Structure

```text
src/
├── forms/
│   ├── AddUserForm.jsx
│   └── EditUserForm.jsx
├── tables/
│   └── UserTable.jsx
├── App.jsx
├── index.css
└── main.jsx
```

- **App.jsx:** Manages user records, editing state, and CRUD operations.
- **AddUserForm.jsx:** Handles adding new users.
- **EditUserForm.jsx:** Handles editing existing users.
- **UserTable.jsx:** Displays user records and provides Edit and Delete controls.
- **index.css:** Contains the application's styling and responsive layout rules.
- **main.jsx:** Initializes and renders the React application.

## Acknowledgments

This project is based on [Build a CRUD App in React with Hooks](https://www.taniarascia.com/crud-app-in-react-with-hooks/) by Tania Rascia.

The original tutorial uses Create React App. This implementation uses React 19 and Vite, with additional adjustments for user ID generation, form behavior, and custom responsive styling.