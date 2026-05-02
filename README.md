# Aero-Prox
Proxy and games for school if your bored
<<<<<<< HEAD
=======

## Scramjet Proxy
This project uses the Scramjet browser proxy for the in-app proxy browser.

### Local setup
1. Clone the Scramjet repository:
   ```sh
   git clone --recursive https://github.com/MercuryWorkshop/scramjet
   ```
2. Install dependencies:
   ```sh
   pnpm i
   ```
3. Start the Scramjet dev server:
   ```sh
   pnpm dev
   ```
4. Open `http://localhost:4141/` and then use Aero-Prox.

### Notes
- `openProxyBrowser()` now loads the target URL directly into the browser iframe.
- Raw HTML scraping features (`fetchViaProxy`) prefer a local Scramjet service at `http://localhost:4141/`, but now also fall back to public CORS proxy services when available.

### Hosting online
If you host Aero-Prox online, the main browser view will use a direct iframe load for URLs. This is simpler but may be blocked on many websites by `X-Frame-Options` or other frame restrictions.

For YouTube search, video parsing, and other HTML scraping features, you still need a local or self-hosted Scramjet proxy service. The direct iframe browser view does not proxy the page content for those scraping functions.
>>>>>>> f40e762 (Add project files)
