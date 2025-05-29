# TrainSwift

**TrainSwift** is a responsive and modern web application for searching, filtering, and booking train tickets. It provides users with a seamless experience to explore train options, select seats, and manage bookings — all in a single platform.  
🌐 [Live Demo](https://trainswift.netlify.app/)

---

##  Features

-  **Train Search:** Search for trains by source, destination, and date.
-  **Advanced Filters:** Filter by price, class, departure/arrival time.
-  **Seat Selection:** Choose seats interactively via a custom seat map.
-  **Booking Confirmation:** Receive confirmation with booking details.
-  **User Auth:** Simple sign-up and login using in-memory auth.
-  **Emission Chart:** Visual CO₂ emission comparison.
-  **My Bookings:** View and manage your confirmed bookings.
-  **404 Handling:** Friendly error pages with navigation support.
-  **Responsive UI:** Built with Tailwind CSS and reusable UI components.

---

##  Live Site

[https://trainswift.netlify.app/](https://trainswift.netlify.app/)

---

## 🛠 Tech Stack

- **Frontend Framework:** React (with Vite)
- **State Management:** Zustand
- **Routing:** React Router
- **Styling:** Tailwind CSS
- **Charting:** [Recharts](https://recharts.org/)
- **Icons:** Lucide
- **UI Components:** Custom + ShadCN-inspired UI
- **Build Tool:** Vite

---

##  Project Structure

```
├── public/                   # Static assets (favicon, icons)
├── src/
│   ├── components/           # Reusable UI & custom components
│   ├── pages/                # Main pages like Home, Booking, etc.
│   ├── stores/               # Zustand stores for auth, trains, bookings
│   ├── assets/               # SVGs and media
│   ├── App.jsx               # Root component
│   ├── main.jsx              # Entry point
├── index.html                # Root HTML file
├── tailwind.config.js        # Tailwind CSS config
├── postcss.config.js         # PostCSS config
├── vite.config.js            # Vite config
├── jsconfig.json             # JavaScript project config
└── .gitignore
```

---

##  How to Run Locally

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/trainswift.git
cd trainswift
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Run the Development Server

```bash
npm run dev
```

Then visit [http://localhost:5173](http://localhost:5173)

---

##  Authentication

- Handled via `authStore.js` using Zustand with local persistence
- No backend — credentials are stored in memory

---

##  State Management

Zustand is used to manage:

- Train data and filters (`trainStore.js`)
- User authentication (`authStore.js`)
- Booking data (`bookingStore.js`)

All stores persist data using `zustand/middleware`.

---

##  Emission Chart

The EmissionChart component visualizes estimated CO₂ emissions per train route. Great for highlighting sustainability in train travel.

---

## Deployment

This project is deployed via [Netlify](https://www.netlify.com/).  
To deploy your own:

1. Connect GitHub repo to Netlify.
2. Set build command: `npm run build`
3. Set publish directory: `dist`

---

## Credits

This project was built using modern React tools, Zustand, Tailwind CSS, and open-source component libraries.

---
