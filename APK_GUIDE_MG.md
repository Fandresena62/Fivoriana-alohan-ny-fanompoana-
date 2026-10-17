# Torolalana: mamorona APK avy amin’ny Hevitra 30

**Soso-kevitra:** apetraho aloha amin’ny Vercel ny PWA, dia ampiasao PWABuilder hanamboarana APK. Mila solosaina amin’ny dingana sasany, ary mety hiova ny menus arakaraka ny kinovan’ny fitaovana.

## Safidy A — PWABuilder (mora indrindra)
1. Ataovy deploy aloha ny app amin’ny Vercel, ka ataovy azo sokafana amin’ny HTTPS.
2. Sokafy https://www.pwabuilder.com/
3. Apetaho ny URL Vercel ary atombohy ny fanombanana.
4. Araho ny toromarika momba ny manifest, icons ary service worker raha misy fanitsiana asaina atao.
5. Safidio ny **Package for Stores** na safidy Android/Google Play (miankina amin’ny interface ankehitriny).
6. Ampidino ny fonosana Android vokariny ary araho ny toromarika ao anatiny. Mety hangataka Android signing key izy.
7. Raha APK azo apetraka mivantana no vokatra omena, alefaso amin’ny finday ary apetraho rehefa eken’ny Android ny fametrahana avy amin’io loharano io. Raha AAB no vokatra, natao indrindra hampidirina amin’ny Google Play izy fa tsy hapetraka mivantana toy ny APK.

## Safidy B — Bubblewrap / Trusted Web Activity (mila teknika kokoa)
1. Mila Node.js sy Java JDK amin’ny solosaina.
2. Araho ny torolalana ofisialy Bubblewrap: https://github.com/GoogleChromeLabs/bubblewrap
3. Mamoròna Android wrapper mifandray amin’ny URL Vercel.
4. Ampifandraiso amin’ny tranonkala ny Digital Asset Links (`/.well-known/assetlinks.json`) ary ampiasao ny signing certificate marina.
5. Amboary sy sonia ny APK/AAB araka ny torolalana Bubblewrap.

## Zava-dehibe
- APK/TWA dia mampiseho ilay tranonkala ao anaty app Android; tsy manova ho app native tanteraka.
- Ny offline dia miankina amin’ny service worker sy ny cache; sokafy indray mandeha amin’ny internet aloha ilay app.
- Aza mizara signing key na tenimiafina amin’olona.
- Raha ny tanjona dia ny hampiasa manokana amin’ny findainao, dia matetika ampy ny PWA apetraka amin’ny Chrome. APK no ilaina raha tena mila rakitra Android `.apk` misaraka ianao.
