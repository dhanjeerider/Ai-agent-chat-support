# PulseChat Support — your own live chat, on your own server, with no monthly bill

**A Tawk.to-style live chat and customer-support platform you install once and own forever.**
PHP 8 + SQLite + vanilla JavaScript + Tailwind CSS + Font Awesome. No Composer, no Node on the server, no third-party service, no per-agent pricing — every chat, ticket and lead stays in a single SQLite file on your own hosting.

Put one line of code on any website — WordPress, Shopify, Wix, plain HTML — and visitors get a friendly chat bubble with a real help desk behind it.

![PulseChat widget embedded on a third-party store](https://iili.io/n1D5hPI.jpg)

---

## Why users ask for exactly this

- **No subscription.** Tawk.to, Crisp, Intercom — you rent them forever. PulseChat is yours after one install.
- **Your data never leaves your server.** Names, e-mails, chats, tickets, uploads — all in `data/pulsechat.sqlite`.
- **Works on any site.** One `<script>` tag. The host page loads nothing from your panel — not a font, not a framework.
- **Nothing is a mock-up.** Every button, toggle and menu in the screenshots below is wired to a real database action. There are no dead ends.
- **Opens instantly.** No build step, no CDN, no API keys for the core chat.
- **Friendly to slow hosting.** SQLite + plain PHP runs fine on the cheapest shared plan.

---

# Part 1 · What your visitors get

## 1. A launcher that lives on any website

One script tag injects the bubble. Colours, label, position and theme come from your own **Chat setup** screen, and the chat opens in an isolated frame so the customer's site can never break it — and your styles can never leak into their site.

![The chat launcher on a third-party store page](https://iili.io/n1D5hPI.jpg)

- ~15 KB loader (4.6 KB gzipped) — no jQuery, no build tools.
- Works on plain HTML, WordPress, Shopify, Wix, Squarespace, React, Laravel — anywhere a `<script>` tag runs.
- If the customer's theme re-renders the page, the launcher puts itself back instead of disappearing.
- Unread badge, sound and desktop notifications are handled by the widget.

## 2. Pre-chat form — asked once, remembered forever

Ask for name, e-mail, phone, company, subject, department and a first message — or switch any of them off in one click. What the visitor types is saved on their device, so the **next visit opens straight into the chat**. No account, no sign-up, no cookie banner.

![Pre-chat form with remembered visitor details](https://iili.io/n1D5wFt.jpg)

## 3. Live messages — no page refresh, ever

Agent replies appear on their own in the visitor's panel, inside the widget and on the standalone chat page. The heartbeat asks only for what is new since the last message, so it stays light: it speeds up when someone is typing, backs off when the tab is idle, and pauses completely on a hidden tab.

![Agent reply arriving live in the visitor's chat](https://iili.io/n1D5NcX.jpg)

- Typing indicator both ways.
- Delivery states, unread counters, auto-scroll.
- Works even if the visitor never reloads the page.

## 4. A composer that feels like a real messenger

Emoji picker, image and file attachments with previews, drag-and-drop, in-chat search, e-mail transcript, and a transcript PDF. Uploads are size-limited, extension-checked and MIME-verified before they are stored.

![Attachments, emoji picker, search and transcript](https://iili.io/n1D5k9s.jpg)

## 5. Visitors can raise and follow their own tickets

This is the feature most chat scripts forget. Your customers get a **Tickets** tab: raise a ticket with a priority, add details, read the team's reply, watch the status change — with an unread badge on the tab. It is the same ticket queue your agents work in.

![Visitor raising a ticket from inside the widget](https://iili.io/n1D5gol.jpg)

## 6. A help centre inside the chat

Articles you write yourself, or import from PDFs, sitemaps and URLs, are searchable from the widget's **Help** tab. As the visitor types, matching articles are suggested before they even send the message — which quietly deflects the same questions over and over.

![Help centre tab inside the widget](https://iili.io/n1D54PS.jpg)

## 7. Offline capture: e-mail, Telegram or phone

When nobody is online, the visitor is never met with a dead end. The widget asks for a contact channel — **e-mail, Telegram username or phone** (WhatsApp optional) — stores it on the visitor, raises a ticket, and **shows the saved details back inside the chat** on the next visit, with a *change* button.

![Offline form capturing e-mail, Telegram or phone](https://iili.io/n1D5PK7.jpg)

## 8. Mobile-first, both sides

On a phone the widget fills the screen instead of floating a cramped card in the corner — same features, same live updates. The agent panel is mobile-ready too, with off-canvas navigation and a composer that stays above the keyboard.

![The chat widget on a phone](https://iili.io/n1D7zlt.jpg)

---

# Part 2 · What your team gets

## 9. Dashboard that tells the truth

Live KPIs straight from SQLite: active visitors, open and unassigned chats, open tickets, unread messages, today's conversations and tickets, a 14-day trend and who is online right now. Click any number and you land on the list behind it.

![Agent dashboard with live KPIs](https://iili.io/n1D5il9.jpg)

## 10. Inbox with full visitor context

The live queue on the left, the conversation in the middle, and everything about the visitor on the right: page trail, device, browser, location, previous chats, tickets, notes. Agents get canned replies, an AI draft, internal notes, assignment, tags, transcript e-mail, and a **delete chat** action.

![Agent inbox with visitor context panel](https://iili.io/n1D5QHu.jpg)

## 11. Visitor tracking and a real leads export

See everyone on your site right now, what they are reading, and where they came from. Every visitor who left a name, e-mail or phone becomes a **lead you can export to CSV** in one click — plus bulk delete for the ones you do not need.

![Visitor tracking with leads export](https://iili.io/n1D5ZAb.jpg)

## 12. Ticket desk

Visitor tickets land in one place with priority, status, department and requester details. Reply, reassign, set the priority, close, or delete — and the visitor sees the reply in their own Tickets tab.

![Agent ticket desk](https://iili.io/n1D5moQ.jpg)

## 13. Knowledge base that actually saves

Write articles by hand, or import a **PDF**, a **sitemap** or a **URL** and let the text be extracted and indexed. Categories, tags, keywords, helpfulness voting, drafts and a public, searchable help centre at `kb.php` for SEO.

![Knowledge base with imports and live editing](https://iili.io/n1D7fDv.jpg)

## 14. Auto-replies, shortcuts and triggers

Keyword rules answer instantly — contains, exact, starts-with, whole-words or regex — with priority, cooldowns, department scoping and "stop further rules" chaining. Attach a help article to a rule and the visitor gets the answer *and* the link. The built-in tester shows which rule would fire before you switch it on.

![Auto-reply rules with a live tester](https://iili.io/n1D7BxR.jpg)

## 15. Analytics you can act on

Conversation volume, first-response and resolution times, department load, busiest hours, countries, top pages and visitor ratings — all computed from your own database, no external analytics.

![Analytics dashboard](https://iili.io/n1D7CVp.jpg)

## 16. Chat setup — the visitor-facing side, moved out of admin Settings

Everything a customer sees or feels lives here, at agent level: brand, welcome text, pre-chat form, remember-visitor, attachments, emoji, tickets, offline form, help centre, and the live sync interval — with a real `chat.php` preview beside the form. Server administration stays where it belongs, in Settings, for administrators only.

![Chat setup screen with live preview](https://iili.io/n1D5yiB.jpg)

## 17. Storage and cleanup, because disks fill up

Per-table disk usage, dry-run previews and one-click pruning of old messages, visitors, attachments and events, plus `VACUUM` to reclaim the space. Nothing accumulates silently.

![Storage and cleanup screen](https://iili.io/n1D7HKP.jpg)

## 18. Accounts — for the main administrator only

`dkkr5558@gmail.com` is the main admin and sees every account: its role, department, chats handled, tickets, active sessions and complete audit trail. Create agents, disable them, or hand over the owner crown — the server admin always stays in control. Agents never see this screen.

![Accounts list, main administrator only](https://iili.io/n1D7Jl1.jpg)

![Account drawer with roles, sessions and audit trail](https://iili.io/n1D73Hg.jpg)

## 19. Embed page for whoever owns the website

A ready snippet to copy, a direct `chat.php` link for e-mail signatures, and short step-by-step guides for WordPress, Shopify, Wix, Squarespace, plain HTML, Next.js and React — plus the widget's JavaScript API for developers.

![Install and embed page with the copy-ready snippet](https://iili.io/n1D7niN.jpg)

## 20. Settings that are actually administration

E-mail transport (**PHP `mail()` or your own SMTP** with host, port, user, password and TLS/SSL), storage and retention, privacy (IP anonymisation, GDPR consent text), maintenance window, CORS allow-list, forced HTTPS, blocked IPs, session control and system health.

![Admin settings: e-mail, storage, privacy and security](https://iili.io/n1D7xfI.jpg)

## 21. The agent panel on a phone

Dashboards, queues and threads all work on a phone with off-canvas navigation — useful when someone has to answer one urgent chat while on the move.

![Agent panel on a mobile screen](https://iili.io/n1D7IUX.jpg)

---

# Part 3 · How you install it

**Requirements:** any shared hosting or VPS with **PHP 8.1+**, the `pdo_sqlite` extension and a writable `data/` folder. Nothing else — no Composer, no Node on the server, no cron required.

1. Upload the `src/php-chat-support/` folder to your domain (or a sub-domain like `chat.yoursite.com`).
2. Open `https://your-domain.com/install.php` and fill the short wizard: brand name, accent colour, your e-mail, admin password.
3. Open **Install & embed**, copy the snippet, paste it before `</body>` on the site you want the widget on. Done.

```html
<script src="https://your-domain.com/widget.js" data-api="https://your-domain.com/api.php" async></script>
```

Prefer to skip the widget? Link straight to `https://your-domain.com/chat.php` — the same chat app, full page.

**Demo logins used in every screenshot**

| Role | E-mail | Password |
| --- | --- | --- |
| Main administrator | `dkkr5558@gmail.com` | `PulseChat@5558` |
| Agent | `aarav@pulsechat.test` | `Demo@1234` |

---

# Part 4 · Security and peace of mind

- CSRF token on every write, and a stale token is refreshed and replayed automatically instead of losing your edit.
- Prepared statements everywhere, output escaping on every screen — XSS and SQL injection are handled at the framework level.
- Login throttling with lockout, database-backed sessions, per-action capability checks, full audit log.
- Rate limits on visitor endpoints, upload size/extension/MIME validation, tokenised attachment downloads.
- Optional IP anonymisation, blocked-IP list, forced HTTPS, maintenance window.
- Panel and chat pages are `noindex`; `.htaccess` hardening ships with the package.

**Proof, not promises:** the package ships with two test suites that drive the real widget and the real panel against a live server — **54/0** visitor checks and **40/0** admin checks, plus a settings round-trip test that saves through the UI and reads the row back out of SQLite.

---

# Part 5 · What you receive

```
src/php-chat-support/
  install.php              one-file installer
  widget.js                the ~15 KB embeddable loader (4.6 KB gzipped, no comments)
  chat.php                 the visitor app (chat + help + tickets)
  api.php + api/           REST endpoints: visitor_* / agent_* / admin_* with CORS
  admin/                   20 panel screens (inbox, tickets, KB, analytics, accounts…)
  lib/                     auth, uploads, mailer, KB, AI, exports, maintenance
  assets/                  Tailwind CSS + subset Font Awesome (visitor bundle is small)
  data/  uploads/          SQLite database and files (created on install)
  docs/features.md         22 annotated feature screenshots
  examples/host-site.html  a demo storefront proving the embed
  README.md                full documentation
```

Also included: a **3-minute walkthrough video**, a **22-page annotated feature tour (PDF)**, and the demo seed script used for the screenshots so you can explore a busy installation immediately.

---

# Part 6 · Recently fixed and improved (v2.2)

| Fix | What changed |
| --- | --- |
| Widget could vanish on some themes | The launcher now mounts on `<html>` and re-attaches itself if a theme or framework re-renders the page — the "disappears after one second" case is gone. |
| Saves that looked like they did nothing | Every save is real AJAX, refreshes a stale security token automatically, and the server reads every row back from SQLite before answering, so you get the true count of changed fields or the real error. |
| Settings not visible until reload | An open chat now re-reads the widget configuration about once a minute and repaints colour, title, label and position live. |
| Hard-coded URLs | The widget, snippets and e-mails use the live request host; a **Public base URL** field pins the canonical URL behind a proxy. |
| Visitor code review | Every script a browser loads ships comment-free, verified equivalent to the original. |

---

## Quick FAQ

**Do I need Linux, Docker, Redis or anything else?** No. PHP 8.1+ with SQLite, on any host.

**Can it run on the same site as WordPress?** Yes — upload it to a sub-domain and paste one script tag. Or use the plain HTML guide.

**Do visitors need an account?** Never. They are remembered on their own device instead.

**Will the database grow forever?** No — retention rules and the cleanup screen prune old chats, visitors and attachments, with a dry run first.

**Can several agents work at once?** Yes. Round-robin or least-busy assignment, departments, internal notes, and a live "who is online" view.

**What about my language?** The whole visitor side is text you control from Chat setup, so nothing is hard-coded.

---

## Get it

Everything you need is in the package: the installer, the widget, the panel, the docs, the video and the screenshots above. Install it in ten minutes, own it forever.

**Questions or a custom setup?** Write to **dkkr5558@gmail.com** — happy to help you get chat running on your site.
