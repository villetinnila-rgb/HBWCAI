# HBWCAI — The Beatles Cruise AI

**All You Need Is Love. And One Link.** 🎸

AI-first cruise programme and offer-feed proof of concept. Rather than building a new chatbot, an organizer publishes one structured data feed. Each passenger can give its link to the personal AI they already use.

## What's in the demo?

- `cruise.json`: UTF-8 JSON feed: ship/event details, historical context, fictional line-up, 25 scheduled events, 9 offers, locations, FAQs and safety-aware assistant instructions.
- `index.html`: mobile-friendly concept preview, reading `cruise.json`. For GitHub Pages hosting, enable Pages → Deploy from branch → main → root.

## Reality check

**Everything involving the illustrated 2027 cruise is fictional**, including performances, timetables, offers, prices, decks, venues and bookability. This is **not** an official Viking Line announcement, nor a verified Helsinki Beatles Weekend 2027 programme.

**Historical context verified:** The real fifth Helsinki Beatles Weekend Beatles cruise took place 25–27 September 2026 aboard Viking Cinderella between Helsinki and Stockholm. Announced performers included Jiri Nikkinen The Beatles Tribute Band, Jay Goeppner & The Urban Crow, The Beat Brothers and Hitmen Beatlemania; Freda Kelly was a special guest. The 2027 mock programme uses some historical performers **only as illustrative demo content**: nothing here confirms their participation in a future event.

Sources:
- [Helsinki Beatles Weekend](https://www.beatlesweekend.fi/en/)
- [Viking Line Beatles Cruise](https://www.vikingline.fi/beatles)
- [Viking Line Åland Beatles cruise](https://www.vikingline.ax/kryssning/nojeskryssningar/beatles-kryssning/)

## One-link experiment

Once this is hosted in a *public* GitHub repository called `HBWCAI`, the feed will be accessible at:

`https://raw.githubusercontent.com/villetinnila-rgb/HBWCAI/main/cruise.json`

Copy the link to your AI and ask (in Finnish, Swedish or English):

> Lue tämä Beatles-risteilyn demo-ohjelma. Rakasta Abbey Roadin medleytä, haluan nähdä kaksi keikkaa ja syödä hyvin. Tee minulle lauantain suunnitelma kellonaikoineen ja poimi sopivat tarjoukset. Kerro mitkä tiedot ovat keksittyjä.

**Important:** Some AI assistants can fetch a public URL directly, while others require a browser capability, connector or pasted JSON. Just scanning a QR code will not automatically install a persistent feed in every AI product. Fresh data and automatic background updates require explicit support.

## Content model

- `event`: cruise overview and timezone
- `historical_inspiration`: real 2026 source context
- `places`, `performers`, `schedule`: structured entertainment information
- `offers`: commercial mock offers, prices, validity windows and targeting tags
- `recommendation_examples`: examples of user preference → relevant items
- `assistant_instructions`: accuracy, safety and non-hallucination guidance
- `integrations`: intentionally disabled booking, payments and live availability

All times are illustrative. The feed intentionally avoids tracking passengers, collecting personal data, and assuming the personal AI knows how to monitor changes.

**One link = a new AI-era content and discovery channel.**