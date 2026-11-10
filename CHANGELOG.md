# Changelog

Every release, newest first. Sites pick up a release within a week.

## 1.12.1 (2026-11-10)

- Logos for 54 more services, so 226 of the 399 have one (the rest show their
  initials). They come from Simple Icons and gilbarbara/logos, or from each
  brand's own press kit where its terms allow it to be shown; see CREDITS.md.
  Brands whose terms require a licence for their logo, such as Adobe, Amazon,
  Microsoft, LinkedIn, Salesforce and Canva, keep their initials.

## 1.12.0 (2026-11-10)

- 184 new services, from 215 to 399: chat and support (15), email, automation
  and pop-ups (25), embeds and social (39, eight of them providers WordPress
  embeds itself), maps, forms, booking and site tools (21), analytics, testing
  and monitoring (28), commerce, reviews, payments, affiliate, ads and push (44),
  and services common in Germany, Austria and Switzerland (12). Each has machine
  translations in seven languages; 58 have a logo.
- A new list in `match`, `frames`: page addresses that count only when a frame
  shows them, such as a booking or form page. A site's own script that merely
  links to such a page now runs, where a host pattern held it. Calendly and
  Google Maps use it, and so do the new booking and form services.
- 49 more WordPress plugins are named, each made to add one service, and four
  plugins' tracking scripts (Reddit, Snapchat, TikTok, Klaviyo) wait for consent
  with their service instead of running into a missing function.
- AdRoll, Quantcast, Marketo, Account Engagement and ScorecardResearch join
  `common`: tag managers often add them.
- bookingkit no longer cites a third party's repository.

## 1.11.1 (2026-11-07)

- PixelYourSite's `sessionStorage` key, which keeps the referrer the visit came
  from, is named, so it is held until a yes and cleared on a no.

## 1.11.0 (2026-11-07)

- PixelYourSite joins the list, under Marketing, and joins `common`. Its plugin
  writes a visitor ID, the traffic source, the landing page and campaign tags to
  first-party cookies before any choice. The cookies are named, so a consent tool
  can hold them and delete them on a no. No host names it: it runs on the site.

## 1.10.0 (2026-11-07)

- Burst Statistics, SlimStat Analytics, Koko Analytics and Independent Analytics
  join the list, under Statistics. Each runs on the site's own server, so no host
  names them: Burst and SlimStat are matched by their script handles, Koko,
  Independent Analytics and SlimStat by what they print in the page. Their data
  stays on the site, so the banner doesn't say it may leave the EU.
- YouTube, Vimeo and Google Maps join `common`. A page builder can load them from
  a script, so a widget added after a site's last scan had no rule on the page and
  loaded before any choice.

## 1.9.0 (2026-11-07)

- YouTube also matches `youtube.com/watch`, `youtu.be` and
  `youtube.com/player_api`, and Vimeo matches `vimeo.com/*`: one path segment
  or more, never the home page. WordPress's `[video]` shortcode takes these
  page addresses, and its player loads from them.
- WooCommerce order attribution joins `common`. It has no hosts, only cookies,
  so a scanned site that doesn't list it lost the rule and `sbjs_*` was set
  before any choice.
- Meta Pixel lists the paid PixelYourSite's plugin file.

## 1.8.0 (2026-11-07)

- Meta Pixel also waits on `fbq('track` and `fbq("track` in inline code, so a
  plugin that prints its pixel calls apart from the base code is held with it.
- Libsyn also matches `traffic.libsyn.com`, where episode files are served from.
- `wordpress.handles` may end in `*` to name a prefix, with at least six
  characters before it. Google Analytics uses `google_gtagjs*` and Google Ads
  `google_gtagjs-AW-*`, for Site Kit's Google tag gateway, which serves the tag
  from the site's own domain. Older plugins read the `*` as a character.

## 1.7.0 (2026-11-06)

- Add optional service-page guidance: 98 sourced English setup notes and
  caveats for 86 services, with note-level verification dates and revisions.
  The separate `dist/guidance/` bundle is a website build input and is not
  listed in the plugin's download manifest.
- Review all 210 service entries and apply supported corrections to 140,
  including cookie durations, storage identifiers, provider information and
  processing locations. Preserve permanent IDs and runtime format 1; add
  the narrow PayPal SDK v6 core path alongside existing detection.
- Add guidance validation, regression checks and pinned-release website
  import documentation. Record evidence and unresolved findings in the
  review ledger; this release does not certify every catalog fact or
  WordPress integration.
- Remove the unsupported Tag Manager consent claim from existing languages
  and remove stale Smartlook cookie translations so the corrected source
  text can be used. No new translations are generated.

## 1.6.0 (2026-11-05)

