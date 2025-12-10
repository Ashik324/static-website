# Tech Thrive Technology Website

This is the official website for Tech Thrive Technology, built with HTML5 and CSS3.

**Live Repository:** [https://github.com/Ashik324/static-website](https://github.com/Ashik324/static-website)

## 🚀 How to Publish/Update this Code

Since you have an existing repository, follow these steps to upload the latest code:

### Step 1: Open Terminal
Open your terminal or command prompt in the folder where these files are located.

### Step 2: Run Git Commands
Copy and paste the following commands:

```bash
# 1. Initialize Git (if not already done)
git init

# 2. Add your repository URL
# If this is the first time connecting:
git remote add origin https://github.com/Ashik324/static-website.git

# OR, if you are updating an existing connection:
git remote set-url origin https://github.com/Ashik324/static-website.git

# 3. Add all the new files
git add .

# 4. Save the changes
git commit -m "Update website design to professional version"

# 5. Send to GitHub
git push -u origin main
```

## 🌐 Live Hosting (GitHub Pages)

Once the code is pushed:
1.  Go to [https://github.com/Ashik324/static-website/settings/pages](https://github.com/Ashik324/static-website/settings/pages)
2.  Under **Build and deployment**, select **Source** -> **Deploy from a branch**.
3.  Select **Branch** -> `main` -> `/ (root)`.
4.  Click **Save**.

Your site will be live shortly!

## 🛠 Local Development

To run this project locally:

1.  Install dependencies:
    ```bash
    yarn install
    ```
2.  Start the dev server:
    ```bash
    yarn run dev
    ```
