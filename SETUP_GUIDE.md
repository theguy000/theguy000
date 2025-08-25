# GitHub Profile Setup Guide

## 📋 Steps to Set Up Your GitHub Profile

### 1. Create the Repository
1. Go to GitHub and create a new repository named `theguy000` (same as your username)
2. Make sure it's **public**
3. Initialize with a README (you can replace it with the one from this folder)

### 2. Upload Files
1. Upload the `me.png` image to the repository
2. Upload the `readme.md` file (rename it to `README.md` in GitHub)
3. Upload the `.gitattributes` file
4. Create the `.github/workflows/` folder structure and upload `update-stats.yml`

### 3. Fix the C+ Language Issue
The C+ issue in GitHub stats is usually caused by:
- Incorrect language detection
- Files with ambiguous extensions
- Missing `.gitattributes` file

**Solutions implemented:**
- Added `&hide=c%2B%2B` parameter to the stats URL to hide C++ if it appears incorrectly
- Created `.gitattributes` file to properly define language detection
- Added `&langs_count=8` to show more relevant languages

### 4. Repository Structure
Your repository should look like this:
```
theguy000/
├── README.md (the main profile readme)
├── me.png (your profile image)
├── .gitattributes (language detection rules)
└── .github/
    └── workflows/
        └── update-stats.yml (optional: for auto-updating stats)
```

### 5. Verify Setup
1. Go to `https://github.com/theguy000`
2. Your profile README should automatically display
3. Check that the image loads correctly
4. Verify that the GitHub stats show the correct languages

### 6. Optional Enhancements
- Set up Wakatime integration for coding time tracking
- Add more repositories to improve language statistics
- Customize the theme colors in the stats URLs

### 🔧 Troubleshooting

**If the image doesn't load:**
- Make sure `me.png` is in the root of the repository
- Check that the repository is public
- Verify the image URL in the README

**If stats don't show correctly:**
- Wait a few minutes for GitHub to update
- Check that the username in URLs matches exactly: `theguy000`
- Ensure you have some repositories with code

**If C+ still appears:**
- The `.gitattributes` file should help
- You can also manually hide it using the `&hide=` parameter
- Make sure your repositories have proper file extensions

### 📝 Notes
- GitHub profile READMEs update automatically when you push changes
- Stats may take a few minutes to reflect changes
- The dark theme is applied to all stats for consistency
- Profile view counter will start tracking once the profile is live
