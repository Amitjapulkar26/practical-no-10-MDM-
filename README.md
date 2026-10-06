```markdown
# 🔎 CampusFind

<p align="center">
  <img src="https://img.shields.io/badge/Practical-10-4F46E5?style=for-the-badge" alt="Practical 10">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/GitHub-Pages-181717?style=for-the-badge&logo=github" alt="GitHub Pages">
</p>

<h2 align="center">Smart Lost & Found Platform for College Campuses</h2>

<p align="center">
  A responsive and interactive frontend web application developed to solve
  a real-world campus Lost & Found problem.
</p>

<p align="center">
  <strong>Report • Search • Match • Reconnect</strong>
</p>

---

## 📚 Practical Information

| Details | Information |
|---|---|
| **Practical No.** | 10 |
| **Practical Type** | Post-Lab |
| **Subject** | Web Fundamentals and Basic Frontend Design |
| **Course Code** | N-MDMWD301P |
| **Project Name** | CampusFind |
| **Project Type** | Frontend Web Application |
| **Domain** | Campus Utility |
| **Academic Year** | 2026–27 |
| **Institute** | S. B. Jain Institute of Technology, Management & Research, Nagpur |

---

## 🎯 AIM

> Create a frontend web application based on a real-world problem or personal interest using HTML, Tailwind CSS, and JavaScript, incorporating responsive design and client-side interactivity.

### Project Implementation

**CampusFind** is developed as a digital Lost & Found platform for college campuses. It allows students to report lost or found belongings, search existing reports, filter items and mark successfully identified items as matched.

---

## 💡 Problem Statement

Students commonly lose items such as ID cards, calculators, notebooks, USB drives, keys and other personal belongings.

Usually, information about these items is scattered across WhatsApp groups, classroom groups or personal communication.

This makes it difficult to:

- Find previously reported items
- Search for a specific item
- Know where an item was found
- Track whether an item has been matched
- Maintain an organized record

### 💡 Proposed Solution

CampusFind provides a centralized and responsive platform where students can **report, search, filter and match** Lost & Found items.

---

## 🎯 Objectives

- To develop a frontend web application using HTML.
- To design a modern responsive interface using Tailwind CSS.
- To implement client-side interactivity using JavaScript.
- To solve a practical real-world campus problem.
- To implement dynamic content rendering.
- To implement search and filtering functionality.
- To use LocalStorage for client-side data persistence.
- To create a responsive interface for desktop, tablet and mobile devices.
- To integrate HTML, Tailwind CSS and JavaScript into a functional application.

---

## 🧠 Theory

### HTML5

HTML5 is used to create the structure of the CampusFind application.

The project uses elements such as:

```html
<header>
<nav>
<section>
<main>
<div>
<input>
<select>
<button>
<img>
```

These elements organize the content and user interface.

### Tailwind CSS

Tailwind CSS is a utility-first CSS framework used for:

- Layout
- Spacing
- Colors
- Typography
- Shadows
- Borders
- Responsive design
- Grid and Flexbox
- Hover effects

Example:

```html
<div class="grid grid-cols-2 md:grid-cols-4 gap-4">
```

### JavaScript

JavaScript provides the client-side functionality of CampusFind.

It handles:

- Adding reports
- Displaying reports
- Searching
- Filtering
- Updating statistics
- Matching items
- Deleting reports
- Opening and closing forms
- Notifications
- LocalStorage

### LocalStorage

LocalStorage is used to save reports inside the user's browser.

```javascript
localStorage.setItem(
  "campusItems",
  JSON.stringify(items)
);
```

Data can be retrieved using:

```javascript
JSON.parse(
  localStorage.getItem("campusItems")
);
```

---

## ✨ Features

| Feature | Description |
|---|---|
| 🔴 Lost Reports | Report items that have been lost |
| 🟢 Found Reports | Report items found on campus |
| 🔍 Search | Search by item name or location |
| 🏷️ Category Filter | Filter reports by category |
| 🔄 Type Filter | Filter Lost and Found reports |
| 📊 Dashboard | Display live report statistics |
| 🤝 Match System | Mark successfully identified items |
| 🗑️ Delete | Remove unwanted reports |
| 💾 LocalStorage | Store reports in the browser |
| 🖼️ Images | Display item images |
| 🔔 Notifications | Provide action feedback |
| 📱 Responsive UI | Adapt to different screen sizes |

---

## 🎨 User Interface

CampusFind contains:

### 🧭 Navigation Bar
Provides the application identity and report-item action.

### 🌈 Hero Section
Introduces CampusFind and provides a quick option to report an item.

### 📊 Statistics Dashboard

Displays:

```text
Total Reports
Lost Items
Found Items
Matched Items
```

### 🔎 Search & Filter

Users can search by item name or location and filter reports by type and category.

### 🃏 Item Cards

Each card displays:

- Item image
- Item name
- Lost / Found status
- Location
- Category
- Match button
- Delete button

### 📝 Report Modal

Allows users to enter item information and publish a new report.

---

## 🔄 Application Workflow

```text
                    👨‍🎓 USER
                       │
                       ▼
              ┌──────────────────┐
              │   Report Item    │
              └────────┬─────────┘
                       │
                       ▼
              ┌──────────────────┐
              │  Enter Details   │
              └────────┬─────────┘
                       │
                       ▼
              ┌──────────────────┐
              │  Store Item Data │
              └────────┬─────────┘
                       │
                       ▼
              ┌──────────────────┐
              │ Display Item Card│
              └────────┬─────────┘
                       │
             ┌─────────┼─────────┐
             ▼         ▼         ▼
          🔍 Search  🏷️ Filter  🤝 Match
             │         │         │
             └─────────┼─────────┘
                       ▼
              ┌──────────────────┐
              │ Update Dashboard │
              └────────┬─────────┘
                       │
                       ▼
              ┌──────────────────┐
              │   LocalStorage   │
              └──────────────────┘
