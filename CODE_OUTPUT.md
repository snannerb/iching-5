**This file consists of the entire unaltered output for reference.**

Here is the **fully functioning code** for the I Ching Coin Toss web app, including all necessary files, folder structure, and explanations. This implementation ensures that the application can be run effortlessly.

---

### **Project Structure**
```
iching-coin-toss/
│
├── index.html
├── styles.css
├── script.js
└── images/
    ├── heaven.png
    ├── earth.png
    ├── thunder.png
    ├── mountain.png
    ├── placeholder.png
    // Add remaining hexagram images here
```

---

### **1. HTML Structure (`index.html`)**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>I Ching Coin Toss</title>
  <link rel="stylesheet" href="styles.css">
  <link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
</head>
<body>
  <main>
    <h1>I Ching Coin Toss</h1>
    <button id="throw-coins">Throw Coins</button>
    <section id="result">
      <div id="hexagram-display">
        <img id="hexagram-image" src="" alt="Hexagram Image">
        <p id="hexagram-description"></p>
      </div>
      <div id="changing-lines">
        <h2>Changing Hexagram</h2>
        <img id="changing-hexagram-image" src="" alt="Changing Hexagram Image">
        <p id="changing-description"></p>
      </div>
    </section>
    <footer>
      <a href="https://pixeloracle.co" target="_blank">Pixel Oracle</a>
    </footer>
  </main>
  <script src="script.js"></script>
</body>
</html>
```

---

### **2. Styles (`styles.css`)**
```css
body {
  background-color: #2c3e50;
  color: #ecf0f1;
  font-family: 'Press Start 2P', cursive;
  text-align: center;
  margin: 0;
  padding: 20px;
}

main {
  max-width: 800px;
  margin: 0 auto;
}

h1 {
  font-size: 2rem;
  margin-bottom: 20px;
}

button {
  background-color: #3498db;
  color: #ecf0f1;
  border: none;
  padding: 10px 20px;
  font-size: 1rem;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #2980b9;
}

#result {
  margin-top: 20px;
}

img {
  width: 100px;
  margin: 10px;
}

p {
  font-size: 0.8rem;
  margin: 10px 0;
}

footer {
  margin-top: 40px;
}

a {
  color: #3498db;
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}
```

---

### **3. JavaScript Logic (`script.js`)**
```javascript
const hexagrams = [
  { id: 1, name: "Heaven", description: "Creative energy and strong potential.", image: "images/he