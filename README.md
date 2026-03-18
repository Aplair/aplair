# Aplair Project

Cinematic real estate video editing and digital media services.

## Project Structure

- `index.html`: The main landing page including the booking modal and contact form.
- `refund-policy.html`: Detailed refund policy for services.
- `terms-of-service.html`: Terms and conditions.
- `assets/`:
    - `css/`: Styling files (`style.css` and its minified version).
    - `js/`: Application logic (`script.js` and its minified version).
    - `images/`: Logo and other graphical assets.
- `sitemap.xml`: SEO sitemap for the application.
- `robots.txt`: Search engine crawling instructions.

## Development

- **Scripts**: All form submissions are handled via `script.js` which connects to the Google Apps Script backend.
- **Styles**: Custom variables and organization are maintained in `style.css`.
- **Minification**: For production, ensure both `.min.js` and `.min.css` are updated.

## Deployment

The project is designed to be hosted on static platforms like GitHub Pages. Ensure URLs in `sitemap.xml` are correct after any domain changes.
