# 📚 Gaya.Library - Modern Public Library Website (Veyangoda, Sri Lanka)

A modern, responsive, frontend-only public library web application for **Gaya.Library** located in **Veyangoda, Sri Lanka**. Built with **HTML5**, **Tailwind CSS**, and **Vanilla JavaScript**. No database or backend server is needed; all book records, categories, loans, and favorites run smoothly entirely in the browser.

### 📍 Library Details
- **Library Name**: `Gaya.Library`
- **Location**: Veyangoda, Western Province, Sri Lanka
- **Phone**: `076 555 1111` (International: `+94 76 555 1111`)
- **Email / Domain**: `info@gaya.library.com` &bull; `gaya.library.com`

---

## ✨ Key Features

### 🎬 High-End Visual Design & Cinematic Features
- **Cinematic Video Background**: Full-screen HTML5 looping library video with `object-fit: cover` and a dark radial backdrop blur overlay (`backdrop-blur-[3px]`) ensuring crisp text legibility.
- **3D Book Coverflow Carousel (Swiper.js)**: Curved 3D book exhibition powered by Swiper.js Coverflow effect with realistic leather hardcover spines, gold filigrees, drag/swipe gestures, autoplay, and direct loan/details actions.
- **Sri Lankan Literary Classics**: Rare hardcover collection including **Madol Duwa (මාදොල් දූව)**, **Gamperaliya (ගම්පෙරළිය)**, **Viragaya (විරාගය)**, **Kaliyugaya (කලියුගය)**, **Yuganthaya (යුගාන්තය)**, **Ape Gama (අපේ ගම)**, and **Senkottan (සෙන්කොට්ටන්)**.
- **High-End Typography**: Google Fonts imported and configured:
  - **`Poppins`**: Clean, modern body and UI typography.
  - **`Playfair Display` & `Abhaya Libre`**: High-end editorial and Sinhala serif typography for headlines and literary prestige.
- **100% Frontend-Only**: Zero backend or database requirements; completely self-contained in browser with persistent `localStorage`.

### 2. 📖 Catalog Page
- **Dynamic Category Filters**:
  - Filter across **Fiction**, **Technology**, **Science**, or **All Books** with real-time book count badges.
- **Live Search**:
  - Instant live search with debouncing across Title, Author, ISBN, Tags, and Sub-categories.
- **Availability Filters**:
  - Filter by status: `Available Now`, `Checked Out`, and `Reserved / Waitlist`.
- **Sorting Options**:
  - Sort by `Most Popular`, `Highest Rated`, `Publication Year (Newest)`, and `Title (A–Z)`.
- **Layout Toggles**:
  - Switch between **Responsive Grid View** and **Detailed List View**.
- **Interactive Book Cards**:
  - Availability pill badges with real-time copy counts or return estimates (`Oct 22, 2026`).
  - 3D hover elevation and tilt effects on book covers.
  - Quick action buttons: **View Details Modal**, **Borrow Now**, **Join Waitlist**, and **Save to Favorites** (heart icon).
- **Active Filter Chips**:
  - Visual removable pills for active keywords and filters with a one-click "Clear All" button.
- **Interactive Pagination**:
  - Seamless page navigation with automatic smooth scroll.

### 3. 🔍 Detailed Book Modal
- Large cover art preview with fallback gradient styling.
- Complete metadata: ISBN, Page count, Language, and Physical Shelf Location (e.g., `Floor 3 • Aisle 1 • Shelf C`).
- Full synopsis, thematic tags (`#MachineLearning`, `#DistributedSystems`, `#MagicalRealism`).
- Interactive loan and hold buttons with calculated due dates (21-day loan periods).

### 4. 🎒 Client-Side Borrowing & Reading List
- **My Loans Slide-over Drawer**:
  - Track currently borrowed books and due dates.
  - Return books at any time with real-time stock updates.
  - Persisted in browser `localStorage`.
- **Saved Favorites Drawer**:
  - Bookmark titles to an offline wishlist with persistent heart badges.

### 5. 🏛️ About & Operating Hours Page
- Heritage, mission, and fine-free philosophy.
- **Live Operating Status Widget**: Computes whether the library is currently `Open Now` or `Closed` based on the real-time day and hour.
- **Floor-by-Floor Directory Guide**: Floor 1 through Floor 4 stack breakdowns.
- **Interactive FAQ Accordion**: Smooth collapsible questions and answers.

### 6. 📬 Contact Page
- Physical address, subway/transit instructions, and phone contacts.
- Comprehensive contact form with simulated submission, field validation, and toast feedback.
- Newsletter subscription box.

### 7. 🎨 UI/UX & Transitions
- **Glassmorphism**: Sticky navigation bar and cards with backdrop blur.
- **Dark Mode / Light Mode**: Manual toggle button with auto-detection of system preferences and `localStorage` persistence.
- **Toast Notifications**: Animated floating toasts for successful actions, returns, and form submissions.
- **100% Mobile Responsive**: Tested for phones, tablets, and desktops with an accessible slide-over mobile menu.

---

## 📁 Project Structure

```
modern-library/
├── index.html              # Main HTML5 entry point containing all pages & modals
├── css/
│   └── styles.css          # Custom animations, 3D card tilt, glassmorphism, scrollbars
├── js/
│   ├── books-data.js       # Curated JavaScript dataset with 20+ realistic book entries
│   ├── catalog.js          # Catalog filtering, search, sorting, and pagination controller
│   └── app.js              # Routing, theme toggle, loans/favorites, modals, and toasts
└── README.md               # Documentation and usage guide
```

---

## 🚀 How to Run the Website

### Option 1: Double-click (No server required)
Because this application is 100% frontend-only and loads external assets via public CDNs, you can open `index.html` directly in any modern browser:
1. Navigate to the project folder:
   ```
   C:\Users\nadee\.gemini\antigravity\scratch\modern-library
   ```
2. Double-click `index.html` (or right-click -> "Open with" -> Google Chrome / Microsoft Edge / Firefox).

### Option 2: Run with a local HTTP server
Using Python (if installed):
```powershell
cd C:\Users\nadee\.gemini\antigravity\scratch\modern-library
python -m http.server 8080
```
Then visit `http://localhost:8080` in your web browser.

### Option 3: Deploy to Vercel or Netlify (100% Ready)
This project is completely frontend-only and ready for instant deployment:
- **Netlify**: Drag and drop the `modern-library` folder onto your [Netlify Dashboard](https://app.netlify.com/drop).
- **Vercel**: Import your Git repository into Vercel:
  - Framework Preset: `Other`
  - Build Command: *(Leave blank)*
  - Output Directory: *(Leave blank / `.`)*
All video streams, 3D vector book covers, and fonts load from high-speed global CDNs with dark fallbacks (`#0f172a`), ensuring zero broken paths.
