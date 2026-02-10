# 🎨 Customization Guide - Journey Through Time

## 📸 Uploading Your Photos

### Step 1: Prepare Your Images
Name your photos exactly as follows:
- `03.jpg` - Your Birthday Party
- `04.jpg` - London Harry Potter Trip  
- `05.jpg` - Switzerland Trip
- `06.jpg` - Amsterdam Trip
- `07.jpg` - Manali Trip
- `08.jpg` - Banaras Trip
- `09.jpg` - Andaman Trip
- `10.jpg` - Pic with Vrinda ⭐

### Step 2: Upload to `/images/` folder
Replace the placeholder images (03.jpg through 10.jpg) with your actual photos.

**Note:** Keep 01.jpg (Marriage) and 02.jpg (Goa) as they are already uploaded.

---

## ✍️ Editing Memory Text

Open `index.html` and find the `memories` array (around line 465). Each memory looks like this:

```javascript
{
    id: 3,
    title: "Birthday Celebration",  // Change this
    image: "images/03.jpg",
    text: "Your personal story here...",  // Change this
    color: "#c8b6e2"
}
```

### Example Customization:
```javascript
{
    id: 3,
    title: "My 30th Birthday Bash",
    image: "images/03.jpg",
    text: "The surprise party you planned made me feel like the luckiest person alive. Every detail was perfect, just like us.",
    color: "#c8b6e2"
}
```

---

## 🎵 Adding Background Music

### Option 1: Use Your Own Music File
1. Find a romantic instrumental MP3 (royalty-free)
2. Name it `background.mp3`
3. Place it in the `/music/` folder
4. Done! It will auto-play on journey start

### Option 2: Remove Music Feature
If you don't want music, open `index.html` and remove/comment out:
- The audio element (line ~440)
- The music control button (lines ~30-40 in HTML)

---

## 🎨 Changing Colors

Find the `:root` section in `index.html` (around line 30):

```css
:root {
    --rose: #d9778b;      /* Romantic pink */
    --wine: #7a2f43;      /* Deep burgundy */
    --lavender: #c8b6e2;  /* Soft purple */
    --sky: #a8d8ea;       /* Light blue */
    --gold: #ffd700;      /* Special gold for Vrinda */
    --white: #ffffff;
}
```

Change any hex color code to customize the theme!

---

## 🌟 Customizing Vrinda's Special Moment

The last memory (Vrinda) has special treatment:
- Golden border and glow
- Confetti animation
- Enhanced visual effects

To customize:
1. Find memory id: 10 in the `memories` array
2. The `special: true` flag triggers the confetti
3. Confetti colors are at line ~250 in the `createConfetti` function

---

## 📱 Testing Locally

Simply open `index.html` in your browser:
- Chrome/Edge: Just double-click the file
- Safari: Right-click → Open With → Safari
- Firefox: Drag and drop into browser window

---

## 🚀 Deploying to GitHub Pages

### Step 1: Create GitHub Repository
1. Go to github.com and create a new repository
2. Name it something like `valentine-journey`
3. Keep it public

### Step 2: Upload Your Files
```bash
git init
git add .
git commit -m "Our beautiful journey"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/valentine-journey.git
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repo Settings
2. Scroll to "Pages" section
3. Source: Select "main" branch
4. Click Save
5. Your site will be live at: `https://YOUR-USERNAME.github.io/valentine-journey/`

---

## 🎁 Tips for Best Experience

### Photo Quality:
- Use high-resolution images (at least 1920x1080)
- Landscape orientation works best
- Bright, clear photos show best against the dark theme

### Text Length:
- Keep memory text between 100-200 characters
- Too long = hard to read
- Too short = feels empty

### Testing on Mobile:
- Open on your phone to test responsiveness
- Everything should scale perfectly
- Swipe to scroll through memories

---

## 🐛 Troubleshooting

### Images Not Loading?
- Check file names exactly match (case-sensitive)
- Images must be in `/images/` folder
- Supported formats: JPG, PNG

### Music Not Playing?
- Some browsers block autoplay
- User must click "Play Music" button manually
- This is normal browser behavior

### Confetti Not Showing?
- Scroll all the way to the bottom
- Wait 2 seconds for animation to start
- Check if memory #10 has `special: true`

---

## 💝 Final Touches

### Make it Personal:
1. Change the welcome title to something meaningful
2. Add your wedding date or anniversary
3. Include inside jokes in memory descriptions
4. Choose a song that's special to both of you

### Before Sharing:
- [ ] All 10 photos uploaded
- [ ] All memory texts personalized
- [ ] Background music added
- [ ] Tested on desktop and mobile
- [ ] Shared with your loved one! ❤️

---

**Made with ❤️ for your Valentine's Day 2025**
