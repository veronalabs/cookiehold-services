# Credits

The list itself is GPL-3.0 (see [LICENSE](LICENSE)). It includes or draws on
these works, under their own licences.

## Open Cookie Database

`cookies/open-cookie-database.json` and the `cookies.json` built from it are a
converted copy of the Open Cookie Database.

- Source: https://github.com/jkwakman/Open-Cookie-Database, at the commit in
  `cookies/source.json`
- Copyright the Open Cookie Database contributors
- Licensed under the Apache License, Version 2.0 (see
  [cookies/LICENSE](cookies/LICENSE))
- Changes: the columns were reduced to name, wildcard, category, platform,
  retention and description; categories were mapped to this list's
  (Functional, Security and Necessary to essential, Personalization to
  functional, Analytics to statistics, Marketing to marketing); whitespace
  was collapsed; rows without a name and repeated name and platform pairs
  were dropped; rows were sorted by name. See `scripts/convert-cookies.mjs`.

Some services' cookie lifetimes also come from it, where the vendor's own
pages give none. Their `sources` link to it.

## webappanalyzer

https://github.com/enthec/webappanalyzer, GPL-3.0. A starting point for drafting
new services, which are then checked against the vendor's own pages before
they are added.

## WhoTracks.me

https://github.com/whotracksme, statistics under CC BY 4.0. Used only to decide
which services to check first, by how common they are. No tracker data from
WhoTracks.me is copied into this list.

## Logos

`logos/` and the `logos.json` built from it hold one-colour logos. Brand
names and logos are trademarks of their owners. They are here only to show
which service is which, and no endorsement is implied. Every logo was made one
colour and fitted to a 24×24 grid; see each source below.

### Simple Icons

https://github.com/simple-icons/simple-icons, version 16.36.0, CC0-1.0. For a
product of a larger brand (Meta Pixel, Cloudflare Turnstile, Zendesk Chat,
Acuity Scheduling),
the brand's own icon.

