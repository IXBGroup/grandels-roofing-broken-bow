# Grandel's Roofing & Construction Landing Page

Simple static landing page for Grandel's Roofing & Construction in Broken Bow, Nebraska. It uses only HTML, CSS, and JavaScript and can be opened directly in a browser.

## Files

- `index.html`
- `style.css`
- `script.js`
- `README.md`

## Replace the Google Form Embed URL

1. Open `index.html`.
2. Find this iframe:

```html
<iframe
  src="https://docs.google.com/forms/d/e/1FAIpQLSfT9B-w4i65J1kHWSHYkLlasQBCtjWafoTMf8UfIOrN-VcrTA/viewform?embedded=true"
  title="Schedule a Free Roof Inspection form"
  loading="lazy">Loading...</iframe>
```

3. Replace the existing `src` URL with the new Google Form embed URL.
4. In Google Forms, you can find this by choosing **Send**, selecting the embed icon, and copying the URL from the iframe code.

## Publish With GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html`, `style.css`, `script.js`, and `README.md` to the repository root.
3. In GitHub, open **Settings** for the repository.
4. Go to **Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select the `main` branch and `/root` folder, then save.
7. GitHub will provide a Pages URL after the site is published.

## Add a Custom Domain Later

1. In the repository, open **Settings** then **Pages**.
2. Enter the custom domain in the **Custom domain** field.
3. Save the domain.
4. Update DNS with your domain provider using GitHub Pages' current DNS instructions.
5. After DNS verifies, enable **Enforce HTTPS** if available.

For the latest DNS record values, use GitHub's official Pages documentation because DNS requirements can change.

## Replace Logo and Hero Image Placeholders

### Logo

1. Add your logo image file to the repository, for example `logo.png`.
2. In `index.html`, replace:

```html
<div class="logo-placeholder" aria-hidden="true">Logo</div>
```

with:

```html
<img class="logo-image" src="logo.png" alt="Grandel's Roofing & Construction logo">
```

3. Add this to `style.css`:

```css
.logo-image {
  width: 54px;
  height: 54px;
  object-fit: contain;
  border-radius: 8px;
}
```

### Hero Image

1. Add a roofing photo to the repository, for example `hero-roofing.jpg`.
2. In `index.html`, replace the `hero-image-placeholder` block with:

```html
<img class="hero-image" src="hero-roofing.jpg" alt="Roofing project by Grandel's Roofing & Construction">
```

3. Add this to `style.css`:

```css
.hero-image {
  width: 100%;
  min-height: 390px;
  object-fit: cover;
  border-radius: 8px;
  box-shadow: var(--shadow);
}
```
