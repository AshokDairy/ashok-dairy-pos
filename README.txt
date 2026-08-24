Ashok Dairy — installable counter app (PWA)
============================================

FILES
  index.html            the whole app
  manifest.webmanifest  name, icons, standalone display
  sw.js                 service worker (offline cache)
  icon-192.png / icon-512.png

INSTALL ON A PHONE (needs an https address)
  1. Put this folder online. Free options: Netlify Drop (drag the folder onto
     app.netlify.com/drop), GitHub Pages, Cloudflare Pages, or any web host.
  2. Open the https link on the phone.
  3. Android/Chrome: menu -> "Install app" / "Add to Home screen".
     iPhone/Safari: Share -> "Add to Home Screen".
  4. It then opens fullscreen, works offline, and keeps its own data.

QUICK TRY WITHOUT HOSTING
  Open index.html directly on the device. Everything works except offline
  caching (service workers need https).

DATA
  Sales, prices, product photos, customers and shop details are stored in this
  browser's local storage on that one device. Use Setup -> "Export sales as CSV"
  regularly as a backup. Clearing browser data erases everything.

PRINTING
  Print opens the system print dialog with an 80 mm thermal-slip layout.
  Works with any printer the phone/desktop can already reach (including a
  Bluetooth/USB thermal printer set up in the OS).
