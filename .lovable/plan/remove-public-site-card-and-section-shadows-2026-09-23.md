# Remove public-site card and section shadows

## Scope
- Remove the global teal glow and all other box shadows applied to public-site cards and section containers.
- Remove local shadow utilities from public marketing cards, showcase frames, pricing panels, testimonials, contact/about panels, and tutorial screenshot containers.
- Remove card shadows from clinic-hosted public pages while leaving functional floating controls and buttons unchanged.
- Preserve borders, backgrounds, spacing, and interactions so the hierarchy remains clear without artificial depth.

## Technical details
- Update the scoped public-site styles in `src/index.css` so shared card, glass, and hairline surfaces use `box-shadow: none`.
- Remove `shadow-*`, `hover:shadow-*`, and colored shadow utilities from card/section markup under `src/site` and relevant card markup in `src/pages/PublicClinicSite.tsx`.
- Verify the Industries page at mobile and desktop widths, then spot-check other public pages for remaining card or section shadows.
