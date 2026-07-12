# Export Cashback Recovery — Full Workflow & Roadmap

> **One line:** Indian exporters' government cashback (RoDTEP / IGST refund / duty drawback)
> gets stuck due to technical errors. We build free tools + guides that these frustrated
> exporters search for on Google → show them the fix → for those with large stuck amounts,
> we help recover the money and take a **10–15% commission**.

Demand is certified (government/court proof): CAG audit + CBIC 72-hour rule (Instruction
05/2026), DGFT cut RoDTEP by 50% then restored it (Notification 66/2025-26), Madras HC
ruling on 7-Jul-2026, CBIC re-credit circular 3-Jul-2026. **The problem is live this week.**

---

## 1. What we are building (The Asset)

Three small things:

| # | Component | Purpose | Tech |
|---|-----------|---------|------|
| A | **Fix-guide pages** | One clear "how to fix" page per error (SEO) | Static site (Bootstrap) |
| B | **Cashback Checker** | Exporter fills 3–4 fields → "you may have ₹X stuck" | JS form + logic |
| C | **Lead form** | "We'll help recover it" → captures name/phone/amount | WhatsApp link |

That's it. No login system, no payment gateway for now. Just static pages + a form.

---

## 2. How the money comes in (Earning Model)

```
Google search ("how to fix SB005 error")
   ↓
Lands on our site  → reads the free fix guide (builds trust)
   ↓
"Check your stuck amount" → runs the Checker → "approx ₹__ stuck"
   ↓
Small amount → fixes it himself (using our guide) — no cost, but SEO/trust grows
Large amount → fills the "we'll help recover it" form
   ↓
We help with recovery → we take 10–15% of the amount actually recovered
```

**Reality (honest):**
- Actual filing happens on the government portal (ICEGATE) using the exporter's own
  login/DSC — a bot alone cannot file. We **diagnose + guide + follow up**, together with
  the exporter or their CA.
- Do the first case **free** (for proof) → "I recovered ₹__ for them" = your marketing.
- One recovered case can be ₹50k–5L → 10% = ₹5k–50k per case. Low volume, good ticket size.

---

## 3. Target search terms (P1 content = these 6)

Priority order (top one = most painful + most searched):

1. **`SB005 error fix`** — IGST refund stuck (GST–Customs data mismatch) ← START HERE
2. `RoDTEP scroll / scrip not generating` — amount shows on ICEGATE but won't convert to cash
3. `e-BRC pending / not showing DGFT` — bank hasn't confirmed the foreign payment
4. `RoDTEP supplementary claim` — forgot the declaration on the shipping bill, now what
5. `PFMS / bank account validation error` — account not linked to the government system
6. `IGST refund denied higher duty drawback` — the Madras HC 2026 case (trending now)

Each term = one page. Same structure on every page:
`What the error is → why it happens → step-by-step fix → "confused? we help" CTA`

---

## 4. Full Workflow (phases + checklist)

### Phase 0 — Setup (1 day)
- [x] Folder + repo ready (`export-cashback/`)
- [ ] Pick a domain (e.g. exportcashback.in) — or start on a free subdomain
- [ ] Reuse the base stack that already works

### Phase 1 — Content asset (3–5 days)
- [x] `SB005 error fix` page — written (flagship)
- [ ] The other 5 error pages
- [ ] Simple, clean English + Hindi mix (audience = Indian exporters / CAs)
- [ ] Basic SEO: title, meta, H1 = exact search phrase

### Phase 2 — Checker tool (2–3 days)
- [x] Form: product type, export value (FOB), scheme, "declared? Y/N"
- [x] Logic: simple rules → "you may have ₹X stuck, reason: ___"
- [x] Result → lead form CTA (WhatsApp)

### Phase 3 — Lead capture (1 day)
- [x] Form → WhatsApp (free)
- [ ] Add your real WhatsApp number in `index.html`

### Phase 4 — Live + traffic (ongoing)
- [ ] Deploy (GitHub Pages — free)
- [ ] Submit to Google Search Console
- [ ] Talk to 2–3 real exporters/CAs (YouTube comments, LinkedIn, IndiaMART sellers)
- [ ] Recover the first case FREE → build a testimonial/proof

### Phase 5 — Monetize
- [ ] Recovery service page: "10–15% success fee, no recovery = no fee"
- [ ] Collect proof of every closed case (for marketing)

---

## 5. Rules (system, not luck)

1. **Perfect one page, then the next** — make SB005 the flagship; don't build 6 half-pages.
2. **Free-first** — recover the first case without charging; that proof is what sells.
3. **No-win-no-fee** — this removes the exporter's objection entirely.
4. **Spend time only on large amounts** — let small ones self-fix via the guide; save your time.
5. **Check one metric weekly** — visitors, checker runs, form submissions.

---

## 6. First task (just this)

> Write the `SB005 error fix` page — what the error is, why it happens, step-by-step fix.
> Just one page. Everything else after that.

---

*Status: demand validated, tech built (index + checker + SB005 guide). Next = add WhatsApp
number, deploy to GitHub Pages, then the remaining error pages.*
