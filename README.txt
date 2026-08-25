Ashok Dairy — counter app (GitHub Pages deploy folder)
======================================================

DEPLOY
  Upload every file in this folder to the repo root of
  AshokDairy/ashok-dairy-pos (branch main), then set
  Settings -> Pages -> Source: main / (root).

FILES
  index.html            the whole app — all CSS, JS and product photos inline
  sw.js                 offline cache (network-first, so new deploys land immediately)
  manifest.webmanifest  install metadata
  icon-192.png          home-screen icon
  .nojekyll             stops GitHub from reprocessing the files

NOTES
  Product photos are baked into index.html as data URIs — nothing to load,
  nothing to break on a static host.
  Layout adapts by window width: phone < 700px, tablet rail 700-1079px,
  desktop ticket column 1080px+.
  Sales, price edits and credit are saved per device.
  Bills print an 80 mm thermal slip from Sales -> a bill -> Print.
