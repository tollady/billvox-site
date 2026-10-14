# Billvox Website

Marketing/registration site for Billvox, the AI-powered invoicing and quoting tool for Australian sole trader tradespeople.

## Hosting

- Cloudflare Pages. `main` branch deploys to billvox.com.au. Other branches get their own Cloudflare preview URLs.
- Clean URLs (`/register`, `/user-guide` instead of `.html`) only resolve on Cloudflare — they do not work when serving the files locally with a plain static server.

## Workflow

One branch per change, reviewed on its Cloudflare preview URL, then merged to `main`.

## Project Structure

- `index.html` — marketing homepage
- `register.html` — sign-up page
- `user-guide.html` — WhatsApp command/usage guide for registered tradies
- `styles.css` — shared styles

## Content Rules

- Only claim features that actually exist in the app. No Xero sync, SMS, card payments, deposits, or receipt scanning yet — none of these are built.
- No unsourced stats, testimonials, or user counts.
- Pricing message is "Free while in beta."
- Australian/British spelling throughout (e.g. "organisation", "colour").
- Mobile-first design.

## Register Page

Leads with WhatsApp sign-up: a `wa.me` link with "Hi Billvox" pre-filled as the message text, plus a QR code shown on desktop. The traditional form is tucked behind a "Prefer to fill in a form?" expandable section — WhatsApp is the primary path, the form is the fallback.

## Footer

Shows ABN 32 613 603 259 on every page.

## Planned Next

- Design refresh: a stepped walkthrough, an animated chat mockup, and an "the old way" comparison section.
- A 20-30 second demo video to fill the placeholder currently sitting under the hero mockup on the homepage (`index.html`, marked with an HTML comment — replace `poster.jpg` and `demo.mp4` when assets are ready).