- Cloudflare Web Analytics joins `common.json`, because Cloudflare's automatic
  setup adds its beacon after the site has sent the page (#30).

## 1.5.0 (2026-11-04)

- HubSpot forms and chat, Functional, with machine translations in seven
  languages (#28).
- A host pattern's path may hold a `*` segment, standing for exactly one
  non-empty segment. Facebook embeds use it, so the Facebook SDK is External
  media in every language, not only the ten listed (#28).
- Point at the new veronalabs home (#27)
- Rename to CookieHold (#26)

## 1.4.0 (2026-11-01)

- 101 new services, each checked against the vendor's own pages, with machine
  translations in seven languages and 38 new logos (#7):
  - Chat, forms and scheduling: Help Scout Beacon, Zoho SalesIQ, Smartsupp,
    HelpCrunch, Re:amaze, Chatbase, Jotform, Tally, Pipedrive, HighLevel,
    Acuity Scheduling, Microsoft Bookings, TidyCal, YouCanBookMe, Google
    Calendar, OpenTable and Booking.com (#15, #16).
  - Reviews, marketing and push: Trustpilot, Trustpilot review invitations,
    Trusted Shops, OptinMonster, OneSignal, Mailjet, Leadfeeder, AddToAny,
    ChatGPT Ads and Kliken (#17).
  - Statistics, commerce, accessibility and widgets: Contentsquare, Zoho
    PageSense, Usermaven, Rybbit, Shopify Buy Button, UserWay, accessiBe,
    Elfsight, Jetpack Comments and The Trade Desk (#18).
  - Embeds: Apple Podcasts, LinkedIn embeds, Discord, TED, Issuu, Yumpu, Imgur,
    Unsplash, Matterport, Sketchfab, Strava, Libsyn, Audioboom, Mapbox, Google
    Translate and Google Trends (#19, #20).
  - Known by their cookies: Wordfence (Essential) and Popup Maker. Library
    CDNs, named but never held back (Essential): jsDelivr, cdnjs, UNPKG,
    BootstrapCDN, jQuery CDN, Google Hosted Libraries, WordPress.org and
    Jetpack Site Accelerator (#21).
  - More marketing, visitor tracking and translation: ConvertBox,
    FirstPromoter, TradeTracker, Stay22, Klook, Encharge, Zoho Marketing
    Automation, SalesViewer, Fraud Blocker, Microanalytics, VisitorTracking,
    Visable Website Leads (wlw) and GTranslate (#22).
  - More embeds, chat and booking: XING, Senja, Kuula, CloudPano, Heyflow,
    Instatus, Superchat, Bookeo, bookingkit, Eversports, Momoyoga, Phorest,
    Planity and Eventfrog (#23).
  - Kustom Checkout (Essential), Mux, Zoho Campaigns, VEGA, Found.ee, MyFonts,
    ShortPixel CDN and WPMU DEV CDN (Essential), Wikimedia Commons, Wix Media
    and Reddit embeds (#24).
- WordPress plugins and their script handles for 17 services, and the image
  and tile hosts feed and map plugins load: `cdninstagram.com`, `fbcdn.net`,
  `pbs.twimg.com` and `tile.openstreetmap.org` (#14).
- LinkedIn Insight Tag: `bcookie` is no longer marked HttpOnly. Pinterest's
  embed entry is now named "Pinterest embeds" (#24).

## 1.3.0 (2026-10-31)

- 33 new services, each checked against the vendor's own pages, with machine
  translations in seven languages and 17 new logos (#7):
  - Statistics and marketing: Matomo, Matomo Tag Manager, Piwik PRO,
    etracker Analytics, Metricool, VG WORT, Brevo, MailerLite, GetResponse,
    Kit and CleverReach (#8).
  - Features, payments and fonts: Awin, CleanTalk Anti-Spam (Essential),
    Cal.com, Lime Connect (Userlike), Zoho Bookings, Zoho Forms, Klarna
    (Essential), Paddle (Essential), Paddle Retain, Adobe Fonts, Font Awesome
    and Bunny Fonts (#10).
  - Embeds and widgets: Bunny Stream, Apple Music, Flickr, Loom, komoot,
    Pinterest embeds, Podigee, GetYourGuide, ProvenExpert and Trustindex (#11).
- `common.json`, built into `services.json` as `common`: 25 trackers that tag
  managers and plugins often add by JavaScript, which a consent tool can keep
  on every page (#12).

## 1.2.0 (2026-10-30)

- Google Fonts (Functional): `fonts.googleapis.com` and `fonts.gstatic.com`,
  with its logo and translations (#5).

## 1.1.1 (2026-10-28)

- Jetpack Stats logo, from Automattic's Jetpack brand kit.

## 1.1.0 (2026-10-28)

- One-colour logos for 56 services, in the new `logos.json` (#2).
- Shorter first sentences for Google Ads, PayPal marketing, Segment,
  WooCommerce order attribution and Yandex Metrica, so each fits a service
  card; a purpose's first sentence is now checked to fit.

## 1.0.0 (2026-10-27)

- First release.
