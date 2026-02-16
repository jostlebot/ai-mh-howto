# How to Deploy This Site to GitHub Pages

## Step 1: Create a GitHub Account (if you don't have one)
1. Go to [github.com](https://github.com)
2. Click "Sign up" and follow the steps
3. Verify your email

## Step 2: Install Git (if not already installed)
Open Terminal and run:
```
git --version
```

If you see a version number, you're good! If not, it will prompt you to install it.

## Step 3: Create a New Repository on GitHub
1. Go to [github.com/new](https://github.com/new)
2. Name it something like `ai-mh-guide` or `your-username.github.io` (for a personal site)
3. Keep it **Public** (required for free GitHub Pages)
4. **Don't** check any boxes for README, .gitignore, or license
5. Click "Create repository"

## Step 4: Push Your Site to GitHub
In Terminal, run these commands one at a time:

```bash
# Navigate to your project
cd ~/ai-mh-howto-site

# Initialize git
git init

# Add all files
git add .

# Create first commit
git commit -m "Initial commit: AI tools guide for MH leaders"

# Connect to your GitHub repository (replace with YOUR URL)
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 5: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings** (tab at the top)
3. Click **Pages** (in the left sidebar)
4. Under "Source", select **main** branch
5. Click **Save**
6. Wait 1-2 minutes

Your site will be live at: `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

## Making Updates
Whenever you edit your site, push the changes:

```bash
cd ~/ai-mh-howto-site
git add .
git commit -m "Description of what you changed"
git push
```

Changes go live within a few minutes.

## Custom Domain (Optional)
If you want to use your own domain (like guide.yoursite.com):
1. In GitHub Pages settings, enter your custom domain
2. Add a CNAME record with your domain registrar pointing to `YOUR-USERNAME.github.io`
3. Wait for DNS to propagate (can take up to 24 hours)

## Need Help?
- GitHub Pages docs: https://docs.github.com/en/pages
- If something goes wrong, check the "Actions" tab in your repo for error messages
