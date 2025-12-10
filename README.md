# Tech Thrive Technology Website

This is the official website for Tech Thrive Technology, built with HTML5 and CSS3.

## 🚀 How to Publish to GitHub & Host Live

### Option 1: The Easy Way (GitHub Desktop / Web Upload)

1.  **Create a Repository:**
    *   Go to [GitHub.com](https://github.com) and sign in.
    *   Click the **+** icon in the top right and select **New repository**.
    *   Name it `tech-thrive-website` (or similar).
    *   Make sure it is **Public**.
    *   Click **Create repository**.

2.  **Upload Files:**
    *   If you are using the web interface, click **uploading an existing file** on the setup page.
    *   Drag and drop all the files from this project folder (index.html, style.css, etc.) into the upload box.
    *   Commit the changes.

### Option 2: The Developer Way (Command Line)

If you have Git installed on your computer:

```bash
# 1. Initialize Git
git init

# 2. Add all files
git add .

# 3. Commit changes
git commit -m "Initial website launch"

# 4. Link to your GitHub repo (Replace URL with your actual repo URL)
git remote add origin https://github.com/YOUR_USERNAME/tech-thrive-website.git

# 5. Push to GitHub
git push -u origin main
```

## 🌐 How to Go Live (GitHub Pages)

Once your code is on GitHub, you can host it for free:

1.  Go to your repository on GitHub.
2.  Click on **Settings** (top tab).
3.  On the left sidebar, click on **Pages**.
4.  Under **Build and deployment** > **Source**, select **Deploy from a branch**.
5.  Under **Branch**, select `main` (or `master`) and folder `/ (root)`.
6.  Click **Save**.

Wait about 1-2 minutes, and GitHub will give you a live URL (e.g., `https://your-username.github.io/tech-thrive-website/`).

## 🛠 Project Setup (Local Development)

To run this project locally on your machine:

1.  Install dependencies:
    ```bash
    yarn install
    ```
2.  Start the dev server:
    ```bash
    yarn run dev
    ```
