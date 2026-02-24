# 💸 DT Money - Rocketseat Ignite

## 📌 Overview

DT Money is a ReactJS front-end application developed during the
Rocketseat Ignite program.\
It simulates a financial transactions dashboard, allowing users to
create and list income and expense transactions.

The project uses a mock API powered by MirageJS, meaning no real backend
or environment variables are required to run it locally.

------------------------------------------------------------------------

## 🛠️ Technologies Used

### Core Technologies

-   **ReactJS** -- UI library
-   **TypeScript** -- Static typing for JavaScript
-   **Create React App (react-scripts)** -- Project scaffolding and
    build tool

### Styling

-   **styled-components** -- CSS-in-JS styling
-   **polished** -- Utility functions for styling

### API & Data Handling

-   **axios** -- HTTP client
-   **miragejs** -- Mock API server

### UI Components

-   **react-modal** -- Modal component

### Performance

-   **web-vitals** -- Performance metrics

### Testing

-   **@testing-library/react**
-   **@testing-library/jest-dom**
-   **@testing-library/user-event**

------------------------------------------------------------------------

## 📁 Project Structure (Simplified)

    dtmoney-rockeatseat-ignite/
    │
    ├── public/
    ├── src/
    │   ├── components/
    │   ├── styles/
    │   ├── services/
    │   ├── App.tsx
    │   └── index.tsx
    │
    ├── package.json
    └── tsconfig.json

------------------------------------------------------------------------

## 🔄 Application Architecture

``` mermaid
flowchart LR
    UI[React Components] -->|HTTP Requests| Axios
    Axios --> MirageJS
    MirageJS -->|Mocked Data| UI
```

The application flow:

1.  React components trigger requests using Axios.
2.  MirageJS intercepts and simulates API responses.
3.  The UI updates based on mocked transaction data.

------------------------------------------------------------------------

## 🚀 How to Run the Project Locally

### ✅ Requirements

-   Node.js (LTS recommended, \>= 14.x)
-   npm or yarn

------------------------------------------------------------------------

### 1️⃣ Clone the Repository

``` bash
git clone https://github.com/threis/dtmoney-rockeatseat-ignite.git
cd dtmoney-rockeatseat-ignite
```

------------------------------------------------------------------------

### 2️⃣ Install Dependencies

Using npm:

``` bash
npm install
```

Or using yarn:

``` bash
yarn
```

------------------------------------------------------------------------

### 3️⃣ Start Development Server

Using npm:

``` bash
npm start
```

Or using yarn:

``` bash
yarn start
```

The application will start at:

    http://localhost:3000

------------------------------------------------------------------------

## 🧪 Running Tests

Using npm:

``` bash
npm test
```

Using yarn:

``` bash
yarn test
```

------------------------------------------------------------------------

## 🔐 Environment Variables

❗ This project does NOT require any environment variables.

-   There is no `.env` file required.
-   No backend API URL configuration is needed.
-   MirageJS handles all data mocking internally.

If in the future a real API is integrated, the standard Create React App
convention should be used:

    REACT_APP_VARIABLE_NAME=value

------------------------------------------------------------------------

## 📦 Build for Production

To generate a production-ready build:

Using npm:

``` bash
npm run build
```

Using yarn:

``` bash
yarn build
```

The optimized build will be generated inside the `build/` directory.

------------------------------------------------------------------------

## 📌 Summary

  Task                       npm               yarn
  -------------------------- ----------------- --------------
  Install dependencies       `npm install`     `yarn`
  Start development server   `npm start`       `yarn start`
  Run tests                  `npm test`        `yarn test`
  Build production version   `npm run build`   `yarn build`

------------------------------------------------------------------------

## 🏁 Final Notes

-   Fully front-end application.
-   No backend required.
-   Ideal for learning React, TypeScript, component architecture, and
    API mocking with MirageJS.
-   Ready to be deployed to platforms like Vercel, Netlify, or similar
    static hosting providers.

------------------------------------------------------------------------

✨ Happy coding!
