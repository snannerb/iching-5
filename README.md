# iching 5

## About
This code was generated by [CodeCraftAI](https://codecraft.name)

**User requests:**
create web app that allows user to replicate the I ching coin toss. Allow image to be imported for all 64 hexagrams. After user clicks "Throw Coins" Button the hexagram image appears with description of hexagram and a Changing line description when needed along with second hexagram image. Use pixel font. Use grey background. Create app with only HTML, CSS, JavaScript. At bottom of app Include link code  <a href="https://pixel-oracle.com/" target="_blank" rel="noopener noreferrer">Visit Pixel Oracle</a> .

Check OUTPUT.md for the complete unaltered output.

## Project Plan
```
Here’s a **simple and clear project plan** for the I Ching coin toss web app, based on the requirements provided. The plan is broken into **main tasks** and includes **technical considerations** for each step.

---

### **Project Plan**

#### **1. Set Up Project Structure**  
**Tasks:**  
- Create the following files:  
  - `index.html` (for HTML structure)  
  - `styles.css` (for styling)  
  - `script.js` (for JavaScript logic)  
- Link the files together in the HTML file.  

**Technical Considerations:**  
- Use a `<script>` tag to link the JavaScript file.  
- Use a `<link>` tag to include the CSS file.  

---

#### **2. Create the HTML Structure**  
**Tasks:**  
- Create a container for the app in `index.html`.  
- Add:  
  - A heading (`<h1>`).  
  - A "Throw Coins" button (`<button>`).  
  - A section to display the hexagram image and description.  
  - A footer with the link to "Pixel Oracle".  

**Technical Considerations:**  
- Use semantic HTML elements (`<main>`, `<section>`, `<footer>`).  
- Ensure the link in the footer opens in a new tab with `target="_blank"`.  

---

#### **3. Style the App**  
**Tasks:**  
- Apply a grey background to the body or main container.  
- Use a pixel font (e.g., `Press Start 2P` from Google Fonts).  
- Style the button and text elements for visual consistency.  

**Technical Considerations:**  
- Import the pixel font using Google Fonts via a `<link>` tag.  
- Use `text-align: center` to center-align content.  
- Ensure the footer link is styled and remains visible.  

---

#### **4. Set Up Hexagram Data**  
**Tasks:**  
- Create a JavaScript array or object to store the 64 hexagrams and their descriptions.  
- Include changing line descriptions if applicable.  
- Ensure each hexagram points to its corresponding image.  

**Technical Considerations:**  
- Store the hexagram data as key-value pairs, e.g.:  
  ```javascript
  const hexagrams = [
    { id: 1, name: "Heaven", description: "Description here", image: "heaven.png" },
    { id: 2, name: "Earth", description: "Description here", image: "earth.png" },
    // ... up to 64
  ];
  ```  
- Host hexagram images in the project folder and reference them by filename.  

---

#### **5. Implement Coin Toss Logic**  
**Tasks:**  
- Simulate the I Ching coin toss process using random number generation.  
- Determine the hexagram and any changing lines based on the result.  
- Map the results to the corresponding hexagram image and description.  

**Technical Considerations:**  
- Use `Math.random()` to simulate coin tosses (e.g., 2 = heads, 3 = tails).  
- Calculate the hexagram and changing lines based on the toss results.  

---

#### **6. Update the DOM with Results**  
**Tasks:**  
- Dynamically display the hexagram image, description, and changing line (if applicable) in the app.  
- Ensure the second hexagram image is shown if there’s a changing line.  

**Technical Considerations:**  
- Use JavaScript to manipulate the DOM (`document.getElementById`, `innerHTML`, etc.).  
- Dynamically load hexagram images using the `<img>` element.  

---

#### **7. Test and Debug**  
**Tasks:**  
- Test the app in multiple browsers for compatibility.  
- Ensure the coin toss logic is accurate and the correct hexagram is displayed.  
- Verify that the app is responsive and visually consistent.  

**Technical Considerations:**  
- Use browser developer tools to debug JavaScript and CSS.  

---

### **Timeline**  
| **Task**                      | **Estimated Time** |  
|-------------------------------|-------------------|  
| Set Up Project Structure       | 1 hour            |  
| Create HTML Structure          | 1 hour            |  
| Style the App                  | 2 hours           |  
| Set Up Hexagram Data           | 2 hours           |  
| Implement Coin Toss Logic     | 3 hours           |  
| Update the DOM with Results    | 2 hours           |  
| Test and Debug                 | 2 hours           |  

**Total Estimated Time:** **13 hours**

---

### **Optional Enhancements**  
1. Add animations when the "Throw Coins" button is clicked.  
2. Include a history of past hexagram readings.  
3. Add sound effects for the coin toss.  

Let me know if you’d like further assistance with any specific task!
```
