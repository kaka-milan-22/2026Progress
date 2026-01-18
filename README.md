# Year Progress Tracker

A simple, beautiful year progress tracker that shows how much of the current year has passed.

## Features

- **Real-time Progress**: Updates every second with accurate calculations
- **Beautiful UI**: Gradient background with glass-morphism design
- **Responsive**: Works perfectly on desktop and mobile devices
- **Statistics**: Shows days elapsed, days remaining, and current date
- **Share Button**: Share your progress on social media or copy to clipboard
- **Leap Year Support**: Automatically accounts for leap years

## Live Preview

Open `index.html` in your browser to see it in action.

## Deploy to GitHub Pages

### Option 1: Direct Upload (Simplest)

1. Create a new repository on GitHub (name it something like `year-progress`)
2. Go to your repository on GitHub
3. Click "Add file" → "Upload files"
4. Drag and drop `index.html`
5. Click "Commit changes"
6. Go to repository Settings → Pages
7. Under "Build and deployment", select `main` (or `master`) branch as the source
8. Click Save
9. Wait 1-2 minutes for deployment
10. Your site will be available at: `https://your-username.github.io/year-progress/`

### Option 2: Using Git Command Line (Recommended for developers)

```bash
# Initialize git repository (if not already done)
git init

# Add your file
git add index.html

# Commit changes
git commit -m "Initial commit: Year progress tracker"

# Rename default branch to main (if needed)
git branch -M main

# Add remote repository (replace with your repo URL)
git remote add origin https://github.com/YOUR_USERNAME/year-progress.git

# Push to GitHub
git push -u origin main

# Enable GitHub Pages
# Go to repository Settings → Pages → Source: main branch → Save
```

### Option 3: Using GitHub CLI (if installed)

```bash
# Create repository and push in one command
gh repo create year-progress --public --source=. --remote=origin
git push -u origin main

# Enable GitHub Pages via web interface
# Go to repository Settings → Pages → Source: main branch → Save
```

## Customization

You can easily customize the appearance by editing the CSS in `index.html`:

- **Background**: Change the `background` gradient in the `body` style
- **Colors**: Modify the `progress-fill` gradient colors
- **Fonts**: Change the font family in the `body` style
- **Sizes**: Adjust the font sizes and container dimensions

## How It Works

The JavaScript calculates the year progress by:

1. Getting the current date
2. Calculating the day number (1-365 or 1-366 for leap years)
3. Computing the percentage: `(dayOfYear / daysInYear) * 100`
4. Updating the UI with the calculated values
5. Repeating every second for real-time updates

## License

MIT License - Feel free to use and modify as you like.
# 2026Progress
