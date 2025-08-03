# Static Website with GitHub Pages CI/CD

A modern, responsive static website with automated deployment using GitHub Actions and GitHub Pages.

## 🚀 Project Overview

This project demonstrates a complete CI/CD pipeline for a static website. The website features:

- **Modern, responsive design** that works on all devices
- **Automated deployment** to GitHub Pages on every push to main branch
- **Clean, semantic HTML** with modern CSS styling
- **Fast loading** and optimized performance

## 📁 Project Structure

```
.
├── index.html              # Main HTML file
├── style.css               # CSS styles
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Actions workflow
└── README.md               # This file
```

## 🔄 CI/CD Workflow

The project uses GitHub Actions for continuous deployment. Here's how it works:

### Workflow File: `.github/workflows/deploy.yml`

This workflow automatically deploys your website to GitHub Pages whenever you push to the main branch. It uses the following actions:

- **`actions/checkout@v4`**: Checks out your repository code
- **`actions/configure-pages@v4`**: Sets up GitHub Pages configuration
- **`actions/upload-pages-artifact@v3`**: Uploads your website files as an artifact
- **`actions/deploy-pages@v4`**: Deploys the artifact to GitHub Pages

### Key Features:

- **Automatic deployment** on every push to main branch
- **Manual trigger** support via `workflow_dispatch`
- **Proper permissions** for GitHub Pages deployment
- **Concurrency control** to prevent deployment conflicts
- **Environment protection** with deployment URL output

## 🛠️ How to Update and Redeploy

### Making Changes Locally

1. **Clone the repository** (after pushing to GitHub):
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. **Make your changes** to `index.html` and/or `style.css`

3. **Test locally** by opening `index.html` in your browser

4. **Commit and push** your changes:
   ```bash
   git add .
   git commit -m "Update website content"
   git push origin main
   ```

### Automatic Deployment

Once you push to the main branch, the GitHub Actions workflow will:

1. ✅ Check out your code
2. ✅ Configure GitHub Pages
3. ✅ Upload your website files
4. ✅ Deploy to GitHub Pages
5. ✅ Provide you with the live URL

The deployment typically takes 1-2 minutes, and you'll see the status in the "Actions" tab of your GitHub repository.

## 📋 Prerequisites for Contributors

### Required Tools

- **Git** (latest version)
- **GitHub account** with repository access
- **Text editor** (VS Code, Sublime Text, etc.)
- **Web browser** for testing

### GitHub Repository Setup

1. **Create a new repository** on GitHub
2. **Enable GitHub Pages** in repository settings:
   - Go to Settings → Pages
   - Source: "GitHub Actions"
   - This enables the deployment workflow

### Local Development

1. **Install Git** if not already installed
2. **Configure Git** with your credentials:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
   ```

## 🚀 Getting Started

### Step 1: Initialize Git Repository

```bash
# Initialize git repository
git init

# Add all files to staging
git add .

# Make initial commit
git commit -m "Initial commit: Static website with CI/CD"
```

### Step 2: Connect to GitHub

```bash
# Add your GitHub repository as remote
git remote add origin https://github.com/yourusername/your-repo-name.git

# Push to GitHub
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Navigate to **Settings** → **Pages**
3. Under "Source", select **"GitHub Actions"**
4. The workflow will automatically deploy your site

### Step 4: Access Your Live Site

After the first successful deployment, your site will be available at:
```
https://yourusername.github.io/your-repo-name
```

## 📝 Customization

### Styling Changes

- Edit `style.css` to modify colors, fonts, layouts
- The CSS includes responsive design for mobile devices
- Use CSS Grid and Flexbox for modern layouts

### Content Changes

- Edit `index.html` to update text, images, and structure
- Add new sections by following the existing HTML structure
- Update navigation links as needed

### Adding New Pages

1. Create new HTML files (e.g., `about.html`, `contact.html`)
2. Update navigation links in `index.html`
3. Push changes to trigger automatic deployment

## 🔧 Troubleshooting

### Common Issues

1. **Workflow not triggering**: Ensure you're pushing to the `main` branch
2. **Deployment failing**: Check the Actions tab for error details
3. **Site not updating**: Wait 1-2 minutes for deployment to complete
4. **Permission errors**: Ensure GitHub Pages is enabled in repository settings

### Debugging

- Check the **Actions** tab in your GitHub repository for workflow logs
- Verify file paths and names are correct
- Ensure all files are committed and pushed

## 📚 Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Actions Documentation](https://docs.github.com/en/actions)
- [HTML5 Reference](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test locally
5. Push to your fork
6. Create a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Happy coding! 🎉** 