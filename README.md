# Gorgflix: put it online for free

This folder is the whole website. It has no server and nothing to build.

Files: index.html (the app), manifest.webmanifest and sw.js (install + offline),
icons, _headers (security headers), robots.txt.

## 1. Deploy (pick one, all free)

**Cloudflare Pages (easiest, unlimited bandwidth)**
1. Make a free account at dash.cloudflare.com
2. Workers & Pages > Create > Pages > Upload assets
3. Drag in this folder (or the zip). Click Deploy.
4. You get https://YOUR-NAME.pages.dev

**Netlify Drop**
1. Go to app.netlify.com/drop
2. Drag this folder onto the page. You get https://something.netlify.app

**GitHub Pages**
1. Create a public repo and upload these files to the main branch.
2. Settings > Pages > Deploy from a branch > main / (root).
3. You get https://YOUR-USER.github.io/YOUR-REPO/

The site must be https (all three do this automatically). Addons must be https too.

## 2. Install it like an app
- iPhone: open the link in Safari > Share > Add to Home Screen.
- Android / Chrome / Edge: use the Install button in Settings > About, or the browser menu.
- Desktop Chrome / Edge: install icon in the address bar.

## 3. Domain
The free .pages.dev / .netlify.app / .github.io address is a real, permanent URL.
A custom domain (yourname.com) costs about $10 a year; every host above lets you attach one.

## 4. App stores are NOT free
Apple Developer is $99 per year, Google Play is a $25 one-time fee, and both review apps.
The installable website above gives iPhone and Android users the same thing for free.

## 5. Before you share it publicly
- Name and logo: "Gorgflix" sounds like Netflix, and the green ogre can read as a famous
  movie character. For a public launch, consider a more distinctive name and mascot.
- Do not ship piracy addons as defaults. The app's built-in sources are legal ones.
- Accounts are stored in each person's own browser. That is fine for family profiles on one
  device, but there is no cross-device sync or password reset. Real accounts need a free backend
  such as Supabase or Firebase.
- Settings > About already has the disclaimer, privacy note and TMDB attribution.

## 6. Updating
Edit index.html, change VER in it and V in sw.js (for example 1.0.1), then upload again.