acuity-scheduling (`squarespace`), adroll (`adroll`), adyen (`adyen`),
afterpay (`afterpay`), akamai-mpulse (`akamai`), algolia (`algolia`),
apple-mapkit (`apple`), apple-music (`applemusic`),
apple-podcasts (`applepodcasts`), arcgis (`arcgis`), audioboom (`audioboom`),
baidu-tongji (`baidu`), bandcamp (`bandcamp`), bluesky (`bluesky`),
booking-com (`bookingdotcom`), bootstrapcdn (`bootstrap`),
braintree (`braintree`), brevo (`brevo`), bunny-fonts (`bunnydotnet`),
bunny-stream (`bunnydotnet`), buy-me-a-coffee (`buymeacoffee`),
cal-com (`caldotcom`), calendly (`calendly`),
campaign-monitor (`campaignmonitor`), carto (`carto`), cdnjs (`cloudflare`),
cloudflare-stream (`cloudflare`), cloudflare-turnstile (`cloudflare`),
cloudflare-web-analytics (`cloudflare`), dailymotion (`dailymotion`),
datadog-rum (`datadog`), discord-widget (`discord`), disqus (`disqus`),
dynatrace (`dynatrace`), emarsys (`sap`), facebook-embed (`facebook`),
fareharbor (`fareharbor`), fathom (`fathom`), flickr (`flickr`),
font-awesome (`fontawesome`), formstack (`formstack`), giphy (`giphy`),
github-gist (`github`), google-ads (`googleads`),
google-adsense (`googleadsense`), google-analytics (`googleanalytics`),
google-calendar (`googlecalendar`), google-docs (`googledocs`),
google-drive (`googledrive`), google-fonts (`googlefonts`),
google-forms (`googleforms`), google-hosted-libraries (`google`),
google-identity (`google`), google-maps (`googlemaps`),
google-pay (`googlepay`), google-tag-manager (`googletagmanager`),
google-translate (`googletranslate`), gravatar (`gravatar`),
gumroad (`gumroad`), help-scout (`helpscout`), hotjar (`hotjar`),
hubspot (`hubspot`), hubspot-forms (`hubspot`), imgur (`imgur`),
instagram-embed (`instagram`), instatus (`instatus`), intercom (`intercom`),
issuu (`issuu`), jquery-cdn (`jquery`), jsdelivr (`jsdelivr`),
kickstarter (`kickstarter`), klarna (`klarna`), klook (`klook`),
ko-fi (`kofi`), komoot (`komoot`), kununu (`kununu`), kuula (`kuula`),
lemon-squeezy (`lemonsqueezy`), livechat (`livechat`), loom (`loom`),
mailchimp (`mailchimp`), mapbox (`mapbox`), maptiler (`maptiler`),
matomo (`matomo`), matomo-cloud (`matomo`), matomo-tag-manager (`matomo`),
mautic (`mautic`), meta-pixel (`meta`), mixcloud (`mixcloud`),
mixpanel (`mixpanel`), new-relic (`newrelic`),
openstreetmap (`openstreetmap`), paddle (`paddle`), paddle-retain (`paddle`),
parsely (`parsedotly`), paypal (`paypal`), paypal-marketing (`paypal`),
pinterest-embed (`pinterest`), pinterest-tag (`pinterest`),
plausible (`plausibleanalytics`), pocket-casts (`pocketcasts`),
posthog (`posthog`), qualtrics (`qualtrics`), quantcast (`quantcast`),
quora-pixel (`quora`), rakuten-advertising (`rakuten`), razorpay (`razorpay`),
reddit-embed (`reddit`), reddit-pixel (`reddit`),
reverbnation (`reverbnation`), rumble (`rumble`), sentry (`sentry`),
shopify-buy-button (`shopify`), simple-analytics (`simpleanalytics`),
sketchfab (`sketchfab`), slideshare (`slideshare`), smugmug (`smugmug`),
snap-pixel (`snapchat`), soundcloud (`soundcloud`),
speaker-deck (`speakerdeck`), spotify (`spotify`), spreaker (`spreaker`),
square (`square`), strava (`strava`), stripe (`stripe`),
surveymonkey (`surveymonkey`), ted (`ted`), telegram (`telegram`),
threads (`threads`), tiktok-embed (`tiktok`), tiktok-pixel (`tiktok`),
tripadvisor (`tripadvisor`), trusted-shops (`trustedshops`),
trustpilot (`trustpilot`), trustpilot-invitations (`trustpilot`),
tumblr (`tumblr`), twitch (`twitch`), typeform (`typeform`),
umami-cloud (`umami`), unpkg (`unpkg`), unsplash (`unsplash`),
vimeo (`vimeo`), vk (`vk`), wikimedia-commons (`wikimediacommons`),
wistia (`wistia`), wix-media (`wix`), wolfram-cloud (`wolfram`),
wordpress-org (`wordpress`), x-embed (`x`), x-pixel (`x`), xing (`xing`),
youtube (`youtube`), zendesk-chat (`zendesk`), zoho-bookings (`zoho`),
zoho-campaigns (`zoho`), zoho-forms (`zoho`),
zoho-marketing-automation (`zoho`), zoho-pagesense (`zoho`),
zoho-salesiq (`zoho`).

### gilbarbara/logos

https://github.com/gilbarbara/logos, commit d6960ed, CC0-1.0. Colours merged
into one; the reCAPTCHA logo keeps its arrows and the Drip logo its drop,
without the word.

amplitude (`logos/amplitude-icon.svg`), braze (`logos/braze-icon.svg`),
customer-io (`logos/customerio-icon.svg`), drip (`logos/drip.svg`),
embedly (`logos/embedly.svg`), fomo (`logos/fomo-icon.svg`),
getyourguide (`logos/getyourguide.svg`),
google-recaptcha (`logos/recaptcha.svg`), heap (`logos/heap-icon.svg`),
mailjet (`logos/mailjet-icon.svg`), olark (`logos/olark.svg`),
onesignal (`logos/onesignal.svg`), optimizely (`logos/optimizely-icon.svg`),
segment (`logos/segment-icon.svg`), tealium (`logos/tealium-icon.svg`),
unbounce (`logos/unbounce-icon.svg`), vwo (`logos/vwo.svg`),
woocommerce-attribution (`logos/woocommerce-icon.svg`),
wufoo (`logos/wufoo.svg`)

### svgl

https://github.com/pheralb/svgl, commit 88467c0, MIT licence, copyright (c)
2022 Pablo Hdez. Gradients merged into one colour.

hcaptcha (`static/library/hcaptcha.svg`)

### Brands' own press kits

The symbol alone where the brand has one (otherwise its short wordmark), from
the brand's own press or brand page, made one colour. Where a brand's terms
forbid changing its logo, only a one-colour file it supplies is used, as
supplied.

