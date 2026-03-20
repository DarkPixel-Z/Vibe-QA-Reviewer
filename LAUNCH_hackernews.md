TITLE: Show HN: VibeCheck – AI QA tool for vibe-coded apps, single HTML file, no backend

I built a QA tool for apps built with AI coding assistants (Lovable, Bolt, Cursor, Replit). The whole thing is a single HTML file with no backend, no server, no signup.

The interesting engineering bit: it actually crawls the live URL using a parallel proxy waterfall — 4 CORS proxies race each other, then falls back to Wayback Machine archive, then sitemap.xml + robots.txt parsing, then a manual HTML paste mode for auth-walled apps. The parsed DOM data (real forms, inputs, nav, scripts, framework detection) gets fed directly to Claude alongside the AI analysis prompt, so findings reference actual element names rather than generic advice.

Reports are shared via URL hash — full report JSON base64-encoded into the #r= fragment. No database, no server. The URL is the report.

Code Review mode runs OWASP Top 10 (2025), CWE/SANS Top 25, WCAG 2.2, and language-specific checks across 30+ languages. Each issue includes a fix confidence score and an Insert Fix button that patches the textarea in place with a side-by-side diff view.

Runs on Claude API (user brings their own key). Free and open source.

GitHub: [link]
