# 🚀 How to Upload Your Site to GitHub

This guide will walk you through uploading your Guitar Tuner Headquarters website to GitHub, step by step.

## Prerequisites

1. A GitHub account (create one at [github.com](https://github.com) if you don't have one)
2. All your project files (index.html, README.md, LICENSE, etc.)

## Method 1: Upload via GitHub Website (Easiest for Beginners)

### Step 1: Create a New Repository

1. Go to [GitHub.com](https://github.com) and log in
2. Click the **"+"** icon in the top-right corner
3. Select **"New repository"**
4. Name your repository: `guitar-tuner-hq` (or any name you prefer)
5. Add a description: "A comprehensive directory for guitar tuners and learning resources"
6. Choose **Public** (so others can see it)
7. **DO NOT** check "Add a README file" (we already have one)
8. Click **"Create repository"**

### Step 2: Upload Your Files

1. On your new repository page, click **"uploading an existing file"**
2. Drag and drop all your files:
   - index.html
   - README.md
   - LICENSE
   - .gitignore
   - CONTRIBUTING.md
3. Add a commit message: "Initial commit - Guitar Tuner HQ website"
4. Click **"Commit changes"**

### Step 3: Enable GitHub Pages (Make Your Site Live!)

1. In your repository, click **"Settings"**
2. Scroll down and click **"Pages"** in the left sidebar
3. Under "Source", select **"main"** branch
4. Click **"Save"**
5. Wait a minute, then refresh the page
6. You'll see: "Your site is live at https://yourusername.github.io/guitar-tuner-hq/"

🎉 **Congratulations!** Your site is now live on the internet!

## Method 2: Using Git Command Line (For Learning Git)

### Step 1: Install Git

- **Windows**: Download from [git-scm.com](https://git-scm.com)
- **Mac**: Open Terminal and type `git --version` (it will prompt to install if needed)
- **Linux**: Use your package manager (e.g., `sudo apt install git`)

### Step 2: Configure Git (First Time Only)

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Step 3: Create Repository on GitHub

1. Follow "Step 1" from Method 1 above to create a new repository
2. **DO NOT** upload any files yet
3. Copy the repository URL (looks like: `https://github.com/yourusername/guitar-tuner-hq.git`)

### Step 4: Upload Your Files Using Git

Open your terminal/command prompt and navigate to your project folder:

```bash
# Navigate to your project folder
cd /path/to/your/guitar-tuner-hq

# Initialize Git
git init

# Add all files
git add .

# Commit your files
git commit -m "Initial commit - Guitar Tuner HQ website"

# Connect to GitHub (replace with your repository URL)
git remote add origin https://github.com/yourusername/guitar-tuner-hq.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 5: Enable GitHub Pages

Follow "Step 3" from Method 1 above.

## Making Updates Later

### Via GitHub Website:

1. Go to your repository
2. Click on the file you want to edit
3. Click the pencil icon (Edit)
4. Make your changes
5. Click "Commit changes"

### Via Git Command Line:

```bash
# Make your changes to files
# Then:

git add .
git commit -m "Description of what you changed"
git push
```

## Common Issues & Solutions

**"Failed to push"**
- Make sure you're connected to the internet
- Check that your repository URL is correct
- Try pulling first: `git pull origin main`

**"Permission denied"**
- You may need to set up SSH keys or use a personal access token
- See [GitHub's authentication guide](https://docs.github.com/en/authentication)

**"Site not updating"**
- GitHub Pages can take 1-5 minutes to update
- Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Check the Pages settings to ensure it's enabled

## Next Steps

- Share your site URL with friends!
- Add your site to your portfolio
- Continue improving and updating your site
- Learn more Git commands to become a pro

## Helpful Resources

- [GitHub Docs](https://docs.github.com)
- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

---

**Need Help?** Open an issue on your repository or search for solutions on Stack Overflow!
