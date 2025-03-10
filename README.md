# MediScan - Medication Management App

## Core Features

### 📷 Camera Interface with OCR Text Extraction
- Use the device camera to scan prescription labels.
- Integrate Optical Character Recognition (OCR) to extract medication details:
  - Drug name
  - Dosage
  - Frequency

#### 📚 Libraries:
- `react-native-camera` or `expo-camera` for camera functionality.
- `tesseract.js` or `Google Cloud Vision API` for OCR processing.

---

### 📋 Dashboard for Active Medications
- Displays a list of active medications with:
  - **Drug name**
  - **Dosage instructions**
  - **Next scheduled dose time**
- Includes an "Add Medication" button for manual entry if scanning fails.

---

### 🔔 Push Notification System
- Sends reminders for upcoming doses.
- Provides action buttons:
  - ✅ **Taken**: Logs the dose and updates adherence history.
  - ❌ **Skip**: Skips the dose and reschedules the next reminder.

#### 📚 Libraries:
- `expo-notifications` or `react-native-push-notifications` for handling push notifications.

---

### 📅 Medication Tracking Calendar
- Displays a calendar view with adherence history:
  - 🟢 **Green** for taken doses
  - 🔴 **Red** for missed doses
- Allows users to tap a date to view medication details.

#### 📚 Libraries:
- `react-big-calendar` (for web) or `react-native-calendars` (for mobile).

---

## 🎨 Design and Accessibility

### 🎨 Color Palette
| Element        | Color Code |
|---------------|------------|
| Primary       | `#007AFF` (Blue for buttons and highlights) |
| Background    | `#FFFFFF` (White for clarity) |
| Secondary     | `#F0F4F8` (Light gray for backgrounds) |
| Accent        | `#00C853` (Green for success, e.g., "Taken" actions) |
| Error         | `#FF3B30` (Red for missed doses or errors) |

### 🔤 Typography
- Minimum **16px** font size for body text.
- Use **sans-serif** fonts like `Roboto` or `Open Sans` for clarity.

### ♿ Accessibility
- Ensure **high contrast** between text and background.
- Implement **ARIA labels** for screen readers.
- Provide **alternative text** for icons and images.

---

## ⚙️ Tech Stack

### 🖥️ Frontend
- **Framework:** React Native (for cross-platform mobile development)

### 🔙 Backend
- **Options:**
  - Firebase
  - Lightweight Node.js server
- **Responsibilities:**
  - Store user data (medications, reminders, adherence history)
  - Handle push notifications

### 🗄️ Database
- Firebase Firestore or PostgreSQL for storing medication and user data.

### 🔍 OCR Processing
- `tesseract.js` (open-source) or `Google Cloud Vision API` (more accurate).

### 🏗️ State Management
- **Options:**
  - Redux Toolkit
  - React Context API (for managing global state, e.g., medications, reminders)

---

## 📄 License
This project is licensed under the MIT License.

---

## 👥 Contributors
- [Eric Kuo](https://github.com/Erickuokuo)

---

🚀 *MediScan – Simplifying Medication Management!*