- activecampaign: ActiveCampaign press kit https://www.activecampaign.com/brand
- aweber: AWeber press page https://www.aweber.com/press.htm. Its one-colour
  brandmark (`AW_BRANDMARK_GRAY.eps`), traced from the preview in that file
- birdeye: Birdeye press page https://birdeye.com/press/
- bookingkit: bookingkit press page https://bookingkit.com/press-page/. The
  cube from its logo
- brightcove: Brightcove branding hub https://www.brightcove.com/branding-hub.
  Its logo as supplied
- chaport: Chaport press page https://www.chaport.com/press. The symbol from
  its logo
- cj: CJ media kit https://www.cj.com/cj-media-kit. Its symbol as supplied
- cleantalk: CleanTalk press kit (linked from https://cleantalk.org/about).
  Its logo without the word ("Only logo.svg")
- cleverreach: CleverReach press page https://www.cleverreach.com/en/press/.
  Its figurative mark, as supplied
- codepen: CodePen logos page https://blog.codepen.io/documentation/logos/.
  The cube from its logo. Its 2014 post
  https://blog.codepen.io/2014/03/07/codepen-icon/ says "free to use the
  CodePen icon pretty much however you want."
- cognito-forms: Cognito Forms media kit
  https://www.cognitoforms.com/newsroom/media-kit
- comm100: Comm100 newsroom https://www.comm100.com/newsroom/. The symbol from
  its monochrome logo
- crisp: Crisp brand assets, https://crisp.chat/en/about/
- digistore24: Digistore24 press page https://www.digistore24.com/de/presse/
- ecwid: Ecwid media page https://www.ecwid.com/media. The cart icon from its
  logo
- eversports: Eversports press page
  https://www.eversportsmanager.com/de-AT/presse
- jameda: jameda press portal https://presse.jameda.de/presskits/logo. The
  symbol from its logo
- jetpack-comments, jetpack-stats, wordpress-com-cdn: Automattic brand
  materials (the Jetpack brand kit)
  https://automattic.com/press/brand-materials/. Its terms name Automattic's
  partners and editorial use; the logo is used here only to identify the
  service.
- judge-me: Judge.me media kit https://judge.me/media-kit. Its white symbol,
  as supplied; the kit offers it "For compact placements where Judge.me is
  already identified"
- kit: Kit brand page https://kit.com/brand. Its wordmark; Kit has no separate
  symbol
- loyaltylion: LoyaltyLion brand guidelines
  https://loyaltylion.com/resources/brand-guidelines. Its black icon, as
  supplied
- mouseflow: Mouseflow press page https://mouseflow.com/press-releases/
- openai-ads: OpenAI design guidelines https://openai.com/brand/
  (openai-logos.zip). The black Blossom. Its terms: "Use the logo only when it
  directly relates to OpenAI services."
- optinmonster: OptinMonster press page https://optinmonster.com/press/. The
  Archie mascot
- podium: Podium press page https://www.podium.com/press. The symbol from its
  black logo
- popup-maker: Popup Maker brand assets https://wppopupmaker.com/brand-assets/
- privy: Privy press page https://www.privy.com/press
- provenexpert: ProvenExpert press materials
  https://www.provenexpert.com/en-us/press-material/. The check mark from its
  square logo
- quantum-metric: Quantum Metric brand assets
  https://www.quantummetric.com/brand-assets. Its brandmark, as supplied
- rapidmail: Positive Group press kit
  https://www.positivegroup.com/fr/presse-et-kit-media/. The rapidmail
  logomark, as supplied
- resmio: resmio press page https://www.resmio.com/presse/. The symbol from
  its black logo
- reviews-io: REVIEWS.io brand guidelines
  https://www.reviews.io/front/brand-guidelines
- rybbit: Rybbit brand kit https://rybbit.com/brand
- shortpixel-cdn: ShortPixel media kit https://shortpixel.com/ (footer,
  MediaKIT.zip). Its robot
- snowplow: Snowplow newsroom https://snowplow.io/newsroom
- taboola: Taboola branding page https://www.taboola.com/branding
- tally: Tally press kit https://tally.so/help/press-kit. Its icon, as
  supplied
- tidio: Tidio brand PDF https://assets.tidio.com/homepage/brand/assets.pdf
- usersnap: Usersnap press page https://usersnap.com/press. Its icon
- weglot: Weglot press page https://www.weglot.com/press
- yotpo: Yotpo brand kit https://www.yotpo.com/about/. Its wordmark; no
  separate symbol is offered
