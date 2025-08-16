# 🍔 The Box Model — Davie’s Burgers  

A hands-on CSS box model exercise where I styled a fictional burger restaurant’s menu page.  I have practiced applying **height, width, padding, border, and margin** to polish the layout.  

---

## 📸 Preview  
![Project Screenshot](https://content.codecademy.com/courses/web-101/unit-6/htmlcss1-img_burgerphoto.jpeg)  

---

## 🗂️ Project Structure  

davies-burgers-box-model/
├─ index.html
├─ style.css
└─ reset.css
---

---

## ▶️ Live Demo  
[![Open in CodeSandbox](https://img.shields.io/badge/Open%20in-CodeSandbox-black?style=for-the-badge&logo=codesandbox)](https://codesandbox.io/p/sandbox/github/sunilkumarpeela/davies-burgers-box-model)  


---

## 🎯 Skills Practiced  
- CSS **Box Model** (content → padding → border → margin)  
- Styling navigation menus & buttons  
- Working with images and background positioning  
- Scrollable content containers  
- Hover effects for interactive elements  

---

## 📄 index.html  
```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8" />
  <title>Davie JR's Menu</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <link href="https://fonts.googleapis.com/css?family=Roboto:100,500,700|Oswald:300,400,700" rel="stylesheet">
  <link rel="stylesheet" type="text/css" href="reset.css">
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
  <nav>
    <img src="https://content.codecademy.com/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers logo" />
    <span><a href="#">MENU</a></span>
    <span><a href="#">NUTRITION</a></span>
    <span><a href="#">ORDER</a></span>
    <span><a href="#">LOCATIONS</a></span>
  </nav>
  <div class="content">
    <div class="header" role="img" aria-label="BBQ Bacon Burger hero image">
      <h1>BBQ BACON BURGER</h1>
    </div>
    <div class="body">
      <p>
        Our BBQ Bacon Burger features our special house ground blend of wagyu and sirloin...
      </p>
      <a href="#" class="button">ORDER NOW</a>
      <ul class="nutrition">
        <li><span class="category">CALORIES</span><span class="value">678</span></li>
        <li><span class="category">FAT</span><span class="value">32</span></li>
        <li><span class="category">PROTEIN</span><span class="value">8</span></li>
        <li><span class="category">CARBOHYDRATES</span><span class="value">34</span></li>
        <li><span class="category">SODIUM</span><span class="value">112</span></li>
      </ul>
    </div>
  </div>
</body>
</html>
```
---
```🎨Style.css
/* Universal Styles */
body {
  background-image: url("https://content.codecademy.com/courses/web-101/unit-6/htmlcss1-img_foodlogo.png");
  text-align: center;
  font-family: 'Roboto', sans-serif;
  font-size: 18px;
}
a { text-decoration: none; }

/* Navigation */
nav { text-align: center; padding: 20px 0; }
nav img { display: block; width:180px; margin: 0 auto 10px; }
nav span { display: inline-block; margin: 10px 8px; font-size: 16px; font-weight: 100; letter-spacing: 2px; }
nav a { color: #666; }

/* Content */
.content { width: 100%; max-width: 900px; height:500px; margin: 10px auto; overflow: scroll; border:1px solid #e6e6e6; border-radius: 8px; }
.header { background:url("https://content.codecademy.com/courses/web-101/unit-6/htmlcss1-img_burgerphoto.jpeg") center/cover; height:320px; display:grid; place-items:center; }
.header h1 { background:#05A8AA; color:#fff; padding:20px; margin:0 auto; width:68%; border-radius:6px; font-family:'Oswald',sans-serif; font-weight:300; }

/* Body */
.body { width:90%; margin:0 auto; padding:20px; }
.body p { color:#333; font-weight:100; line-height:34px; width:90%; margin:18px auto 0; }

/* Button */
.button { display:block; width:200px; padding:20px; margin:40px auto; border:1px solid blue; border-radius:4px; color:#05A8AA; font-weight:700; }
.button:hover { background:#05A8AA; color:#fff; }

/* Nutrition */
ul.nutrition { padding:20px; }
ul.nutrition li { display:inline-block; background:#05A8AA; list-style:none; width:200px; padding:10px 20px; margin:3px 6px; border-radius:6px; }
.nutrition .category { color:#fff; letter-spacing:2px; display:block; }
.nutrition .value { color:#fff; font-size:26px; font-weight:700; letter-spacing:2px; }
```
---
```♻️ reset.css
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
```
