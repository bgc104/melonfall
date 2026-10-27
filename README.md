# Melonfall website — melonfall.com (BUILT 2026-10-26, not yet hosted)

Static site for melonfall.com, built from the locked brand spec
(`../branding/BRANDING.md`) and the privacy draft
(`../appstore/privacy-and-review.md`). No build step — plain HTML.
Packaged for handoff as `../melonfall-site.zip`.

## Contents
- `index.html` — landing page (icon, wordmark, fruit ladder, features incl.
  the Watermelon Counter, "Coming soon to the App Store")
- `support/index.html` — serves at melonfall.com/support
- `privacy/index.html` — serves at melonfall.com/privacy
- `app-ads.txt` — AdMob verification file (commented placeholder; see below)
- `icon.png` — the 1024px app icon, also the favicon / apple-touch-icon
- `CNAME` — GitHub Pages custom-domain file (melonfall.com)

## Status of the go-live steps
1. ✅ melonfall.com registered (Benjamin, Dynadot, 2026-10-26).
2. ✅ Support address set: support@melonfall.com (in `support/index.html`).
   STILL NEEDED: the mailbox — or a forwarder to a mailbox Benjamin reads —
   must actually be live before App Review; reviewers may test it.
3. ✅ Privacy effective date set: October 26, 2026. (Re-confirm the AdMob
   data list against the final SDK integration before submitting the app.)
4. ⬜ HOSTING — Benjamin's call (2026-10-26): **GitHub Pages**. Put the
   CONTENTS of this folder at the repo root (the `CNAME` file with
   melonfall.com is already included), enable Pages (Settings → Pages →
   Deploy from branch, main / root), set the custom domain to melonfall.com,
   and at Dynadot add A records @ → 185.199.108.153 / 185.199.109.153 /
   185.199.110.153 / 185.199.111.153 (delete any Dynadot parking A record
   first) plus CNAME www → <his-username>.github.io. Tick "Enforce HTTPS"
   once GitHub provisions the certificate. Note: GitHub hosts no email —
   support@melonfall.com still needs Dynadot email forwarding or a mailbox,
   live before App Review (not before site launch).
5. ⬜ Once the AdMob account exists, replace the commented placeholder in
   `app-ads.txt` with AdMob's exact publisher line. Do not publish the
   placeholder as a live line.
6. ⬜ After hosting, verify all three URLs load, then the Support URL and
   Privacy URL in `../appstore/listing.md` are ready to paste into
   App Store Connect as written.

## Brand notes
Deep Teal #0B5563 background, Cream #FFF6E9 text, Flesh Red #FF3B47 primary
button, Rind Green #22A24B secondary, Fredoka for the wordmark/headings —
per BRANDING.md. Voice: short, juicy, no corporate filler.
