TWEET 1:
I built a free QA tool for vibe-coded apps and it's a single HTML file with zero backend.

Drop a URL → real report in 30 seconds.

Here's how the no-backend crawl trick works 🧵

TWEET 2:
The problem: you've shipped your Lovable/Bolt app and want to QA it but you're not an engineer.

Existing tools: require signup, GitHub repo, $25/review, or a Chrome extension.

VibeCheck: open the file. Done.

TWEET 3:
The crawl system uses 4 CORS proxies in parallel — fastest wins.

If all proxies fail (auth-walled app, bot protection):
→ Tries Wayback Machine archive
→ Crawls sitemap.xml for route structure  
→ Parses robots.txt for hints
→ "Paste HTML" tab as last resort

No backend. No server. Zero infra cost.

TWEET 4:
What it actually parses from your live page:

• Every form — fields, labels, required attrs, autocomplete
• Real button inventory
• Nav links
• Framework detection (React/Vue/Supabase/Stripe/Firebase)
• WCAG accessibility issues
• Open Graph tags
• Scripts & external dependencies

Claude then gets real data, not just your description.

TWEET 5:
Reports are shared via URL hash — base64-encoded JSON in the #r= fragment.

No database. No server. The report IS the URL.

Every shared report is a self-contained link that works forever.

TWEET 6:
Code Review mode hits:
• OWASP Top 10 (2025)
• CWE/SANS Top 25
• WCAG 2.2
• SOLID/DRY/12-Factor
• 30+ languages

Each issue: severity badge, standard reference (OWASP A03, CWE-79), "why this matters", and a copy-paste fix with confidence %.

One click inserts the fix with a diff view.

TWEET 7:
Anthropic just launched Code Review for Claude Code at $15-25/review for enterprise teams.

VibeCheck is free, zero-install, and built for the 63% of vibe coders who aren't developers and don't have a GitHub PR workflow.

Different market. Same problem.

TWEET 8:
Free & open source on GitHub → [link]

Bring your own Anthropic API key (free tier at console.anthropic.com).

Drop your Lovable/Bolt URL in a reply — I'll run a report live and share it back 👇

#vibecoding #buildinpublic #webdev #lovable #claudeapi
