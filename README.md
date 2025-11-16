# 🎨 Dynamic Portfolio Generator

A professional web-based portfolio generator with Firebase authentication, allowing users to create, save, and download their portfolios as PDF documents.

![Portfolio Generator](https://img.shields.io/badge/Version-1.0-blue) ![Firebase](https://img.shields.io/badge/Firebase-Integrated-orange) ![License](https://img.shields.io/badge/License-MIT-green)

## 📖 Overview

The Dynamic Portfolio Generator is a full-stack web application that enables users to create professional portfolios through an intuitive form interface. Users can register, log in, build their portfolios with multiple sections, and download them as beautifully formatted PDF files. All data is securely stored in Firebase Firestore for future access.

## ✨ Features

### Authentication System (Task-1)
- ✅ **User Registration** - Create new accounts with email/password authentication
- ✅ **Duplicate Email Detection** - Alert users if email already exists before account creation
- ✅ **Secure Login** - Email/password verification with detailed error messages
- ✅ **Session Management** - Automatic login persistence and secure logout
- ✅ **Access Control** - Portfolio builder accessible only to authenticated users

### Portfolio Management (Task-2)
- ✅ **PDF Generation** - Download professional portfolios as PDF files
- ✅ **Auto-Save** - Portfolio data automatically saved to Firestore on generation
- ✅ **Manual Save** - "Save Progress" button to save anytime
- ✅ **Auto-Load** - Previously saved data loads automatically on login
- ✅ **Real-time Preview** - See portfolio before downloading

### Advanced Features
- ✅ **Multiple Academic Backgrounds** - Add/remove unlimited education entries
- ✅ **Multiple Projects** - Add/remove unlimited project entries
- ✅ **Dynamic Form Fields** - Smooth add/remove animations
- ✅ **Responsive Design** - Works on desktop, tablet, and mobile
- ✅ **Professional UI** - Clean black & off-white theme with smooth animations
- ✅ **Error Handling** - User-friendly error messages and loading states

## 🛠️ Technologies Used

**Frontend:**
- HTML5
- CSS3 (Custom animations & responsive design)
- JavaScript (ES6+)
- Font Awesome Icons

**Backend & Services:**
- Firebase Authentication (Email/Password)
- Firebase Firestore Database
- Firebase SDK v10.7.1

**Libraries:**
- jsPDF 2.5.1 (PDF generation)

## 📦 Installation & Setup

### 1. Download the File
Download `Portfolio-Generator-ERROR-FIXED.html` from the project files.

### 2. Firebase Configuration (Already Configured)
The Firebase project is already set up with these credentials:
- **Project ID**: portfolio-generator-f1fc3
- **Auth Domain**: portfolio-generator-f1fc3.firebaseapp.com
- **API Key**: Already configured in the code

### 3. Enable Firebase Services

#### Enable Email/Password Authentication:
1. Go to [Firebase Console](https://console.firebase.google.com/)
2. Select project: **portfolio-generator-f1fc3**
3. Navigate to **Build** → **Authentication**
4. Click **Sign-in method** tab
5. Enable **Email/Password** provider
6. Click **Save**

#### Enable Firestore Database (Optional - for Save feature):
1. In Firebase Console, go to **Build** → **Firestore Database**
2. Click **Create Database**
3. Select **Start in test mode** (for development)
4. Choose a location closest to your users
5. Click **Enable**

### 4. Run the Application
Simply open `Portfolio-Generator-ERROR-FIXED.html` in any modern web browser:
- Google Chrome (Recommended)
- Mozilla Firefox
- Microsoft Edge
- Safari

**No server setup required!** The application runs entirely in the browser.

## 🚀 Usage Guide

### First Time User

1. **Open the application** in your browser
2. **Create Account**:
   - Click "Create Account" link
   - Enter email and password (minimum 6 characters)
   - Confirm password
   - Click "Create Account"
   - You'll be automatically logged in

3. **Build Your Portfolio**:
   - Fill in **Personal Information** (name, email, phone, bio)
   - Upload **Profile Photo** (optional but marked required)
   - Add **Skills** (soft skills and technical skills)
   - Click **"Add Academic Background"** to add education (multiple entries supported)
   - Fill **Work Experience** details
   - Click **"Add Project"** to add projects (multiple entries supported)

4. **Generate & Download**:
   - Click **"Generate Portfolio"** to see preview
   - Review your portfolio
   - Click **"Download PDF"** to save as PDF file
   - Your data is automatically saved!

### Returning User

1. **Login**:
   - Enter your registered email and password
   - Click "Login"
   - Your previous portfolio data loads automatically

2. **Edit & Update**:
   - Modify any section
   - Add/remove academic backgrounds or projects
   - Click **"Save Progress"** to save changes
   - Or click **"Generate Portfolio"** to save and preview

3. **Download Updated Portfolio**:
   - Generate preview
   - Download updated PDF

## 📝 Form Sections

| Section | Required | Multiple Entries | Description |
|---------|----------|------------------|-------------|
| Personal Info | Yes | No | Name, email, phone, photo, bio |
| Skills | Yes | No | Soft skills & technical skills |
| Academic Background | No | Yes | Institute, degree, year, grade |
| Work Experience | Yes | No | Company, duration, title, responsibilities |
| Projects | No | Yes | Name, description, technologies |

## 🎯 Task Requirements Completion

### ✅ Task-1: Authentication
- **1.1** Registration page with authentication ✓
- **1.2** Email/password required to access resume form ✓
- **1.3** Alert for duplicate email during registration ✓
- **1.4** Login page with credential verification ✓

### ✅ Task-2: Portfolio Features
- **2.1** Generate portfolio as PDF file ✓
- **2.2** Save tasks to database (Firestore) ✓
- **2.2** Load saved information on return ✓

## 🐛 Troubleshooting

### "Error generating portfolio. Please try again."
**Solution**: This is now fixed in the latest version. The portfolio generates even if Firestore is not set up.

### "Auth/admin-restricted-operation" error
**Solution**: Enable Email/Password authentication in Firebase Console (see Installation step 3).

### Save Progress doesn't work
**Solution**: Set up Firestore Database (see Installation step 3.2). Note: Portfolio generation and PDF download work without Firestore.

### PDF doesn't download
**Solution**: 
- Ensure you've filled all required fields (marked with *)
- Check browser's download settings
- Allow pop-ups and downloads for the site

### Login doesn't work
**Solution**: 
- Verify Email/Password authentication is enabled in Firebase Console
- Check email format is valid
- Password must be at least 6 characters
- Try clearing browser cache and cookies

## 🔒 Security Notes

- Passwords are handled securely by Firebase Authentication
- Test mode Firestore rules should be updated for production
- No sensitive data is stored in client-side code
- Firebase API key is safe for public exposure (it's a client key)

## 🎨 Customization

### Changing Colors
Edit the CSS variables in the `<style>` section:
