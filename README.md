# 🩸 LifeLink – Emergency Blood Donor Finder

## 📌 Overview

LifeLink is a web-based Emergency Blood Donor Finder designed to help patients and hospitals quickly locate compatible blood donors during emergencies. The system allows users to register as blood donors and enables emergency blood searches based on blood group compatibility and geographic proximity.

The application prioritizes donor privacy by displaying anonymous donor information publicly while revealing contact details only after a valid emergency search.

---

# ✨ Features

* 🩸 Blood donor registration
* 🔍 Emergency blood donor search
* 📍 Location-based donor matching
* ❤️ Blood group compatibility checking
* 📞 Secure donor contact sharing during emergencies
* 🔒 Privacy protection for donor information
* ⚡ Fast and lightweight backend
* 🌐 Responsive web interface

---

# 🛠️ Tech Stack

## Frontend

* HTML5
* CSS3
* JavaScript

## Backend

* Node.js
* Express.js

## Database

* LowDB (JSON Database)

## Additional Packages

* CORS
* UUID

---

# 📂 Project Structure

```text
LifeLink-Emergency-Blood-Donor-Finder
│
├── backend
│   ├── algorithms
│   │   └── matching.js
│   ├── db.json
│   ├── server.js
│   ├── package.json
│   └── README.md
│
├── frontend
│   ├── css
│   ├── js
│   ├── images
│   └── index.html
│
└── README.md
```

---

# 🚀 Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/LifeLink-Emergency-Blood-Donor-Finder.git
```

## Navigate to Project

```bash
cd LifeLink-Emergency-Blood-Donor-Finder/backend
```

## Install Dependencies

```bash
npm install
```

## Start Server

```bash
npm start
```

The application will start on:

```
http://localhost:4000
```

Open the URL in your browser.

---

# 📌 API Endpoints

## Register Donor

**POST**

```
/api/donors
```

Request Body

```json
{
  "name":"John",
  "bloodType":"O+",
  "phone":"9876543210",
  "lat":12.914,
  "lng":74.856
}
```

---

## View Donors

**GET**

```
/api/donors
```

Returns anonymized donor information.

---

## Emergency Search

**POST**

```
/api/emergency-search
```

Example

```json
{
  "bloodType":"A+",
  "lat":12.91,
  "lng":74.85,
  "urgency":"High",
  "radiusKm":20,
  "topK":5
}
```

---

# 🧠 Matching Algorithm

The donor matching algorithm considers:

* Blood group compatibility
* Donor eligibility
* Geographic distance
* Donor availability
* Search radius
* Emergency priority

The system returns the nearest compatible donors first.

---

# 🔐 Privacy Features

* Public users cannot view donor names.
* Phone numbers remain hidden.
* Personal information is revealed only after an emergency match.
* Anonymous donor IDs are used for public listings.

---

# 🎯 Future Enhancements

* GPS integration
* Google Maps support
* SMS notifications
* Email alerts
* Hospital portal
* Blood bank integration
* Mobile application
* Authentication system
* Admin dashboard
* Real-time donor availability

---

# 💻 Requirements

* Node.js 18+
* npm
* Modern Web Browser

---

# ▶️ Running the Project

### Backend

```bash
cd backend
npm install
npm start
```

### Frontend

The frontend is served automatically by the Express server.

Visit:

```
http://localhost:4000
```

---

# 📷 Screenshots

Add screenshots of:

* Home Page
* Donor Registration
* Emergency Search
* Search Results
* About Section

---

# 👨‍💻 Author

**Surya Nandu**

Computer Science & Data Science Engineering

---

# 🤝 Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

---

# 📄 License

This project is developed for educational and academic purposes.

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.
