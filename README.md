# Ronams and Associates website

A static, dependency-free multi-page website. No framework or package install is needed.

## Preview

Open `index.html` in a browser, or serve this folder with any static web server. For example, from this folder run `python -m http.server 8000` and visit `http://localhost:8000`.

## Business configuration before publishing

Edit `config.js` to update supplied phone numbers and confirmed company details. The email, office address and WhatsApp destination are intentionally blank/unpublished until verified. Once the WhatsApp-enabled number is confirmed, enter its international digits without `+` in `whatsappNumber` and add the approved WhatsApp actions.

The request and contact forms currently validate input but do not send or store it. Their success-area copy explains this and offers click-to-call links. To accept submissions online, configure a secure backend endpoint in `config.js` and wire the forms to it; do not put private credentials in browser code. Update the privacy notice to match the actual storage and processing behavior before enabling a backend.

Replace the `.invalid` sitemap host with the final public HTTPS domain and add canonical URLs and Open Graph image metadata after the deployment domain is confirmed. The photos and web fonts are loaded from Unsplash and Google Fonts, so an internet connection is required for those assets. Replace the demonstration brand mark if the original logo becomes available.

## Pages

- `index.html` — home
- `about.html` — company approach and values
- `services.html` — seven directly linked service details
- `contact.html` — phone and general enquiry
- `request.html` — guided service request
- `privacy.html` and `terms.html` — site notices

## Deployment

Upload the contents of this folder to a static web host. Use the host's HTTPS setting and point the domain at this folder. There is no build step.
