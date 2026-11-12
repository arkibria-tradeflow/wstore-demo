# WStore Demo

Reusable wholesale digital showroom demo, currently branded for **GMS Store**, Al Murar, Dubai.

## Customer journey
- Responsive homepage and product catalogue with search, categories and sorting.
- Product specifications, carton quantities and optional item notes.
- Multi-item enquiry basket with automatic piece totals.
- Contact form and formatted WhatsApp message preview.
- WhatsApp handoff to +971 54 129 6145; the visitor must tap Send.
- Store details, phone and Google Maps directions.

## Run
Serve this directory with any static web server, e.g. `python3 -m http.server 8000`, then visit http://localhost:8000.

## Publish with GitHub Pages
Repository Settings → Pages → Deploy from a branch → `main` → `/ (root)` → Save.

## Reuse
Edit `config.js` to change store information. Sample products and illustrations are defined in `app.js`; replace them with the client's actual catalogue before production use.

## Demo boundaries
This is a static customer-facing prototype. Product availability and specifications are illustrative. It does not connect to Google Sheets yet and has no server, shared enquiry inbox, admin authentication, quote editor, analytics or inventory deduction. Basket data is stored on the visitor's device, and enquiry contact details are retained in session storage and included in the WhatsApp handoff. It does not claim messages are delivered or received.

## Future integration
Connect a private Google Sheet through a server-side product adapter; keep credentials off the public repository. Add database-backed enquiries and real authentication separately if required. Keep the business website independent from any future Tradero integration.
