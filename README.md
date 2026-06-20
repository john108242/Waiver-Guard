# Liability Waiver & Release System

A premium, fully responsive, and mobile-optimized web application for managing customer liability waivers. Designed specifically for touchscreen devices such as **iPads and tablets**, as well as desktop computers.

## 🚀 Live Demo & Hosting
Since iOS and Android devices require a secure context (**HTTPS**) to access media devices (camera), you must host this project on a secure web server to capture photos on iPads/tablets. 

The easiest way to host this for free is using **GitHub Pages**:
1. Upload this repository to GitHub.
2. Go to **Settings** > **Pages** in your GitHub repository.
3. Under **Build and deployment**, set the source to **Deploy from a branch**.
4. Select the **main** (or **master**) branch and the `/root` folder, then click **Save**.
5. Your site will be live at `https://<your-username>.github.io/<your-repository-name>/` in a few minutes.

---

## ✨ Features
- **Client Information Form**: Fields for Full Name, Phone Number, National ID/Passport, Gender (interactive cards), and staff name.
- **Camera Capture**: Directly accesses the tablet/phone camera to snap client photos and preview them.
- **Digital Touch Signature**: Touch-friendly canvas signature box, optimized for iPad styluses and touch inputs, with automatic screen-scroll locking while drawing.
- **Local Persistence Log**: Saves all signed waivers locally in the browser's `localStorage` for offline review.
- **Auto-Generated PDF**: Automatically builds a formatted corporate certificate with the client's information, photo, and signature, and downloads it directly as a PDF named `[customer_name]_[date].pdf`.

---

## 📂 Project Structure
- `index.html` - Application layout, form elements, and print template.
- `style.css` - Modern dark midnight glassmorphism theme and media queries.
- `app.js` - Camera stream, canvas signature physics, localStorage CRUD, and html2pdf compiling.
- `server.ps1` - Lightweight PowerShell script to serve files locally on `http://localhost:8080/`.

---

## 🛠️ Local Development (Offline testing)
Double-click `server.ps1` (or run it in PowerShell) to launch a local web server at:
[http://localhost:8080/](http://localhost:8080/)
