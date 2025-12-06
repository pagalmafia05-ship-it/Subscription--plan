# Subscription Landing Page (Single-file)

This repository contains a single-file subscription landing page demo (`index.html`) that includes:

**Features**
- Two subscription plans: **Basic (₹149)** and **Business (₹249)**.
- **Admin panel** protected by password: `rimshaarru`.
  - Edit plan titles, prices, subtext, features.
  - Upload images for each plan (saved to browser `localStorage`).
- Clicking **Buy Now** opens a modal:
  - Shows the plan image (uploaded via Admin).
  - Starts a **10-minute countdown timer**.
  - Shows UPI app buttons — clicking attempts to open a UPI deep link on mobile devices.
- All settings and uploaded images persist in the browser using `localStorage`.
- No backend required — purely static HTML/JS/CSS.

**How to use**
1. Download `index.html` and open it in your browser.
2. Click **Admin Panel** and enter password: `rimshaarru`.
3. Select a plan, edit fields, upload an image, and click **Save Plan**.
4. Click **Buy Now** on any plan:
   - A modal shows the image and timer.
   - Click a UPI app button to attempt payment via your phone's UPI apps.

**Notes & Limitations**
- Uploaded images and settings are saved in **localStorage** of your browser — clearing browser data will remove them.
- UPI deep links (`upi://pay?...`) work on many mobile devices with UPI apps installed. On desktop browsers they may not function or may show an error.
- This demo uses a placeholder `merchant@upi` payee VPA. Replace with your actual VPA in the JS `UPI_APPS` section if you have one.
- This is a frontend demo only. For real payments, integrate a secure backend and payment gateway.

**Publishing to GitHub Pages**
1. Create a new public GitHub repository.
2. Upload `index.html` (and optionally `README.md`).
3. In the repository settings, enable **GitHub Pages** and choose the `main` branch (or `gh-pages`) root.
4. Your site will be available at `https://<your-username>.github.io/<repo-name>/`.

Enjoy! ❤️
