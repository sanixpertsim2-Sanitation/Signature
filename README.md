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
- `sanixperts-logo.png` ...... crisp 480px logo (optional — see "Sharper logo" below)

## What's locked vs editable
- **Locked for everyone:** logo, "SaniXperts Inc.", website, office phone (289-674-7265),
  office address, tagline and value chips.
- **Per employee:** name, job title, mobile, email.

## The logo
The signature points at the company's own hosted logo:
`https://sanixperts.ca/wp-content/uploads/2020/05/logo.png`
Because every signature references that one URL, no one can ever end up with a different
version — this is the core of the fix.

### Sharper logo (optional)
That official file is 166px. For extra crispness on high-DPI screens, host the included
`sanixperts-logo.png` (480px) on your GitHub Pages repo and change one line near the top of
`index.html`:
```
var LOGO_HOSTED = "https://sanixpertsim2-sanitation.github.io/Signature/sanixperts-logo.png";
```

## Hosting on GitHub Pages
1. Put `index.html` (and optionally `sanixperts-logo.png`) in the repo.
2. Employees open the page, fill in their 4 fields, pick a layout, click **Copy signature**.
3. Paste into Outlook: `File ▸ Options ▸ Mail ▸ Signatures ▸ New ▸ paste ▸ Save`.

## Outlook compatibility
Signatures use table-based layout, inline styles, Arial/Helvetica, and a hosted logo —
the combination Outlook (desktop, web, and New Outlook) renders reliably.
