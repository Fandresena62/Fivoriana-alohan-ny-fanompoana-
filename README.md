# Hevitra 30 — Fivoriana alohan’ny fanompoana

PWA tsotra, azo apetraka amin’ny Android ary natao hiasa offline rehefa voasokatra indray mandeha tamin’ny HTTPS. Tafiditra ao amin’ny `index.html` ny votoaty 30, ka tsy mila internet ny famakiana azy rehefa voatahiry ny app shell.

## Ao anatin’ity tetikasa ity
- `index.html` — interface sy votoaty Hevitra 30
- `manifest.webmanifest` — mamaritra ny PWA
- `sw.js` — mitahiry ny app mba hiasa offline
- `icons/` — sary famantarana
- `vercel.json` — fanamboarana static hosting
- `APK_GUIDE_MG.md` — torolalana hamoronana APK

## 1. Ampidiro ao amin’ny GitHub
1. Midira ao amin’ny https://github.com ary mamoròna repository vaovao, ohatra `hevitra-30-fanompoana`.
2. Sokafy ilay repository ary fidio **Add file → Upload files**.
3. Alefaso ny rakitra rehetra ato amin’ity folder ity, miaraka amin’ny `icons/` sy ireo rakitra miafina raha misy.
4. Tsindrio **Commit changes**.

Azonao atao koa ny manaisotra ZIP, dia mampiasa Git amin’ny solosaina raha zatra izany ianao.

## 2. Alefaso amin’ny Vercel
1. Midira ao amin’ny https://vercel.com ary fidio **Add New → Project**.
2. Ampifandraiso amin’ny GitHub ka fidio ny repository.
3. Framework Preset: **Other**.
4. Build Command: avelao banga (na esory).
5. Output Directory: `.` (root folder).
6. Tsindrio **Deploy**.
7. Rehefa vita, sokafy amin’ny HTTPS ilay adiresy Vercel. Sokafy indray mandeha amin’ny internet ilay app mba hahafahan’ny service worker mitahiry azy.

## 3. Apetraho amin’ny Android ho PWA
1. Sokafy amin’ny Chrome Android ilay URL Vercel.
2. Tsindrio ny menio ⋮.
3. Safidio **Install app** na **Add to Home screen**.
4. Omeo anarana raha angatahina, dia apetraho.

Ny famakiana votoaty dia miasa offline rehefa voatahiry ny app. Ny fametrahana voalohany sy ny fanavaozana dia mila internet.

## Fanavaozana
Rehefa manova votoaty ao amin’ny `index.html` ianao dia ovao koa ny `CACHE_NAME` ao amin’ny `sw.js` (ohatra `hevitra30-v2`) mba hahazoana ny kinova vaovao rehefa alefa indray.

## Fanamarihana
- Tsy mila API na database ivelany ity app ity.
- Ny andinin-teny dia fanondroana; vakio ao amin’ny Baiboly ampiasainareo.
- Ny APK dia dingana fanampiny; jereo ny `APK_GUIDE_MG.md`.
