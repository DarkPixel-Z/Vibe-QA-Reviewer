VibeCheck is a free, zero-install QA tool for apps built with Lovable, Bolt, Replit, Cursor, and other AI coding tools — delivered as a single HTML file with no backend required.

**Drop a URL → real QA report in 30 seconds.**

Unlike other QA tools, VibeCheck actually crawls your live page using a 5-layer proxy fallback system (CORS proxies → Wayback Machine → sitemap.xml → manual HTML paste for auth-walled apps). Claude then gets your real form fields, nav links, buttons, and detected frameworks — not just your description.

**App QA Mode — 8 categories:**
Navigation, Forms, Auth, Error Handling, Mobile Responsiveness, Performance, Accessibility (WCAG 2.2), Data Persistence. Each with a scored report, per-issue code fixes, and shareable URL.

**Code Review Mode — 30+ languages:**
OWASP Top 10 (2025), CWE/SANS Top 25, SOLID/DRY/12-Factor, UAT test scenarios with automation hints, per-issue confidence scores, and a one-click Insert Fix button with before/after diff view.

**Everything else:**
Severity filter + live search, report history, PDF/Word/HTML export, multi-file code tabs, re-run after fixes, copy full fixed file.

**The no-backend trick:** Reports are base64-encoded into the URL hash. Share a report = share a URL. No server, no database, no login.

Bring your own Anthropic API key. Free tier works fine.
