PENNY - WALLET APP UI
=====================

Files
-----
index.html      Markup: splash screen, signup/login page, Telegram pop-up, wallet
style.css       All styling (wallet sized from the mockup, 368px-wide design)
script.js       Splash timing (about 3.3s + soft fade), balance count-up, globe/plane animation,
                signup/login flow, bottom navigation
manifest.json   Home-screen install settings
icon-192.png    App icon
icon-512.png    App icon (large)
penny-logo.jpg  Splash screen logo (unchanged)
globe.jpg       Original signup/login illustration (unchanged; shown if motion is reduced
                or if the layer images below fail to load)
globe-sphere.png  Globe layer cut from globe.jpg (airplane/note/trail removed)
globe-props.png   Note and lock layer cut from globe.jpg
penny-plane.png   Paper airplane cut from globe.jpg

How it works
------------
- Every launch: blue splash (logo pop-in, light sweep, gentle breathing, about 3.3s), then it
  dissolves into the signup/login page.
- Create an account / Log in opens a pop-up for Telegram username + password.
- Done opens the wallet. The username is remembered on the device, so later
  launches go splash -> wallet. The balance counts up from 0.00 once per login. Tap your name in the wallet to log out.
- This is front-end only: passwords are not stored or verified. Real Telegram
  sign-in needs a backend that validates Telegram's initData.

Run on GitHub Pages
-------------------
1. Create a new repository and upload all the files to the root.
2. Go to Settings > Pages.
3. Under Source, choose "Deploy from a branch", pick main and / (root), then Save.
4. Open the link GitHub gives you (https://<username>.github.io/<repo>/).

Install on your phone
---------------------
iPhone (Safari): Share > Add to Home Screen.
Android (Chrome): Menu > Install app / Add to Home screen.

Notes
-----
- The font (DM Sans) loads from Google Fonts, so it needs an internet connection.
- Keep all files in the same folder so the paths resolve.
