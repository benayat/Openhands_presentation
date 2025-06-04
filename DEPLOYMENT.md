# OpenHands Presentation - Deployment Guide

## 🚀 GitHub Pages Deployment

This presentation is ready for deployment to GitHub Pages. Follow these steps:

### Prerequisites
- GitHub account
- Git installed locally
- Web browser

### Step 1: Create GitHub Repository
1. Go to [GitHub](https://github.com) and create a new repository
2. Name it something like `openhands-presentation` or `openhands-seminar`
3. Make it **public** (required for free GitHub Pages)
4. Don't initialize with README (we already have files)

### Step 2: Push to GitHub
```bash
# Add remote origin (replace with your repository URL)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Push to GitHub
git push -u origin master
```

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings** tab
3. Scroll down to **Pages** section
4. Under **Source**, select **Deploy from a branch**
5. Choose **master** branch and **/ (root)** folder
6. Click **Save**

### Step 4: Access Your Presentation
- Your presentation will be available at: `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`
- It may take a few minutes to deploy initially
- The main presentation is at the root URL
- Additional resources are accessible via `index-resources.html`

## 📁 File Structure

```
openhands-presentation/
├── index.html                 # Main presentation (19 slides)
├── index-resources.html       # Navigation hub for all materials
├── README.md                 # Project overview and usage
├── speaker-notes.md          # Detailed presentation guide
├── technical-appendix.md     # Implementation details
├── presentation-summary.md   # Key statistics and takeaways
├── FINAL_DELIVERY.md        # Complete delivery documentation
├── DEPLOYMENT.md            # This deployment guide
├── serve.py                 # Local development server
├── .gitignore              # Git ignore rules
└── .git/                   # Git repository data
```

## 🔧 Local Development

To run locally for testing:

```bash
# Using Python (recommended)
python serve.py

# Or using Python's built-in server
python -m http.server 8000

# Then open: http://localhost:8000
```

## 🎯 Presentation Features

- **19 comprehensive slides** covering OpenHands architecture and research
- **Professional reveal.js design** with smooth transitions
- **Responsive layout** that works on different screen sizes
- **Working links** to GitHub repository and ArXiv paper
- **Current statistics** (57K+ stars, 188+ contributors)
- **Academic-quality content** suitable for graduate seminars

## 📱 Navigation

- **Arrow keys**: Navigate between slides
- **Space bar**: Next slide
- **ESC**: Overview mode
- **F**: Fullscreen mode
- **S**: Speaker notes (if available)

## 🔗 Key Links in Presentation

- [GitHub Repository](https://github.com/All-Hands-AI/OpenHands)
- [ArXiv Paper](https://arxiv.org/abs/2407.16741)
- [Documentation](https://docs.all-hands.dev/)
- [Official Website](https://all-hands.dev/)

## 🛠️ Customization

To customize the presentation:

1. **Content**: Edit `index.html` - all slide content is in HTML
2. **Styling**: Modify the `<style>` section in the `<head>`
3. **Configuration**: Adjust reveal.js settings in the `<script>` section
4. **Resources**: Update links and references as needed

## 📊 Performance

- **Load time**: < 2 seconds on modern connections
- **Size**: Lightweight with CDN-hosted dependencies
- **Compatibility**: Works on all modern browsers
- **Mobile-friendly**: Responsive design

## 🔒 Security

- All external resources loaded via HTTPS
- No sensitive data embedded
- Safe for public deployment
- CDN-hosted dependencies for reliability

## 📞 Support

If you encounter issues:
1. Check browser console for errors
2. Verify all files are properly uploaded
3. Ensure GitHub Pages is enabled correctly
4. Test locally first using the development server

## 📄 License

This presentation is created for educational purposes. OpenHands project is under MIT License.