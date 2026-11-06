# Hermann Gmeiner School — School Activities Platform (Day 3)

A modern, responsive, and bilingual (English & Albanian) single-page web application designed for Hermann Gmeiner School. This project showcases extracurricular clubs, sports tournaments, tech workshops, and academic events, allowing students to explore, filter, sort, favorite, and register for activities seamlessly.

---

## 🚀 Day 3 New Features (Favorites & Sorting)

* **Favorites System:**
  * Interactive heart toggle button (`❤️` / `🤍`) on every activity card.
  * Unique ID-based tracking to ensure correct persistence regardless of list order.
  * **"Favorites Only" Filter:** Dedicated button to instantly toggle and display only saved favorite activities.
  * Persistent storage using browser `localStorage` (`hg_favorites`).
* **Advanced Sorting Options:**
  * Four distinct sorting criteria:
    1. **Date:** Earliest first (`date-asc`)
    2. **Date:** Latest first (`date-desc`)
    3. **Title:** A to Z (`title-asc`)
    4. **Title:** Z to A (`title-desc`)
  * Stable sorting with automatic tie-breakers by activity ID.
  * Real-time sorting updates without page reloads, fully compatible with active search queries, category filters, and the "Favorites Only" view.
* **UI/UX Enhancements:**
  * Smooth toast notifications when adding/removing favorites.
  * Advanced empty-state handling with a quick reset filters button.
  * Student Spotlight grid and student-friendly FAQ section.

---

## 🛠️ Existing Core Features

* **Bilingual Support (EN / SQ):** Instant language switcher with `localStorage` persistence preventing any flash of unstyled content on reload.
* **Live Search & Category Filters:** Instant text search by title combined with category selection (Sports, Technology, Arts, Education).
* **Registration Flow:** Interactive registration modal with client-side form validation and success feedback.
* **"My Registrations" Lookup:** Email-based lookup allowing students to review all clubs they have registered for.
* **Playful Micro-Interactions:** Floating 3D interactive book animation following page scroll, responsive mobile navigation drawer, and floating WhatsApp contact button.

---

## 📂 Project Structure

```text
├── index.html          # Main single-page application markup & JavaScript logic
├── style.css           # Complete responsive styling, variables & animations
├── activities.json     # Main JSON dataset containing all school activities (EN/SQ)
├── activities.js       # Fallback dataset for direct local file execution (file://)
└── README.md           # Project documentation and setup guide