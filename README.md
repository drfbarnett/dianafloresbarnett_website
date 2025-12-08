# Quarto Website Template

A template repository for creating a personal or academic website using [Quarto](https://quarto.org/).

## 📁 Repository Structure

```
quarto-website-template/
├── _quarto.yml          # Main configuration file - CUSTOMIZE THIS FIRST
├── theme-custom.scss    # Custom colors and theme settings
├── styles.css           # Additional CSS styles
├── index.qmd            # Homepage
├── about.qmd            # About/bio page
├── research.qmd         # Research projects page
├── publications.qmd     # Publications list
├── people.qmd           # Team members page
├── posts.qmd            # News/blog listing page
├── teaching.qmd         # Courses and teaching
├── posts/               # Individual news posts
│   └── YYYY-MM-DD-title.qmd
├── people/              # Team member photos
├── images/              # Site images and graphics
├── publications/        # Publication PDFs (optional)
├── docs/                # Rendered HTML output (for GitHub Pages)
│   └── .nojekyll        # Disables Jekyll processing on GitHub Pages
├── .nojekyll            # Disables Jekyll processing
├── .gitignore           # Git ignore rules
└── README.md            # This file
```

## 🚀 Getting Started

### Prerequisites

1. **Install Quarto**: Download from [quarto.org/docs/get-started](https://quarto.org/docs/get-started/)
2. **Install Git**: [git-scm.com](https://git-scm.com/)
3. **Create a GitHub account**: [github.com](https://github.com/)

### Step 1: Create Your Repository

**Option A: Use this template (if it's a GitHub template repo)**
1. Click "Use this template" button
2. Name your repository `YOUR_USERNAME.github.io` for a personal site
3. Clone to your computer: `git clone https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io`

**Option B: Manual setup**
1. Download/clone this template
2. Create a new repository on GitHub
3. Initialize git and push

### Step 2: Customize the Configuration

Open `_quarto.yml` and update:

```yaml
website:
  title: "Your Name"  # Change this
  navbar:
    right:
      - icon: github
        href: https://github.com/YOUR_USERNAME  # Change this
      - icon: envelope
        href: mailto:YOUR_EMAIL@example.com     # Change this
```

### Step 3: Add Your Content

1. **Edit each `.qmd` file** - Replace placeholder text with your information
2. **Add images** - Put your photos in `images/` and `people/` folders
3. **Create posts** - Add news items in `posts/` folder

### Step 4: Preview Locally

```bash
# Navigate to your project folder
cd your-website-folder

# Start the preview server
quarto preview
```

This opens your browser with a live preview. Changes update automatically.

### Step 5: Render the Site

```bash
quarto render
```

This creates the `docs/` folder with your rendered HTML files.

### Step 6: Deploy to GitHub Pages

1. **Commit and push your changes:**
   ```bash
   git add .
   git commit -m "Initial website setup"
   git push origin main
   ```

2. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Click **Settings** → **Pages**
   - Under "Source", select **Deploy from a branch**
   - Select **main** branch and **/docs** folder
   - Click **Save**

3. **Wait a few minutes**, then visit `https://YOUR_USERNAME.github.io`

## 📝 How to Edit Content

### Markdown Basics

Quarto uses Markdown for content. Here's a quick reference:

```markdown
# Heading 1
## Heading 2
### Heading 3

**Bold text**
*Italic text*
[Link text](https://url.com)

![Image description](images/photo.jpg)

- Bullet point
- Another point

1. Numbered item
2. Second item
```

### Adding a New Page

1. Create a new `.qmd` file in the root folder
2. Add a YAML header:
   ```yaml
   ---
   title: "Page Title"
   ---
   ```
3. Add the page to the navbar in `_quarto.yml`
4. Write your content

### Adding a News Post

1. Create a file in `posts/` named `YYYY-MM-DD-title.qmd`
2. Include this header:
   ```yaml
   ---
   title: "Post Title"
   date: "2024-03-15"
   categories: [News]
   ---
   ```
3. Write your content below the header

## 🎨 Customization

### Colors

Edit `theme-custom.scss` to change colors:

```scss
$primary:   #2c3e50;   // Main brand color
$secondary: #18bc9c;   // Accent color
```

### Fonts

Add custom fonts in `theme-custom.scss`:

```scss
$font-family-sans-serif: "Your Font", sans-serif;
```

### Adding Extensions

Quarto has many extensions. For example, to add Font Awesome icons:

```bash
quarto add quarto-ext/fontawesome
```

Then use icons like: `{{< fa envelope >}}`

## 🔧 Troubleshooting

### Site not updating on GitHub Pages?
- Check the **Actions** tab for build errors
- Make sure the `docs/` folder is committed
- Verify Pages settings point to `/docs` folder

### Preview not working?
- Make sure Quarto is installed: `quarto --version`
- Check for YAML syntax errors (proper indentation)

### Images not showing?
- Verify the file path is correct
- Check that the image file is committed to git
- Use relative paths: `images/photo.jpg` not `/images/photo.jpg`

## 📚 Resources

- [Quarto Documentation](https://quarto.org/docs/websites/)
- [Quarto Gallery](https://quarto.org/docs/gallery/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)

## 📄 License

This template is provided for educational use. Feel free to customize for your own website.

---

*Template created for Git and GitHub instruction. Happy coding!*
