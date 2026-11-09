# AltSchool Africa - School of Engineering (Assignment 1)

**Student Name:** Adam Adebowale  
**AltSchool ID:** `ALT/SOE/KAR/026/0228`  
**Program / Track:** AI-Powered Fullstack Engineering  
**Location:** Lagos, Nigeria  
**Email:** adebowaleadam0@gmail.com  

---

## 📁 Project Structure

```text
Altschool assignemnt 1/
├── index.html        # Pure semantic HTML: Profile, Bio, Why Joined, Goals, Top Navigation & Footer
├── form.html         # Pure semantic HTML: AltSchool Registration Form clone, Top Navigation & Footer
└── README.md         # Learning notes & code walkthrough
```

> **Note:** Strictly pure HTML (NO CSS, NO stylesheets, NO inline styles), adhering 100% to assignment constraints.

---

## 🧠 Core Learning Concepts & Code Breakdown

### 1. Global Navigation
- **Where it lives:** In the `<header>` at the top of both `index.html` and `form.html`.
- **How it works:** Uses semantic `<header>`, `<nav>`, and an unordered list `<ul>` with links `<a>` to allow seamless back-and-forth movement between the two pages.

### 2. Fragment Identifier (`#top`)
- **How it works:**
  1. The target element is assigned an ID: `<body id="top">`.
  2. The anchor link references that ID with a hash: `<a href="#top">↑ Back to top</a>`.
  3. When clicked, the browser automatically scrolls the page to the top.

### 3. Accessible Form Elements (`form.html`)
- **Explicit Label Association:** Every input has a unique `id`, and its corresponding `<label>` uses the `for` attribute with the exact same value:
  ```html
  <label for="first-name">First name *</label>
  <input type="text" id="first-name" name="firstName" required>
  ```
- **Semantic Input Types:**
  - `type="email"`: Validates email syntax on mobile and desktop.
  - `type="text"`: For regular text inputs (First and Last name).
  - `type="tel"`: Pulls up numeric/phone keypads on mobile devices.
  - `type="password"`: Masks sensitive characters.
- **Attributes:**
  - `required`: Tells the browser that the field cannot be submitted blank.
  - `placeholder`: Provides a sample hint for the user.
  - `autocomplete`: Enhances accessibility by allowing browsers to autofill user information safely.

### 4. Semantic Footer & `<address>` Tag
- Uses the HTML5 `<footer>` landmark.
- The `<address>` tag is the standard HTML element to represent contact information for the author or owner of the document.
- Contains copyright symbol `&copy;` for standard legal/attribution notice.
