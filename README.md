# Secure & Share Govt Document with Family Members

This project allows users to securely store and share simulated government documents (such as PAN card, passport, mark sheet, etc.) by linking them to a Firebase account. All users must register/login to upload and manage their documents. This version simulates file uploads using URLs (no actual storage).

## 🔧 Technologies Used

* HTML
* CSS
* JavaScript
* Firebase Authentication
* Firebase Firestore (No Storage used)

## 🔐 Features

* User registration and login with Firebase Auth
* Simulated document upload with title + URL
* View your uploaded documents (linked to your account)
* Basic styling and modular HTML + JS

## 🚀 Setup Instructions

### Option 1: Run Online via GitHub Pages (Easy)

1. Go to your GitHub repo: `https://github.com/blitz-blaze7/secure-share-govt-docs`
2. Go to **Settings → Pages**
3. Under **Source**, select the `main` branch and set folder to `/root`
4. Click **Save**
5. After a few seconds, you’ll get a public link like:
   `https://blitz-blaze7.github.io/secure-share-govt-docs/`
6. Open it in a browser

### Option 2: Download and Run Locally

1. Click **Code → Download ZIP**
2. Extract and open the folder
3. Open `index.html` in your browser

## 📂 Firebase Configuration

Firebase is initialized inside the `<script>` of `index.html`:

```js
const firebaseConfig = {
  apiKey: "AIzaSyCCVbi-JPGLBMeXoU-CJ8Uds0zyrBP-_Sc",
  authDomain: "docshare-5cbf3.firebaseapp.com",
  projectId: "docshare-5cbf3",
  storageBucket: "docshare-5cbf3.firebasestorage.app",
  messagingSenderId: "860103685314",
  appId: "1:860103685314:web:6b749c33eeeb1bc0fcf75b"
};
```

## 🧪 Testing Instructions

1. Open the app in browser (GitHub Pages or local)
2. Register a new account
3. Log in
4. Enter title and a dummy document URL (e.g. `https://example.com/doc1.pdf`)
5. Click **"Save Document"**
6. It will appear below as a clickable link

## 🧾 Logging

All user document activity is stored in Firestore with timestamp.

## ⚠️ Notes

* File uploads are simulated using URLs (Firebase Storage not enabled)
* For production, upgrade Firebase and add real storage

## 📜 License

Open-source for academic/demo use only.
