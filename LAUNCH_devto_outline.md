TITLE: I built a zero-backend AI QA tool as a single HTML file — here's how the crawl trick works

TAGS: webdev, javascript, ai, showdev

INTRO:
The problem with vibe coding isn't writing the code — it's checking it afterward.

[Hook: 63% of vibe coders aren't developers. They ship apps using Lovable/Bolt and have no easy way to QA them.]

SECTION 1: The no-backend crawl system
- Why CORS is actually solvable with public proxies
- The 5-layer waterfall: allorigins → codetabs → corsproxy → Wayback Machine → manual paste
- What Promise.allSettled() does for parallel proxy racing
- Why Wayback Machine is a secret weapon for auth-walled sites

SECTION 2: What we actually parse from the live DOM
- DOMParser in the browser — no puppeteer needed
- Real form field extraction (type, name, label association, required, autocomplete)
- Framework fingerprinting from script srcs + inline JS patterns
- WCAG quick wins without a headless browser

SECTION 3: The URL-as-database trick
- Encoding full report JSON into the URL hash (#r=base64...)
- history.replaceState() — no back button pollution  
- Why this beats a real database for a tool like this

SECTION 4: The Code Review engine
- Building an OWASP Top 10 prompt that actually works
- Getting Claude to reference real line locations
- Fix confidence scoring without ground truth

SECTION 5: What's next
- PayPal paywall for premium reports
- Next.js rebuild when demand justifies a backend
- White-label for agencies

GITHUB: [link]
