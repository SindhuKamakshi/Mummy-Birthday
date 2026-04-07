# 🎂 Birthday Surprise Website

A classy, emotional, interactive birthday website with glassmorphism design.

## 📁 Folder Structure

```
birthday-website/
├── index.html              ← Main website file (open this in browser)
├── README.md               ← This file
├── music/
│   └── (add your .mp3 here)
└── photos/
    ├── brothers/           ← Add brothers photos here
    ├── daughter1/          ← Add first daughter photos here
    ├── daughter2/          ← Add second daughter photos here
    ├── son/                ← Add son photos here
    └── final/              ← Add the final special photo here
```

## 🚀 How to Run in VS Code

1. Install the **Live Server** extension in VS Code
   - Open Extensions (Ctrl+Shift+X)
   - Search "Live Server" by Ritwick Dey
   - Click Install

2. Open the `birthday-website` folder in VS Code

3. Right-click `index.html` → **"Open with Live Server"**

4. The website opens in your browser at `http://127.0.0.1:5500`

---

## ✏️ Customization Guide

### 📸 Adding Photos

In `index.html`, find sections like:

```html
<div class="photo-item">
  <div class="placeholder">📸<span>Photo 1</span></div>
  <!-- <img src="photos/brothers/photo1.jpg" alt="Brothers photo 1"> -->
</div>
```

1. Add your image file to the correct folder (e.g. `photos/brothers/photo1.jpg`)
2. **Delete** the `<div class="placeholder">...</div>` line
3. **Uncomment** the `<img>` line (remove `<!--` and `-->`)

### ✍️ Editing Messages

Search for comments like:
```
✍️  BROTHERS MESSAGE — EDIT THIS TEXT
```
Edit the text inside the `<div class="message-block">` below it.

### 🎵 Adding Background Music

1. Place your `.mp3` file in the `music/` folder (e.g. `music/birthday-song.mp3`)
2. In `index.html`, find the `<audio id="bg-music">` tag
3. Uncomment the source line and update the path:
```html
<source src="music/birthday-song.mp3" type="audio/mpeg">
```

### 🎨 Changing Colors

At the top of `index.html`, find `:root { ... }` and edit the CSS variables:
```css
--pink:       #f9c4d2;   /* Main pink */
--lavender:   #d8b4fe;   /* Lavender accent */
--pink-deep:  #f48fb1;   /* Deep pink (buttons, accents) */
--lav-deep:   #a78bfa;   /* Deep lavender */
```

### 💬 Editing the Final Typed Message

Search for `const finalMessage =` in the `<script>` section and edit the text.

---

## 📱 Mobile Friendly
The website is fully responsive and works on phones and tablets.

