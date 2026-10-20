# 🏠 Regents Court Locksmiths – Landlord Maintenance App

> ⚠️ IMPORTANT TEAM NOTICE ON GIT WORKFLOW:
> can NOT wait for University GitLab access to begin working!*

---

## 📌 Project Overview & Purpose

We are developing a specialized, **offline-first Android mobile application** (supporting Android version 16+) commissioned by **Regents Court Locksmiths** for private landlords managing small rental property portfolios[cite: 1, 2].

### Why are we building this?
Landlords are often hesitant to register their personal and property details on centralized cloud databases[cite: 2]. Additionally, landlords frequently need access to property maintenance details in areas with poor or zero mobile coverage (e.g., basements, rural sites)[cite: 2].

Our app solves this by operating **100% locally on the device** without requiring a central server or user login wall, allowing landlords to track properties, document damage, and automatically generate structured repair request emails[cite: 1, 2].

---

## 🎯 Primary Goals & Core Features

### 1. Property Portfolio Management
* **Add New Properties:** Store full street addresses, live/map-based geolocations, access notes (e.g., key location/entry codes), tenant contact numbers, and property photos[cite: 2].
* **Archive & Update:** Allow landlords to hide (archive) sold properties while keeping historical records intact, and edit details to fix mistakes[cite: 2].

### 2. Repair Request Logging
* **Damage Documentation:** Log repairs linked to specific properties including textual descriptions, damage photos, and live GPS timestamps[cite: 2].
* **Filter & Sort:** Enable landlords to sort listings (e.g., by date) and filter repairs by status (e.g., *Requested*, *Quoted*, *In Progress*, *Completed*)[cite: 2].

### 3. Automated Repairer Emailing
* **Email Intent Generator:** Automatically compile property addresses, repair types, and damage details into a pre-filled email addressed to chosen locksmiths/repairers[cite: 2].
* **Landlord Control:** Hand off the generated request directly to the phone's standard email app so the landlord can review and edit before sending[cite: 2].

### 4. Partner Directory & Client Support
* Shortlist trusted repair partners with web links to view services[cite: 2].
* Provide direct contact options (Email, Phone/SMS, Website) for Regents Court Locksmiths[cite: 2].
* Full support for standard Android App Backup[cite: 2].

---

## 🏗️ Architecture & Technical Constraint Checklist

* [x] **Platform:** Android (Version 16+ / API level 16+)[cite: 2].
* [x] **Database:** Local SQLite / Room Database (strictly on-device)[cite: 2].
* [x] **Auth:** NO login, NO user registration, NO mandatory cloud dependency[cite: 1, 2].
* [x] **Hardware Access:** Camera (damage photos), GPS/Location (geolocation stamping)[cite: 2].
* [x] **External Actions:** Android Email Intents, Web Browser Intents[cite: 2].

---

## 👥 Team Action Plan & Next Steps

### 🎨 UI/UX & Frontend Team
* Design wireframes and screens for:
  1. **Dashboard:** Property list with status badges, sorting, and filtering[cite: 2].
  2. **Property Details:** House details, tenant contacts, access notes, and repair history list[cite: 2].
  3. **Repair Form:** Form input for descriptions, photo capture button, and GPS stamp indicator[cite: 2].
  4. **Directory/Utils:** Repairer links and company contact options[cite: 2].

### ⚙️ Android & Backend Team
* Set up the Android Studio project targeting Android 16+[cite: 2].
* Design local database schemas (Entities: `Property` and `RepairRequest`).
* Implement local image storage handling and GPS location services.
* Build the `EmailIntentHelper` class to format repair emails[cite: 2].

---

## 🚀 How to Get Started Now

1. **Clone this repository:**
   ```bash
   git clone <REPOSITORY_URL>
