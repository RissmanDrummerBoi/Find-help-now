# Find Help Now

A free, fast and easy-to-use support directory that helps people in the Eastern Cape, South Africa find the right organisation to talk to when they or someone they know is experiencing abuse, violence or a mental health crisis.

## Description

Find Help Now is a single-page website that brings emergency and support contacts together in one place. Each organisation has its own card showing who they are, what help they offer, when they are available (24/7 or weekdays) and a one-tap call button. Visitors can search by keyword (for example "rape", "child", "mental" or "GBV") or filter by type of help to get to the right contact quickly.

The directory covers:

- Rape and sexual assault support (Thuthuzela Care Centre)
- Gender-based violence (GBV) social workers and the national GBV Command Centre
- Domestic and sexual violence support (TEARS)
- Child protection (Childline)
- Free legal advice and human rights support
- Mental health services and referrals (SADAG)
- SAPS emergency numbers for reporting violence

## Why I built this

I built this website after realising that not everyone knows who to talk to when something goes wrong. Many people go through abuse or violence in silence, not because help doesn't exist, but because they don't know where to find it or who to call. I wanted to put those contacts in one simple place that anyone can open on their phone and use immediately.

## Features

- One-tap calling from any phone (`tel:` links, including USSD codes)
- Live search with hidden keywords, so "suicide" or "kids" finds the right card
- Filter chips: All, Open 24/7, GBV & abuse, Children, Mental health, Legal
- Availability badges on every card
- **Quick Exit** button (also triggered with the `Esc` key) that leaves the page immediately, for users who need to hide that they were here
- Responsive layout that works on small phones
- Accessible: labelled search, screen reader announcements for results, visible keyboard focus, reduced-motion support
- No frameworks, no dependencies, no tracking: one HTML file

## Tech stack

- HTML5
- CSS3 (custom properties, grid, flexbox)
- Vanilla JavaScript

## Getting started

1. Download or clone this repository.
2. Open `find-help-now.html` in any browser.

No build step or server is needed. To host it, upload the file to any static host (GitHub Pages, Netlify, etc.).

## Adding or updating an organisation

Copy an existing `<article class="card">` block and edit it:

```html
<article class="card" data-tags="247 gbv keywords people might search">
  <h3>Organisation name</h3>
  <span class="hours">Open 24/7</span>
  <p>What they help with.</p>
  <div class="phone-numbers">
    <a href="tel:0123456789" class="phone-btn">📞 012 345 6789</a>
  </div>
</article>
```

- Use `hours limited` as the badge class for non-24/7 services.
- `data-tags` controls search and filters. Use `247`, `gbv`, `child`, `mental` or `legal` to place the card under a filter, plus any extra keywords.
- For USSD codes, encode `#` as `%23` in the link (for example `tel:*134*7545%23`).

## Important notice

Please verify all phone numbers and operating hours with each organisation before relying on them, as services can change. **If you are in immediate danger, call SAPS on 10111.**

## Author

Built by **Rissmantech PTY LTD**.

Contact: [rkellysiweya77@gmail.com](mailto:rkellysiweya77@gmail.com)

## Contributing

Know an organisation that should be listed, or spotted an outdated number? Open an issue or pull request.
