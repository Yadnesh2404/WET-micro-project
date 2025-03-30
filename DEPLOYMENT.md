# Deployment Guide

Follow these steps to deploy your Agnel Polytechnic Vashi website to GitHub Pages:

## Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com/) and sign in to your account
2. Click on the "+" icon in the top right corner and select "New repository"
3. Name your repository (e.g., "agnel-polytechnic-website")
4. Set the repository to "Public"
5. Do not initialize with a README (we already have one)
6. Click "Create repository"

## Step 2: Push Your Code to GitHub

Run the following commands in your terminal:

```bash
# Navigate to your project directory
cd path/to/your/project

# Initialize Git repository
git init

# Add all files to staging
git add .

# Commit changes
git commit -m "Initial commit"

# Add the remote repository
git remote add origin https://github.com/your-username/your-repository-name.git

# Push to GitHub
git push -u origin main
```

If you're using the main branch instead of master, replace `master` with `main` in the command above.

## Step 3: Configure GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to the "GitHub Pages" section (or navigate to "Pages" in the left sidebar)
4. Under "Source", select "GitHub Actions"
5. Wait a few minutes for the deployment to complete

## Step 4: Access Your Website

After the deployment is complete, your website will be available at:
```
https://your-username.github.io/your-repository-name/
```

## Troubleshooting

If your website doesn't display properly:

1. Check that all file paths are correct (they are case-sensitive)
2. Make sure all image files were properly pushed to GitHub
3. Verify that the GitHub Actions workflow completed successfully

## Updating Your Website

To update your website, simply make changes to your local files, commit them, and push to GitHub:

```bash
git add .
git commit -m "Updated website content"
git push
```

The GitHub Actions workflow will automatically deploy your updates to GitHub Pages. 