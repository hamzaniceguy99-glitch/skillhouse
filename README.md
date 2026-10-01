# Skillhouse — home brewing coaching

Static marketing site (HTML / CSS / JS, no build step) hosted on GitHub Pages
at `skillhouse.shop`.

> Generated from `C:\Users\souha\coaching-sites-factory` (content file `sites/skillhouse.mjs`).
> To change the content, edit that file and run `node build.mjs skillhouse` — editing the
> HTML here directly would be overwritten on the next build.

## Before you promote this site

| Priority | What | Where |
|---|---|---|
| 🔴 Blocking | Legal page: fill every `[BRACKET]` (legal name, address, state, payment provider). Have a lawyer review it if you can. | `legal.html` |
| 🟠 Important | `contact@skillhouse.shop` doesn't exist yet: set up free email forwarding in Namecheap (*Domain List → Manage → Redirect Email*). | Namecheap |
| 🟠 Important | Contact form: replace `VOTRE_ID_FORMSPREE` with your Formspree id (until then it falls back to `mailto:`). | `contact.html` |
| 🟠 Important | Add a real introduction of the coach (name, background, photo). Never invent credentials. | `about.html` |
| 🟡 Later | Prices ($29 / $75 / $149) and plan contents should match what you actually sell. | `index.html` `#pricing` |
| 🟡 Later | Testimonials: only add real ones, with permission. Fake reviews are illegal (FTC). | — |

## Business description (Stripe, directories…)

```
Coaching in home brewing for adults aged 21 and over, delivered online: one-on-one video sessions and small group sessions covering sanitation and brewing a first batch, fermentation and temperature control, designing and adjusting recipes, and diagnosing off-flavors. Brewers follow an 8 to 12 week program with written review of their brew logs and tasting notes. We sell and ship no alcohol or ingredients, and brewers are responsible for the federal and state limits that apply to home brewing. Services are sold as month-to-month subscriptions from $29 to $149 per month, cancellable at any time. No physical products are sold or shipped. Site: skillhouse.shop
```

## Structure

```
index.html            Home: hero, programs, method, pricing, approach, FAQ
programs.html         The four programs in detail
about.html            How we work, principles
contact.html          Contact form
legal.html            Business info, privacy policy, terms of service
404.html              Error page (absolute paths)
assets/css/style.css  Brand colors at the top, shared styles below
assets/js/main.js     Menu, theme, animations, form
```

## DNS (Namecheap → Advanced DNS)

Delete the parking records, then add:

| Type | Host | Value |
|---|---|---|
| A Record | `@` | `185.199.108.153` |
| A Record | `@` | `185.199.109.153` |
| A Record | `@` | `185.199.110.153` |
| A Record | `@` | `185.199.111.153` |
| CNAME Record | `www` | `hamzaniceguy99-glitch.github.io.` |