```

---

## 🧩 Main JavaScript Functions

| Function | Purpose |
|---|---|
| `addItem()` | Adds a new Lost/Found report |
| `showItems()` | Displays and filters reports |
| `matchItem()` | Marks an item as matched |
| `deleteItem()` | Deletes a report |
| `updateStats()` | Updates dashboard statistics |
| `setFilter()` | Changes the report filter |
| `save()` | Saves data to LocalStorage |
| `openForm()` | Opens the report form |
| `closeForm()` | Closes the report form |
| `toast()` | Displays action notifications |

---

## 📱 Responsive Design

The application uses Tailwind CSS responsive utilities.

| Device | Layout |
|---|---|
| 💻 Desktop | Multi-column dashboard and item cards |
| 📟 Tablet | Adaptive grid layout |
| 📱 Mobile | Single-column responsive layout |

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **HTML5** | Application structure |
| **Tailwind CSS** | Styling and responsive design |
| **JavaScript** | Client-side functionality |
| **LocalStorage** | Browser-based data persistence |
| **Unsplash** | Demo images |
| **GitHub** | Source code management |
| **GitHub Pages** | Deployment |

---

## 📂 Project Structure

```text
practical-no-10-MDM-
│
├── index.html
└── README.md
```

### `index.html`

Contains the complete CampusFind application including:

- HTML structure
- Tailwind CSS classes
- JavaScript functionality
- LocalStorage logic
- Responsive interface

### `README.md`

Contains the complete project documentation and practical information.

---

## 🚀 How to Run

### Using VS Code Live Server

1. Clone the repository.
2. Open the project in Visual Studio Code.
3. Open `index.html`.
4. Install the Live Server extension if required.
5. Right-click `index.html`.
6. Select **Open with Live Server**.

### Using a Browser

Open:

```text
index.html
```

directly in a modern browser.

No backend or database is required.

---

## 🌐 Live Website

### 🔗 Deployed Application

**https://amitjapulkar26.github.io/practical-no-10-MDM-/**

### 💻 Source Code

**https://github.com/Amitjapulkar26/practical-no-10-MDM-**

The project is deployed using **GitHub Pages** with `index.html` as the main entry page.

---

## 📸 Output Screenshots

> Add your actual screenshots inside a `docs` folder and update the paths below.

### 🏠 CampusFind Dashboard

![CampusFind Dashboard](docs/dashboard.png)

### 🔎 Search & Filter

![CampusFind Search and Filter](docs/search.png)

### 🤝 Matched Item

![CampusFind Matched Item](docs/matched.png)

---

## 🔗 Source Code GitHub Repository

The complete source code is available at:

**https://github.com/Amitjapulkar26/practical-no-10-MDM-/**

---

## 📱 GitHub Repository QR Code

Add the generated repository QR code as:

```text
docs/github-qr.png
```

Then it can be displayed using:

```markdown
![GitHub Repository QR Code](docs/github-qr.png)
```

---

## 📊 Sample Reports

| Item | Location | Type | Category |
|---|---|---|---|
| 🪪 Student ID Card | CSE Block | 🔴 Lost | ID Card |
| 🧮 Scientific Calculator | Mathematics Lab | 🟢 Found | Electronics |
| 📓 Black Notebook | Central Library | 🔴 Lost | Stationery |
| 💾 USB Drive | Computer Lab | 🟢 Found | Electronics |

---

## 💾 Data Storage

CampusFind uses browser LocalStorage for client-side persistence.

```javascript
localStorage.setItem(
  "campusItems",
  JSON.stringify(items)
);
```

### Important

- Data remains after refreshing the page.
- Data is stored locally in the current browser.
- Data is not synchronized between devices.
- Clearing browser site data removes the stored reports.

---

## 📈 Learning Outcomes

After completing this practical, the following concepts were implemented:

- HTML5 structure
- Tailwind CSS
- Responsive web design
- JavaScript functions
- Arrays and objects
- DOM manipulation
- Event handling
- Dynamic content rendering
- Search and filtering
- Conditional rendering
- LocalStorage
- Client-side interactivity
- GitHub repository management
- GitHub Pages deployment

---

## 🔮 Future Scope

The application can be extended with:

- 🔐 Student authentication
- 👤 User profiles
- ☁️ Cloud database
- 📷 Direct image upload
- 📧 Email notifications
- 🔔 Real-time notifications
- 🗺️ Campus map integration
- 🛡️ Admin moderation dashboard
- 📱 Progressive Web App support
- 🔄 Real-time synchronization

---

## 📝 Conclusion

The **CampusFind** frontend web application successfully demonstrates the development of a responsive and interactive real-world web application using **HTML, Tailwind CSS and JavaScript**.

The application provides an organized solution for reporting, searching, filtering and matching lost and found items within a college campus.

The project also demonstrates client-side data management using **LocalStorage**, responsive design using **Tailwind CSS**, and dynamic interface updates using **JavaScript**.

---

## 📚 References

1. HTML5 Documentation
2. Tailwind CSS Documentation
3. JavaScript Documentation
4. MDN Web Docs
5. GitHub Documentation
6. GitHub Pages Documentation

---

## 👨‍💻 Developer

### Amit Gajanan Japulkar

**CSE (AI & ML)**  
**S. B. Jain Institute of Technology, Management & Research, Nagpur**

**Academic Year:** 2026–27

---

## ⭐ Project Highlights

```text
                 🔎 CAMPUSFIND
                       │
        ┌──────────────┼──────────────┐
        │              │              │
      REPORT         SEARCH         MATCH
        │              │              │
        └──────────────┼──────────────┘
                       │
                       ▼
                   RECONNECT
```

### Report • Search • Match • Reconnect

---

<p align="center">

## 🔎 CampusFind

<strong>Smart Lost & Found for College Campuses</strong>

<br><br>

Made with ❤️ using

<strong>HTML • Tailwind CSS • JavaScript</strong>

<br><br>

<sub>Practical No. 10 • Post-Lab • Academic Year 2026–27</sub>

</p>
```
