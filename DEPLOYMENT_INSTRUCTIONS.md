# GitHub Pages Deployment Instructions

## Step 1: Create a GitHub Repository
1. Go to [GitHub](https://github.com) and sign in to your account (or create one if you don't have it)
2. Click on the "+" icon in the top right corner and select "New repository"
3. Name your repository: `username.github.io` (replace "username" with your actual GitHub username)
4. Make sure the repository is set to "Public"
5. Click "Create repository"

## Step 2: Upload Your Portfolio Files
### Option 1: Using GitHub Web Interface
1. In your new repository, click on "uploading an existing file"
2. Extract the portfolio.zip file you downloaded
3. Drag and drop all the files and folders from the extracted portfolio folder
4. Add a commit message like "Initial portfolio upload"
5. Click "Commit changes"

### Option 2: Using Git Command Line
1. Extract the portfolio.zip file you downloaded
2. Open a terminal/command prompt in the extracted portfolio folder
3. Run the following commands (replace "username" with your GitHub username):
```
git remote add origin https://github.com/username/username.github.io.git
git branch -M main
git push -u origin main
```

## Step 3: Configure GitHub Pages
1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to the "GitHub Pages" section (or click on "Pages" in the left sidebar)
4. Under "Source", select "GitHub Actions" 
5. The workflow will automatically run when you push to the main branch

## Step 4: View Your Deployed Portfolio
1. After the GitHub Actions workflow completes (usually takes 1-2 minutes)
2. Your portfolio will be available at: https://username.github.io (replace "username" with your GitHub username)

## Step 5: Updating Your Portfolio
1. To make changes, edit the files locally
2. Commit and push the changes to GitHub
3. The GitHub Actions workflow will automatically deploy the updates

## Troubleshooting
- If your site doesn't appear, check the Actions tab in your repository to see if the workflow completed successfully
- Make sure your repository is named exactly as username.github.io
- Ensure all files are in the root of the repository, not in a subfolder
