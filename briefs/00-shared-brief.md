# Shared design brief — AVD mobile-first sample pages

Goal: three standalone sample web pages, one per local business, used as a text-message pitch.
The owner opens a link on their phone and sees their own business presented better than it is now.

## Hard requirements

- ONE file per business: `index.html`, fully self-contained. Inline `<style>`, no external CSS/JS/frameworks/fonts/images. Load fast on a phone.
- Mobile-first. Design for 390x844 first; must also look right at 1440 wide (max-width container, no stretched layout).
- Real facts only. Use only the facts in the business brief. Never invent prices, review counts, awards, staff counts, licenses, or guarantees. No lorem ipsum.
- Big tap-to-call: `<a href="tel:...">` as the primary action, 48px+ tap target, plus a sticky bottom bar on mobile with Call + Text (`sms:` link).
- Page background soft off-white `#f1f5fa`, white cards, one accent color per business, generous spacing. Professional and calm, not a SaaS landing page, no gradient soup, no emoji, no fake dashboard graphics, no AI-slop: no "unlock", "elevate", "revolutionize", no purple-on-white startup look.
- Icons: inline SVG only, 1.5px stroke, currentColor.
- Sections (in order, compact): sticky header with business name + call button; hero (plain-language promise + city + call button + 3 trust pills); services or packages (real ones, real prices where given); service area strip; short honest trust/about block; simple estimate form (name, phone, what needs doing) with a note that it goes to the owner's email — form must NOT post anywhere, `action="#"` plus a JS-free-friendly note; footer with business phone, city, and a small line: `Sample design — not the live site.`
- Accessibility: semantic landmarks, real heading order, labels on inputs, focus-visible styles, `prefers-reduced-motion` respected.
- No tracking, no cookies, no external requests at all.
- Total file under 60 KB.

## Accent colors

- tyrees: charcoal `#1c1f24` + warm copper accent `#b4682b`
- brightleaf: deep green `#14532d` + soft leaf accent `#2f7d4f`
- handyman: navy `#0f2a4a` + safety amber `#e08b1a`
