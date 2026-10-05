# Singapore PM2.5 PWA

A simple Progressive Web App that retrieves the latest Singapore PM2.5 readings from:

https://api-open.data.gov.sg/v2/real-time/api/pm25

## Important

A PWA must be served over HTTPS (or localhost during development) for the service worker and installability features to work.

## Easiest deployment: GitHub Pages

1. Create a GitHub repository.
2. Upload all files in this folder to the repository root.
3. Enable GitHub Pages for the repository, using the main branch and root folder.
4. Open the resulting HTTPS address on your Android phone in Chrome.
5. In Chrome, use **Add to Home screen** (or **Install app**, depending on the Chrome version).

The app makes the PM2.5 API request directly from the browser. It does not contain an API key.

## Local testing

For a simple local test, use a local web server rather than opening index.html directly.

For example, with Python:

    python -m http.server 8000

Then open:

    http://localhost:8000/

Service-worker installation requires HTTPS except for localhost.
