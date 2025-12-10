# Website Maintenance Manual - Tech Thrive Technology

This website is built using **Static HTML5 & CSS3**. This ensures maximum speed, security, and stability. There is no database or backend CMS to manage.

## 1. How to Update Content (Text)

To change text on any page, you simply need to edit the corresponding HTML file.

*   **Home Page:** Edit `index.html`
*   **About Page:** Edit `about.html`
*   **Services:** Edit `services.html`
*   **Contact/Enquiry:** Edit `contact.html` or `enquiry.html`

**Example:**
To change the "Hero Title" on the homepage:
1.  Open `index.html`.
2.  Search for the text "Empowering Businesses".
3.  Replace it with your new text.
4.  Save the file.

## 2. How to Update Images

Currently, the site uses high-quality placeholder images from Unsplash.

**To use your own images:**
1.  Create a folder named `images` in the project root.
2.  Save your image there (e.g., `team-photo.jpg`).
3.  In the HTML file, find the `<img>` tag.
4.  Change the `src` attribute:
    *   **Old:** `<img src="https://images.unsplash.com/..." alt="...">`
    *   **New:** `<img src="images/team-photo.jpg" alt="Our Team">`

## 3. How to Add a New Service

To add a 5th service to the Services page:

1.  Open `services.html`.
2.  Find the section `<div class="grid grid-2">`.
3.  Copy an entire `<div class="service-card">...</div>` block.
4.  Paste it immediately after the last service card.
5.  Update the `<h3>` title and `<p>` description inside the new block.

## 4. How to Change Colors (Branding)

The entire color scheme is managed in one place: `style.css`. You don't need to find-and-replace colors in every file.

1.  Open `style.css`.
2.  Look at the top under `:root`.
3.  Change the Hex codes:

```css
:root {
  /* Change this to your new primary color */
  --color-primary: #0B2545; 
  
  /* Change this to your new accent color (buttons/highlights) */
  --color-accent: #14B8A6; 
}
```

## 5. How to Publish Updates

Once you have made changes locally:

1.  **Save** all files.
2.  Open your terminal/command prompt.
3.  Run these commands to push to GitHub (which will auto-update your live site):

```bash
git add .
git commit -m "Updated homepage text"
git push origin main
```

## 6. Form Handling

The Enquiry form is currently a frontend interface. To receive emails, you have two simple options without needing a backend server:

**Option A: Formspree (Easiest)**
1.  Go to [formspree.io](https://formspree.io) and register (Free).
2.  Create a new form and get your unique URL.
3.  Update the `<form>` tag in `enquiry.html`:
    ```html
    <form action="https://formspree.io/f/YOUR_UNIQUE_ID" method="POST" ...>
    ```

**Option B: Netlify Forms (If hosting on Netlify)**
1.  Add the `netlify` attribute to the form tag:
    ```html
    <form name="enquiry" method="POST" data-netlify="true" ...>
    ```
2.  Netlify will automatically catch submissions and show them in your dashboard.

---
*Document prepared by Tech Thrive Development Team*
