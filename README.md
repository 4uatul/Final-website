# Atul Bhardwaj - Portfolio Website Instructions

## 🎉 Welcome to Your Portfolio!

This is a modern, fully responsive portfolio website designed to attract recruiters and showcase your skills, projects, and experience.

---

## 📸 ADDING YOUR PROFILE PICTURE

### Method 1: Using a Local Image File (Recommended)
1. **Prepare your photo:**
   - Use a professional headshot
   - Square format works best (500x500px or larger)
   - Save it as `profile.jpg` or `profile.png`

2. **Add the image:**
   - Save your photo in the **same folder** as `portfolio.html`
   - If you named it something else (e.g., `myPhoto.png`), update line 420 in the HTML:
   ```html
   <img src="myPhoto.png" alt="Atul Bhardwaj Profile Picture" class="profile-img">
   ```

### Method 2: Using a URL (LinkedIn, Google Drive, etc.)
1. **Get the image URL:**
   - LinkedIn: Right-click your profile picture → "Copy image address"
   - Google Drive: Upload image → Get shareable link → Make sure it's publicly accessible
   
2. **Update the HTML:**
   - Find line 420 in `portfolio.html`
   - Replace `src="profile.jpg"` with your URL:
   ```html
   <img src="https://your-image-url-here.com/image.jpg" alt="Atul Bhardwaj" class="profile-img">
   ```

---

## 🖼️ ADDING PROJECT IMAGES

Your website has 3 featured projects. Here's how to add screenshots for each:

### Step-by-Step:
1. **Take screenshots** of your projects (recommended size: 800x500px)

2. **Name them:**
   - `project1.jpg` - SmartStock project
   - `project2.jpg` - TF-IDF Search Engine
   - `project3.jpg` - Heart Disease Predictor

3. **Save them** in the same folder as `portfolio.html`

4. **Image locations in HTML:**
   - **SmartStock**: Line 632
   - **TF-IDF Search Engine**: Line 660
   - **Heart Disease Predictor**: Line 688

### Using Placeholder Images (Temporary):
If you don't have screenshots yet, you can use placeholder images:

Replace the `src` attribute with:
```html
<img src="https://via.placeholder.com/800x500/2563eb/ffffff?text=Project+Name" alt="Project">
```

---

## 🔗 ADDING YOUR GITHUB PROJECT LINKS

Currently, all project links point to your main GitHub profile (`https://github.com/4uatul`).

### To add specific repository links:

1. **Find the project links in HTML:**
   - SmartStock: Line 651
   - TF-IDF Search Engine: Line 679
   - Heart Disease Predictor: Line 707

2. **Update with your repo URLs:**
   ```html
   <a href="https://github.com/4uatul/your-repo-name" class="project-link" target="_blank">View on GitHub →</a>
   ```

### Example:
If your SmartStock repo is at `https://github.com/4uatul/smartstock-saas`, change:
```html
<a href="https://github.com/4uatul/smartstock-saas" class="project-link" target="_blank">View on GitHub →</a>
```

---

## 📝 EDITING CONTENT

### Adding More Projects:
1. Find the Projects section (starting at line 584)
2. Copy the entire `<div class="project-card">...</div>` block (lines 632-656)
3. Paste it inside `<div class="projects-grid">` section
4. Edit the content for your new project

### Changing Colors:
All colors are defined at the top of the CSS (lines 11-20). Edit these variables:
```css
--primary-color: #2563eb;      /* Main blue color */
--secondary-color: #0ea5e9;    /* Lighter blue */
--accent-color: #06b6d4;       /* Teal accent */
```

Try these color combinations:
- **Professional Blue** (current): `#2563eb`, `#0ea5e9`
- **Modern Green**: `#10b981`, `#34d399`
- **Bold Purple**: `#8b5cf6`, `#a78bfa`
- **Tech Orange**: `#f97316`, `#fb923c`

