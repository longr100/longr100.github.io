# Step-by-Step Guide: Setting Up Your GitHub Pages Website

## Part 1: Creating the GitHub Repository

### Step 1: Create a New Repository on GitHub
1. Go to https://github.com and log in
2. Click the "+" icon in the top-right corner
3. Select "New repository"
4. Fill in the repository details:
   - **Repository name**: Choose a name (e.g., "my-website")
   - **Description**: (Optional) Add a brief description
   - **Public**: Select "Public" (required for free GitHub Pages)
   - **Initialize repository**: Leave all checkboxes UNCHECKED for now
5. Click "Create repository"

### Step 2: Note Your Repository Information
After creating the repo, you'll see a page with setup instructions. Keep this page open - you'll need the repository URL.

## Part 2: Setting Up Your Local Files

### Step 3: Create Your Project Folder
1. On your computer, create a new folder for your website (e.g., "my-website")
2. Download or copy these files into this folder:
   - index.html
   - style.css
   - script.js
   - README.md
   - .gitignore

### Step 4: Create Subdirectories
Inside your project folder, create two new folders:
1. Create a folder named `images`
2. Create a folder named `files`

Your folder structure should now look like:
```
my-website/
├── index.html
├── style.css
├── script.js
├── README.md
├── .gitignore
├── images/
└── files/
```

### Step 5: Add Your Content (Do This Now or Later)
- Place your photos in the `images/` folder
- Place your PDFs and downloadable files in the `files/` folder
- Edit `index.html` to update the text and file references

## Part 3: Pushing to GitHub

### Step 6: Initialize Git (Command Line Method)
1. Open Terminal (Mac) or Command Prompt/Git Bash (Windows)
2. Navigate to your project folder:
   ```bash
   cd path/to/my-website
   ```
3. Initialize git:
   ```bash
   git init
   ```
4. Add all files:
   ```bash
   git add .
   ```
5. Create your first commit:
   ```bash
   git commit -m "Initial commit"
   
 
 Step 6: Initialize Git (GitHub Desktop Method)

Download and Install GitHub Desktop

Go to https://desktop.github.com
Download and install for your operating system
Open GitHub Desktop and sign in with your GitHub account


Add Your Project Folder

Click File → Add Local Repository
Click Choose... and browse to your project folder (the one with index.html, style.css, etc.)
Click Add Repository


Create the Repository

GitHub Desktop will say "This directory does not appear to be a Git repository"
Click the Create a Repository button
In the dialog that appears:

Name: Should already be filled with your folder name
Description: (Optional) Add a brief description
Important: Uncheck "Initialize this repository with a README" (you already have one)
Leave Git Ignore and License as "None"


Click Create Repository


Make Your First Commit

You'll see all your files listed in the left panel under "Changes"
At the bottom left, there's a "Summary" field - type: Initial commit
Click the blue Commit to main button


Publish to GitHub

Click the Publish repository button in the top toolbar
In the dialog:

Important: Make sure "Keep this code private" is UNCHECKED (must be public for free GitHub Pages)
Organization: Leave as "None" (unless you want it under an organization)


Click Publish Repository
 
 
 ###Step 6 (alt): Initialize Git (GitHub Desktop Method)

Download and Install GitHub Desktop

Go to https://desktop.github.com
Download and install for your operating system
Open GitHub Desktop and sign in with your GitHub account


Add Your Project Folder

Click File → Add Local Repository
Click Choose... and browse to your project folder (the one with index.html, style.css, etc.)
Click Add Repository


Create the Repository

GitHub Desktop will say "This directory does not appear to be a Git repository"
Click the Create a Repository button
In the dialog that appears:

Name: Should already be filled with your folder name
Description: (Optional) Add a brief description
Important: Uncheck "Initialize this repository with a README" (you already have one)
Leave Git Ignore and License as "None"


Click Create Repository


Make Your First Commit

You'll see all your files listed in the left panel under "Changes"
At the bottom left, there's a "Summary" field - type: Initial commit
Click the blue Commit to main button


Publish to GitHub

Click the Publish repository button in the top toolbar
In the dialog:

Important: Make sure "Keep this code private" is UNCHECKED (must be public for free GitHub Pages)
Organization: Leave as "None" (unless you want it under an organization)


Click Publish Repository
   ```

### Step 7: Connect to GitHub Repository
1. Add your GitHub repository as the remote origin (replace with your actual URL):
   ```bash
   git remote add origin https://github.com/yourusername/my-website.git
   ```
2. Rename the branch to main (if needed):
   ```bash
   git branch -M main
   ```
3. Push your files to GitHub:
   ```bash
   git push -u origin main
   ```

## Part 4: Enable GitHub Pages

### Step 8: Configure GitHub Pages
1. Go to your repository on GitHub (https://github.com/yourusername/my-website)
2. Click on "Settings" (top menu bar)
3. In the left sidebar, click "Pages"
4. Under "Source":
   - Select branch: **main**
   - Select folder: **/ (root)**
5. Click "Save"

### Step 9: Wait for Deployment
- GitHub will take 1-5 minutes to build and deploy your site
- You'll see a message: "Your site is ready to be published at https://yourusername.github.io/my-website/"
- Refresh the page after a minute to see if it's live

### Step 10: Visit Your Website!
- Click the link or go to: `https://yourusername.github.io/my-website/`
- Your website should now be live!

## Alternative: GitHub Desktop (No Command Line)

If you prefer a graphical interface:

### Using GitHub Desktop:
1. Download and install GitHub Desktop from https://desktop.github.com
2. Open GitHub Desktop and sign in
3. Click "File" > "Add Local Repository"
4. Browse to your project folder
5. If prompted that it's not a Git repository, click "Create a repository"
6. Fill in the details and click "Create Repository"
7. Click "Publish repository" in the top bar
8. Make sure "Keep this code private" is UNCHECKED
9. Click "Publish Repository"
10. Follow Steps 8-10 above to enable GitHub Pages

## Updating Your Website

Whenever you make changes:

### Command Line:
```bash
git add .
git commit -m "Description of changes"
git push
```

### GitHub Desktop:
1. Open GitHub Desktop
2. You'll see changed files in the left panel
3. Add a commit message at the bottom
4. Click "Commit to main"
5. Click "Push origin" at the top

Changes will appear on your live site within 1-2 minutes.

## Troubleshooting

**Site not loading?**
- Wait 5 minutes after enabling Pages
- Check that your repository is Public
- Ensure `index.html` is in the root folder
- Check the Actions tab for build errors

**Images not showing?**
- Check file paths in your HTML
- Ensure images are in the `images/` folder
- File names are case-sensitive on GitHub Pages

**404 Error?**
- Make sure the URL is exactly: `https://yourusername.github.io/repository-name/`
- Check that GitHub Pages is enabled in Settings

## Need Help?

- GitHub Pages Documentation: https://docs.github.com/pages
- Git Documentation: https://git-scm.com/doc
