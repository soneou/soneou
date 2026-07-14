# Setup Guide: Professional GitHub Profile for `soneou`

This package is designed for the GitHub account **`soneou`**.

GitHub displays a profile README when:

1. The repository name exactly matches your GitHub username.
2. The repository is public.
3. A file named `README.md` exists in the repository root.

Official GitHub documentation:
https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme

---

## Option A: Set up from the GitHub website

### Step 1: Create the special profile repository

1. Log in to GitHub.
2. Click **New repository**.
3. Repository name: `soneou`
4. Visibility: **Public**.
5. You may leave **Add a README file** unchecked because this package already includes one.
6. Click **Create repository**.

### Step 2: Upload this package

After extracting the ZIP file, upload these items to the root of the `soneou` repository:

```text
soneou/
├── README.md
├── SETUP_GUIDE.md
└── assets/
    ├── hero.svg
    ├── divider.svg
    └── footer.svg
```

Important: Do not upload the outer folder itself as an extra nested folder. `README.md` must be directly at the root of the repository.

### Step 3: Commit the files

Use a commit message such as:

```text
Create professional GitHub profile README
```

Then open:

```text
https://github.com/soneou
```

The new profile README should appear near the top of your profile.

---

## Option B: Set up with Git commands

### 1. Create a public repository named `soneou` on GitHub

Then run:

```bash
git clone https://github.com/soneou/soneou.git
cd soneou
```

### 2. Copy the files from this package into the cloned repository

Your repository should look like this:

```text
soneou/
├── README.md
├── SETUP_GUIDE.md
└── assets/
    ├── hero.svg
    ├── divider.svg
    └── footer.svg
```

### 3. Commit and push

```bash
git add .
git commit -m "Create professional GitHub profile README"
git branch -M main
git push -u origin main
```

---

## How to customize the text

Open `README.md` in VS Code, Notepad++, or GitHub's online editor.

The easiest items to edit are:

- The **About Me** paragraph.
- The **Current focus** text block.
- The **Tech Stack** badges.
- The **Featured Projects** section.
- The **Connect With Me** links.

After editing locally:

```bash
git add README.md
git commit -m "Update profile information"
git push
```

---

## How to customize the banner background

The top banner is stored here:

```text
assets/hero.svg
```

You can edit it in a text editor because SVG is XML-based code.

Main color values used in the current design:

```text
Dark background: #080B16 / #11152B / #0A1020
Purple accent:  #8B5CF6
Cyan accent:    #22D3EE
Gold stars:     #FBBF24
Light text:     #F8FAFC
```

To change the main name, find:

```xml
NEOU SO
```

To change the subtitle, find:

```xml
SOFTWARE DEVELOPER · AI · AUTOMATION
```

To change the banner tagline, find:

```xml
Building useful software with clean code, practical AI,
and curiosity that refuses to sit quietly.
```

---

## Notes about the external statistics cards

The README uses these external image services:

- `github-readme-stats.vercel.app`
- `github-readme-activity-graph.vercel.app`
- `img.shields.io`

They create live cards and badges based on your GitHub account. If one of those services is temporarily unavailable or rate-limited, the rest of your profile will still work.

To remove live statistics entirely, delete the section under:

```markdown
## 📊 GitHub Activity
```

---

## Recommended profile bio

You can replace your current short bio with something more professional:

```text
Software Developer | AI & Computer Vision | Python, PHP & Automation | Building practical tools and learning in public.
```

GitHub profile settings:

```text
Profile photo → Settings → Public profile → Bio
```

---

## Recommended pinned repositories

Pin these six projects so visitors immediately see your strongest work:

1. `Autonomous-Lane-Detection-U-Net`
2. `car_person_cat_object_detection`
3. `spam_email_detection`
4. `POS-System-with-PHP`
5. `telegram_download_restricted_video`
6. `yt_download_video`

On your GitHub profile, use **Customize your pins** to choose the repositories.

---

## Troubleshooting

### The README does not appear on my profile

Check all three conditions:

```text
Repository name = soneou
Repository visibility = Public
README.md = located at repository root
```

### The banner is missing

Confirm these files exist exactly:

```text
assets/hero.svg
assets/divider.svg
assets/footer.svg
```

File names are case-sensitive on GitHub.

### Git asks for a password

GitHub no longer accepts account passwords for HTTPS Git operations. Use GitHub authentication through Git Credential Manager, GitHub CLI, SSH, or a personal access token.

---

## Final repository structure

```text
soneou/
├── README.md
├── SETUP_GUIDE.md
└── assets/
    ├── hero.svg
    ├── divider.svg
    └── footer.svg
```

Once pushed to the public repository `soneou`, GitHub will render `README.md` directly on the profile page.