### Adding More Skills:
1. Find the Skills section (line 724)
2. Copy a `<div class="skill-category">...</div>` block
3. Paste and edit the content

### Updating Experience:
1. Find the Experience section (line 448)
2. Copy a `<div class="timeline-item">...</div>` block
3. Add your new experience following the same format

---

## 📧 CONTACT FORM

The contact form is configured to open the user's email client with:
- Your email: `atuloninternet@gmail.com`
- Pre-filled subject and message

### To change your email:
Find line 922 and update:
```javascript
const mailtoLink = `mailto:YOUR-NEW-EMAIL@example.com?subject=...`;
```

---

## 🚀 DEPLOYING YOUR WEBSITE

### Option 1: GitHub Pages (FREE & Easy)
1. Create a new repository on GitHub
2. Upload `portfolio.html` and all images
3. Rename `portfolio.html` to `index.html`
4. Go to Settings → Pages → Select main branch
5. Your site will be live at: `https://yourusername.github.io/repo-name`

### Option 2: Netlify (FREE & Easy)
1. Go to [netlify.com](https://www.netlify.com/)
2. Drag and drop your folder with `portfolio.html` and images
3. Site goes live instantly!

### Option 3: Your Own Domain
1. Purchase a domain (e.g., atulbhardwaj.com)
2. Use any hosting service (GitHub Pages, Netlify, Vercel)
3. Connect your custom domain

---

## ✅ CHECKLIST BEFORE PUBLISHING

- [ ] Added profile picture
- [ ] Added all project images
- [ ] Updated GitHub project links
- [ ] Verified all contact information
- [ ] Tested the website on mobile
- [ ] Checked all links work
- [ ] Updated any outdated information

---

## 🎨 FEATURES OF YOUR WEBSITE

✅ **Fully Responsive** - Works on desktop, tablet, and mobile  
✅ **Modern Animations** - Smooth scrolling and hover effects  
✅ **Professional Design** - Clean, recruiter-friendly layout  
✅ **Easy to Edit** - Well-commented code  
✅ **Fast Loading** - No external dependencies  
✅ **SEO Friendly** - Proper HTML structure  

---

## 🆘 NEED HELP?

### Common Issues:

**Q: My images aren't showing up**  
A: Make sure the image files are in the same folder as the HTML file and the names match exactly (including file extension)

**Q: How do I view the website?**  
A: Double-click `portfolio.html` to open it in your browser

**Q: The layout looks broken on mobile**  
A: The design is responsive - try resizing your browser window or check on an actual mobile device

**Q: Can I add more sections?**  
A: Yes! Copy any section's structure and modify the content. Keep the same CSS class names for consistent styling.

---

## 📊 FILE STRUCTURE

```
your-folder/
│
├── portfolio.html          (Main website file)
├── profile.jpg            (Your profile picture)
├── project1.jpg           (SmartStock image)
├── project2.jpg           (TF-IDF Search Engine image)
├── project3.jpg           (Heart Disease Predictor image)
└── Atul_Bhardwaj_Resume.pdf  (Your resume - optional)
```

---

## 🎯 PRO TIPS FOR RECRUITERS

1. **Use High-Quality Images** - First impressions matter!
2. **Keep Content Updated** - Add new projects and experiences regularly
3. **Test Everything** - Click all links before sharing
4. **Mobile-First** - Most recruiters view on phones first
5. **Add Your Resume** - Include a downloadable PDF version
6. **Show, Don't Tell** - Use metrics and results in your project descriptions

---

## 🌟 NEXT STEPS

1. **Add your images** (profile + projects)
2. **Update GitHub links** to your actual repositories
3. **Test the website** in different browsers
4. **Deploy online** using GitHub Pages or Netlify
5. **Share the link** on LinkedIn and your resume!

---

## 📞 QUESTIONS?

If you run into any issues or need modifications, feel free to reach out!

**Good luck with your job search! 🚀**

---

*Built with ❤️ for impact-driven data scientists*