# HEXVAULT standalone (with official TON Connect)

1. Open index.html and edit the HV_CONFIG block at the top:
   - tonAddr: your Tonkeeper address
   - tonRate: price of 1 TON in USD
   - manifestUrl: https://YOUR-SITE.com/tonconnect-manifest.json
   - orderEndpoint: optional, a Formspree URL that emails you every order
2. Open tonconnect-manifest.json and replace YOUR-SITE.com with your real domain.
3. Upload index.html, tonconnect-manifest.json and icon.png to one host over https
   (Netlify Drop, Vercel, GitHub Pages or Cloudflare Pages all work).
4. Open your site, add an item, go to Payment and press Connect Wallet.

Notes: there is no admin panel or customer accounts in this version.
Edit the product list (SEED in index.html) by hand. Orders reach you through
orderEndpoint. Payments are matched by their exact amount (no comment needed).
