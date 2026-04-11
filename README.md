
# 📱 KharchaApp — Smart way to track every rupee

Take charge of your daily spending with just one tap. A smart personal expense management application built with Flutter, designed to help users efficiently track, analyze, and manage their daily spending with powerful insights and automation.


---

## 📲 Download Kharcha App now: 
### Google Play Store
https://play.google.com/store/apps/details?id=com.shafqat.kharcha


---

## 📅 Overview

Kharcha App enables users to:

* Track grocery and utility expenses
* Manage bill plans
* Analyze spending patterns
* Automate alerts and reminders
* Backup and restore financial data

The app focuses on **simplicity + powerful analytics**, making it suitable for everyday users as well as advanced budget planners.

---

## 📅 Key Features

### 🧾 Bill & Expense Management

* Create and manage multiple bill plans
* Store detailed item-level purchase data
* View complete bill breakdown in a dedicated page
* Smart bill selection using:

  * 🔍 Search-based selection (for 1000+ bills)
  * 📅 Month-wise filtering
  * 🔤 Alphabetical grouping (by first letter)

---

### 🛍️ Live Shopping Mode

* Maintains Live shopping lists that update as you buy


---

### 📦 Item Tracking

* Maintain structured item data (name, Urdu, Roman, category, image)
* Track:

  * Quantity
  * Unit (kg, liter, etc.)
  * Price per item
* Dynamic total calculation per bill

---

### 📊 Analytics & Insights

* Category-wise consumption (Pie Chart)
* Spending distribution visualization
* Total cost and item count summaries
* Future-ready structure for advanced analytics

---

### 🔔 Smart Notifications System

* Background alerts using WorkManager
* JSON-driven alert configuration
* Periodic notifications (minute/hour/day/week)
* Works even when app is closed

---

### 💾 Backup & Restore

* Export app data into a compressed file
* Share backup via external apps (e.g., messaging apps)
* Restore data with:

  * File picker support
  * Selective restore options (checkbox-based)
* Maintains file structure and integrity

---

### 🧾 Receipt Management

* Add and store receipt images
* Full-screen preview with zoom support
* Persistent local storage

---

### ⚙️ Utility Bills Management

* Track recurring bills (electricity, gas, etc.)
* JSON-based utility definitions
* Monthly tracking support

---

### 🧠 Smart Filtering Engine

* Filter by:

  * Category
  * Utility type
  * Date/month
* Efficient data handling from local JSON files

---

## 🏗️ Technical Architecture

### 📱 Frontend

* Flutter (Dart)
* Material UI components
* Stateful + modular widget structure

---

### 📂 Data Storage

* Local JSON files:

  * `plans.json` → Bill plans
  * `items.json` → Master item list
  * `userutilitybills.json` → Utility tracking
  * `alert.json` → Notification config

* File storage handled via:

  * `path_provider`

---

### 🔄 Background Processing

* `workmanager` for background tasks
* Periodic notification scheduling
* Independent execution from UI thread

---

### 🔊 Speech Support

* SSML-based speech integration (planned/partial)

---

### 📊 Data Handling

* JSON parsing and mapping
* Functional-style processing (fold, map, filter)
* Null-safe handling and validation

---

## 🧰 Tech Stack

| Layer            | Technology               |
| ---------------- | ------------------------ |
| UI Framework     | Flutter                  |
| Language         | Dart                     |
| Storage          | Local JSON + File सिस्टम |
| Background Jobs  | WorkManager              |
| Charts           | Flutter chart libraries  |
| Notifications    | Local Notifications      |
| File Handling    | Path Provider            |
| State Management | Stateful Widgets         |

---

## ⚙️ Setup & Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-repo/kharcha-app.git
cd kharcha-app
```

---

### 2️⃣ Install Dependencies

```bash
flutter pub get
```

---

### 3️⃣ Run App

```bash
flutter run
```

---

## 📦 Build & Release (Android)

### 🔐 Generate Release Build

```bash
flutter build appbundle
```

---

### 📁 Output File

```
build/app/outputs/bundle/release/app-release.aab
```

---

### 🔑 Keystore Setup

* Generate keystore:

```bash
keytool -genkey -v -keystore key.jks -keyalg RSA -keysize 2048 -validity 10000 -alias key
```

* Configure in:

  * `android/key.properties`
  * `build.gradle`

---

### ☁️ Play Store Deployment Steps

1. Create app in Developer Console
2. Upload `.aab` file
3. Configure:

   * App content
   * Privacy policy
   * Data safety
4. Add:

   * Screenshots
   * App description
5. Release to production

---

## 🔒 Security Considerations

* Code obfuscation enabled for release builds
* Uses AAB (split APKs) for better protection
* No sensitive logic exposed in plain text
* Local data storage (no external API dependency)

---

## 📈 Performance Considerations

* Lazy loading via `ListView.builder`
* Efficient JSON parsing
* Optimized UI rendering
* Handles large datasets (1000+ bills)

---

## 🧪 Future Enhancements

* Cloud sync
* AI-based expense insights
* Voice-based expense entry
* Multi-user support
* Advanced reporting dashboard

---

## 👨‍💻 Developer Notes

* Modular and scalable architecture
* JSON-driven configuration system
* Easy to extend for new features
* Designed for offline-first usage

---

## 📄 License

This project is licensed for personal and commercial use.

---

## 🤝  (Contribution)

Contributions, suggestions, and improvements are welcome.

---

## 📬 Contact

For support or queries, reach out via your preferred channel or shafqatgreat@gmail.com

---

**Kharcha App — Smart way to track every rupee.**
