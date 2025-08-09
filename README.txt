# Firebase Hosting Static Website

This project is a ready-to-use template for hosting a static website on **Firebase Hosting**.  
It includes all the necessary configuration files and instructions to quickly deploy your HTML/CSS/JS site online.

---

## 📂 Project Structure
```
.
├── .firebaserc       # Firebase project configuration (replace with your Firebase Project ID)
├── .gitignore        # Files and folders to be ignored by Git
├── firebase.json     # Firebase Hosting settings (public folder)
├── public/           # Your static site files (index.html, CSS, JS, etc.)
└── README.md         # Instructions for setup and deployment
```

---

## 🚀 Prerequisites

Before you start, make sure you have:

- [Node.js](https://nodejs.org/) installed
- Firebase CLI installed:
  ```bash
  npm install -g firebase-tools
  ```
- A Firebase account: [Firebase Console](https://console.firebase.google.com/)

---

## ⚙️ Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/<your-username>/<your-repo>.git
   cd <your-repo>
   ```

2. **Login to Firebase**
   ```bash
   firebase login
   ```

3. **Update Firebase Project ID**
   - Open `.firebaserc`
   - Replace `"your-firebase-project-id"` with your actual Firebase project ID.

---

## ▶️ Running the Project Locally

You can preview your site locally before deploying:

```bash
firebase serve
```

or

```bash
firebase emulators:start
```

The site will be available at [http://localhost:5000](http://localhost:5000).

---

## 🌐 Deploying to Firebase Hosting

Run the following command to deploy your website:

```bash
firebase deploy --only hosting --project your-firebase-project-id
```

After deployment, your site will be live at:

```
https://<your-project-id>.web.app
```
or
```
https://<your-project-id>.firebaseapp.com
```

---

## 📝 Notes

- This project is for **static websites only** (HTML, CSS, JS).  
- For full backend functionality, consider using **Firebase Functions** or **Cloud Run**.  
- Model coefficients or scripts in the public folder are visible to everyone.

---

## 📜 License
This project is licensed under the MIT License — feel free to modify and use it.
