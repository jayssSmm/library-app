
# 📚 JavaScript Library Manager

A simple browser-based library management application built using vanilla JavaScript and object constructors.
Users can add books, remove them, and toggle their read status dynamically.

---

## 📌 Description

This project is a frontend application that demonstrates core JavaScript concepts such as:

* Object constructors and prototypes
* DOM manipulation
* Event delegation
* Form handling
* Dynamic UI updates

Books are stored in an in-memory array and rendered in a table interface.

---

## 🚀 Features

* Add new books via form
* Display books in a table
* Remove books from the library
* Toggle read/unread status
* Unique ID generation using `crypto.randomUUID()`
* Dynamic DOM updates without page reload

---

## 🛠 Tech Stack

* **HTML5**
* **CSS3**
* **Vanilla JavaScript (ES6)**

No frameworks or external libraries used.

---

## 📂 Project Structure

```
library-app/
│
├── index.html
├── styles.css
├── object_constructors.js
└── README.md
```

---

## ⚙️ Installation

1. Clone the repository:

```bash
git clone git@github.com:jayssSmm/myLibrary_js.git
```

2. Navigate to the project directory:

```bash
cd library-app
```

3. Open `index.html` in your browser:

```bash
explorer.exe index.html
```

No dependencies or setup required.

---

## ▶️ Usage

### Add a Book

1. Click **Show Form**
2. Enter:

   * Title
   * Author
   * Pages
   * Read status
3. Submit the form

### Remove a Book

* Click **Remove Book** next to any entry

### Toggle Read Status

* Click the **read/unread button** to switch state

---

## 🧠 How It Works (Technical Overview)

### Book Object

Books are created using an object constructor:

```javascript
function Book(id, title, author, pages, read) {
    this.id = id
    this.title = title
    this.author = author
    this.pages = pages
    this.read = Boolean(read)
}
```

### Library Storage

* All books are stored in an array:

  ```javascript
  const myLibrary = []
  ```

### Rendering

* Books are dynamically rendered into a table using template literals
* UI updates happen without refreshing the page

### Event Handling

* Event delegation is used on the table for:

  * Removing books
  * Toggling read status

---

## ⚠️ Known Issues

* Book removal logic may not correctly identify the index in the array (`indexOf` usage)
* Read status stored as string instead of boolean in toggle
* No persistent storage (data resets on refresh)

---

## 🔮 Future Improvements

* Fix removal logic using `findIndex`
* Store read status as boolean consistently
* Add localStorage for persistence
* Improve UI/UX design
* Add edit functionality
* Add search/filter capability

---

## 📸 Screenshots

![Library UI](screenshot/library-ui.png)


---

## 🤝 Contribution

Contributions are welcome.

1. Fork the repository
2. Create a new branch
3. Submit a pull request

---

## 📄 License

This project is licensed under the MIT License.

---

## 🏁 Portfolio Context

This project demonstrates:

* Understanding of object-oriented JavaScript (constructors & prototypes)
* DOM manipulation and dynamic rendering
* Event delegation patterns
* State management using arrays

It serves as a foundational frontend project for building more complex applications.

---
