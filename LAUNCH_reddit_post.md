TITLE: I built a free AI QA tool for vibe-coded apps — single HTML file, no signup, no backend

Hey r/webdev,

Been building with Lovable/Bolt/Cursor and kept running into the same problem — I'd ship something and have no easy way to QA it without being an engineer. So I built VibeCheck.

**What it does:**
- Drop a URL → it actually crawls your live page (real DOM parsing, not just AI guessing)
- Get a full QA report across 8 categories in ~30 seconds
- OWASP Top 10 security audit, accessibility check, form validation, mobile responsiveness, auth patterns
- Code Review mode: paste any code (30+ languages), get issues with OWASP/CWE references, UAT test scenarios, and a one-click "Insert Fix" button that patches your code in place with a diff view

**The no-backend trick:**
The whole thing is a single HTML file. Crawling works via a 5-layer proxy fallback (allorigins → codetabs → corsproxy → Wayback Machine → manual HTML paste for auth-walled apps). Reports are base64-encoded into the URL hash so you can share them without a server.

**What you get:**
- Scored report (0-100) with animated ring
- Per-issue fix confidence score
- Severity filter (Critical / Warnings / Info) + live search
- Report history (last 8 saved in localStorage)
- HTML / PDF / Word export
- Shareable URL — every shared report is a self-contained link

Free and open source: [github link]

Runs on the Anthropic Claude API — you bring your own key (free tier at console.anthropic.com).

Happy to answer questions. Feedback welcome, especially on the crawl accuracy.

---
*Built this as a lead-gen tool for my consulting firm but figured the community would get more use out of it open source.*
