# ⚛️ React Events – TanStack Query + React Router

An event management application demonstrating modern React development patterns.

## 🌟 Live Demos

| Component | URL |
| :--- | :--- |
| **Frontend (Vercel)** | 👉 https://react-events-green.vercel.app/events|
| **Backend API (Render)** | 👉 https://react-events-3ywp.onrender.com/events |

---

## 📌 Overview

**React Events** is a small events management application built to showcase effective use of:

* **React + Vite** for a modern frontend setup.
* **React Router v6** for client-side routing.
* **TanStack Query (React Query)** for efficient data fetching, caching, and mutations.
* **Optimistic Updates** (examples are available in `EditEventOld.js` and `AppOld.jsx`).
* **Express.js backend** (hosted on Render) for serving event data and images.

### ✔️ Features

This application allows users to:

* Browse all events
* Search events
* View event details
* Create new events
* Edit existing events
* Delete events

---

## 🚀 Deployment

### Frontend

* Deployed on **Vercel**.
* Uses the following **Vite environment variable** for API calls:
    ```
    VITE_API_URL=[https://react-events-3ywp.onrender.com](https://react-events-3ywp.onrender.com)
    ```
* All API calls in the app utilize this variable:
    ```javascript
    const BASE_URL = import.meta.env.VITE_API_URL;
    ```

### Backend

* **Express server** deployed on **Render**.
* Serves the following endpoints:
    * `/events`
    * `/events/:id`
    * `/events/images`
    * Static images from the `/public` directory.

---

## 📁 Project Structure

| Directory/File | Description |
| :--- | :--- |
| `/backend` | Node.js/Express server code. |
| &nbsp;&nbsp;&nbsp;&nbsp;`app.js` | Main backend server file. |
| &nbsp;&nbsp;&nbsp;&nbsp;`data/` | Mock filesystem database (JSON files). |
| &nbsp;&nbsp;&nbsp;&nbsp;`public/` | Static images folder. |
| `/src` | Frontend React source code. |
| &nbsp;&nbsp;&nbsp;&nbsp;`components/` | Reusable React components. |
| &nbsp;&nbsp;&nbsp;&nbsp;`util/http.js` | Data fetching and mutation functions. |
| &nbsp;&nbsp;&nbsp;&nbsp;`App.jsx` | Main application component. |
| &nbsp;&nbsp;&nbsp;&nbsp;`main.jsx` | Entry point for the React application. |
| &nbsp;&nbsp;&nbsp;&nbsp;`assets/` | Static assets like icons or local images. |

---

## 🧪 Technologies Used

### Frontend

* **React 18**
* **Vite**
* **React Router 6**
* **TanStack Query 5**
* **JavaScript ES Modules**

### Backend

* **Node.js + Express**
* **Filesystem-based mock database** (`events.json`, `images.json`)

---

## 🛠 How to Run Locally

Follow these steps to set up and run the project on your local machine.

### 1. Clone the project

```bash
git clone [https://github.com/anouar4070/React-Events](https://github.com/anouar4070/React-Events)
cd React-Events
