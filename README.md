# Making Journal: GitHub Pages Template

A minimal static website for your weekly making journal, using GitHub Pages.

## Prerequisites

Before you start, make sure you have the following installed:

- **GitHub Desktop:** Download from [desktop.github.com](https://desktop.github.com/). This handles all the Git operations for you — no terminal needed.
- **VS Code:** Download from [code.visualstudio.com](https://code.visualstudio.com/).
- **A GitHub account:** Sign up at [github.com](https://github.com/) if you don't have one.

## Quick Setup

1. **Create your own copy of this repository:**
   - Click the green **"Use this template"** button at the top of this repo, then choose **"Create a new repository"**.
   - Give your new repository a name (e.g. `making-journal`) and click **"Create repository"**.
2. **Clone your new repository with GitHub Desktop:**
   - In GitHub Desktop, select your new repository, then click **"Clone"**. 
   - Choose a folder on your computer to save the project.
3. **Enable GitHub Pages:**
   - Go to your repo on GitHub → **Settings** → **Pages**
   - Under "Source", select **Deploy from a branch**
   - Choose the **main** branch and **/ (root)** folder
   - Click **Save**
4. **Wait 1–2 minutes**, then visit `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

## How to Use

### Working on your journal
- In GitHub Desktop, click **"Open in Visual Studio Code"** to open your project.
- Journal entries are in `journal-pages/week-XX.md` — one file per week.
- Write using [Markdown](https://www.markdownguide.org/basic-syntax/).

### Publishing your changes
When you're ready to update your site, switch from VS Code to GitHub Desktop:
1. Your changed files will appear automatically in the left panel.
2. Type a short summary in the **"Summary"** box at the bottom left (e.g. "Week 03 documentation").
3. Click the blue **"Commit to main"** button.
4. Click **"Push origin"** at the top. Your site will update automatically within a couple of minutes.

### Adding images
1. Place your file in the matching `assets/week-XX/` folder.
2. Embed it in your week's page:
   ```
   ![Alt text](../assets/week-01/photo.jpg)
   *Your caption here*
   ```
   The text inside the square brackets is alt text (a description for accessibility), not a visible caption. To add a caption, place a line of italic text below the image.

### Adding video (hosted elsewhere)
Markdown doesn't embed video directly. Link to it instead:
```
[Watch the video](https://www.youtube.com/watch?v=XXXX)
```

Or, if you need an inline embed, use a small HTML snippet:
```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/XXXX"></iframe>
```

## File Structure

```
/
├── _config.yml          ← Site settings (title, theme)
├── index.md             ← Homepage with links to all weeks
├── journal-pages/
│   ├── week-01.md       ← One file per week
│   ├── ...
│   └── week-12.md
├── assets/
│   ├── week-01/         ← Images/media for each week
│   ├── ...
│   └── week-12/
└── README.md            ← This file (not shown on the site)
```

## Customisation

> **Note:** Customising the theme or site settings is entirely optional and goes beyond what is required for the course. Only explore this if you're comfortable with the basics first.

- **Site title and description:** Edit `_config.yml`.
- **Theme:** The default is `minimal`. You can change `remote_theme` in `_config.yml` to any [supported GitHub Pages theme](https://pages.github.com/themes/).
