# Magmafy Recruiting Form

Static one-page careers site for the Media Buyer role (HTML/CSS/JS, no build step).

- `index.html`: job description + application form
- `logo-mark.webp`: Magmafy logo

## How it works
On submit the form posts the answers to a Google Apps Script web app that appends a row to a Google Sheet
(`SHEET_ENDPOINT` in `index.html`). The result panel also offers a prefilled WhatsApp message to
`https://wa.me/966590873178` (`WHATSAPP` constant). While `SHEET_ENDPOINT` is empty, only the WhatsApp flow is used.

The Apps Script code and setup steps live in the `Magmafy-Applicants` repo (`apps-script/Code.gs`).

## Deploy
Hosted on GitHub Pages (branch `main`, folder `/`) at `careers.magmafyogp.com` (see the `CNAME` file).
DNS: add a `CNAME` record `careers` pointing to `mrvoroo.github.io` at the domain's DNS provider.
Then in the repo: Settings > Pages > Custom domain `careers.magmafyogp.com` and tick Enforce HTTPS.
