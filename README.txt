CAMPUSFIND FRONTEND (RECOVERED FROM THE LIVE PUBLIC WEBSITE)

The original Netlify source ZIP was not available. This is a recreated frontend based on the public page's visible content and layout. It keeps the same CampusFind name, sections, report form, filters, and overall warm/green visual style, but may not be pixel-identical to the original.

BEFORE DEPLOYING TO NETLIFY:
1. Open assets/config.js.
2. Replace https://YOUR-BACKEND-URL with your deployed Spring Boot backend base URL, for example https://campusfind-api.example.com (no trailing slash).
3. Deploy the CONTENTS of this frontend folder to Netlify (not the parent folder).

The backend must allow this Netlify origin through FRONTEND_ORIGIN. API routes used:
GET /api/health
GET /api/items
GET /api/stats
POST /api/items
POST /api/items/{id}/photo

A report needs type, category, title, location, date, contact name, contact email/phone, and a private management code (4-20 chars). Keep the management code private.
