# SaniXperts Signature Studio

A single tool that generates **standardized, Outlook-safe** email signatures for every
employee. It fixes the copyright/consistency problem: previously each signature was a
flat AI-generated image, so the logo differed slightly on every one. Now the logo is **one
locked, hosted file** and everything else is real HTML text.

## Files
- `index.html` ........... the builder (host this — it's the tool employees use)
- `example-01-classic.htm` ... sample output, Classic layout
- `example-02-compact.htm` ... sample output, Compact layout (great for replies)
- `example-03-modern.htm` .... sample output, Modern Stacked layout
- `assets/sanixperts-symbol-curved-wordmark-white.png` ... approved canonical logo

## What's locked vs editable
- **Locked for everyone:** logo, "SaniXperts Inc.", website, office phone (289-674-7265),
  office address, tagline and value chips.
- **Per employee:** name, job title, mobile, email.

## The logo
Every generated signature uses the approved curved-wordmark asset from this repository:
`https://sanixpertsim2-sanitation.github.io/Signature/assets/sanixperts-symbol-curved-wordmark-white.png`
The symbol and curved SANIXPERTS wordmark therefore stay consistent for every employee.

## Hosting on GitHub Pages
1. Keep `index.html` and the `assets` folder together in the repo.
2. Employees open the page, fill in their fields, pick a layout and size, then click **Copy to Outlook**.
3. Paste into Outlook: `File ▸ Options ▸ Mail ▸ Signatures ▸ New ▸ paste ▸ Save`.

## Outlook compatibility
Signatures use table-based layout, inline styles, Arial/Helvetica, and a hosted logo —
the combination Outlook (desktop, web, and New Outlook) renders reliably.
