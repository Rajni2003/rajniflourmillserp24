# Rajni Flour Mills ERP System

An intuitive, responsive, and resilient Enterprise Resource Planning (ERP) application designed custom for managing flour mill operations. It bridges the gap between fast, offline-first local interaction and structured cloud database synchronization.

---

## 🚀 Key Features

*   **Offline-First Architecture**: Operations continue flawlessly if the local network or internet drops out. All records save instantly to local storage.
*   **Dynamic Firebase Cloud Sync**: Automatically merges local offline modifications with a secure remote Firebase Firestore database once connection stability is verified.
*   **Bilingual Accessibility**: Tailored layout supporting dual translations (English and Punjabi labels) for standard ease of use.
*   **Operational Flow Tracking**: Structured pipeline covering the entire lifecycle of milling tasks:
    1.  **New Entry**: Capture customer queues, incoming grain types, weights, and expected delivery commitments.
    2.  **Under Process**: Materials organized cleanly by category (Wheat, Maize, Rice, etc.) to optimize active production steps.
    3.  **Completed Orders**: Enter absolute final weight outputs and queue orders for pick up.
    4.  **Final Dispatch & Income Verification**: Record actual pricing tallies and payments (Cash / UPI) prior to archiving.
*   **Granular Reporting**: Built-in month-to-date summaries, specific calendar date-range lookups, interactive transactional charts, and instantaneous raw `.csv` file exporting.
*   **Local Backups Management**: Secure standalone `.json` structural files can be generated, exported locally, or re-uploaded to rebuild internal browser data states cleanly.

---

## 🛠️ Tech Stack & Dependencies

*   **Frontend**: Vanilla HTML5, Modern CSS3 variables (featuring customizable Dark & Light glassmorphism themes).
*   **Styling & Responsiveness**: Scalable flexbox configurations accommodating mobile displays up to massive terminal views.
*   **Icons Framework**: Dynamic, responsive node icons injected via the [Lucide Icons CDN](https://unpkg.com/lucide@latest).
*   **Cloud Platform Database**: Integrated cleanly via native ES6 modules utilizing the [Firebase JavaScript v10.8.0 SDK](https://firebase.google.com/docs/web/setup) (App & Firestore modules).

---

## 📂 Codebase File Structure

*   `index.html` / Application Frames: Declarative modular markup establishing high-performance custom data dashboard zones, filter widgets, entry fields, and transaction lists.
*   `styles.css`: Deep styling definitions using localized custom parameters (`:root` / `[data-theme="light"]`) establishing layout constraints and rendering interactive dynamic elements smoothly.
*   `app.js`: Core controller handling UI states, calculation utilities, local variables lifecycle rules, and programmatic background database synchronizations.

---

## 🔧 Installation & Getting Started

1. Clone or download this project workspace into your directory of choice.
2. Since the app relies directly on standard ES6 JavaScript Dynamic Modules (`import` / `importmap`), launch the directory through a local web server (e.g., using VS Code's *Live Server* extension, python's `http.server`, or Node.js running `http-server`).
3. Open the assigned address link in any modern web browser.
4. If your network configuration blocks direct connection to the underlying cloud database `milllmr.firebaseapp.com`, the program will alert the operator via a localized system tray prompt and auto-enable safe local execution constraints immediately.
