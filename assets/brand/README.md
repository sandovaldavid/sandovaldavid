# GitHub profile brand assets

These assets implement the approved personal-brand identity for David Sandoval's GitHub profile README.

## Source and ownership

| Responsibility | Source |
|---|---|
| Identity, semantic colors, typography and Logo v2 | Figma — `Identity System` |
| Production preview and profile-banner contract | Figma — `Search & Social Preview System` |
| Channel implementation and rendered README | `sandovaldavid/sandovaldavid` |
| Avatar | Managed manually by David in GitHub profile settings |

Identity System reference:

- File key: `sHPP8DGCfZ370Oc2oKGNPH`
- Component set: `Application / GitHub Profile Header`
- Component set node: `406:204`
- Desktop Light variant node: `406:138`
- Desktop Dark variant node: `406:171`
- Mobile Light variant node: `408:197`
- Mobile Dark variant node: `408:219`
- Logo v2 component: `Logo / Isotype`
- Logo v2 component set node: `479:50`
- Canonical standard geometry node: `500:189`

The Identity System component is the implementation reference for this channel. Search & Social Preview System remains the owner of reusable production-preview masters and export contracts.

The profile assets were synchronized with the current Logo v2 geometry on **2026-09-03**. The historical literal `</>` mark is no longer valid for new GitHub profile exports.

## Files

| File | Format | Mode | Dimensions | Use |
|---|---|---|---:|---|
| `github-profile-header-light.svg` | Desktop | Light | 1600 × 400 | Default light header on wide screens |
| `github-profile-header-dark.svg` | Desktop | Dark | 1600 × 400 | Dark header on wide screens |
| `github-profile-header-mobile-light.svg` | Mobile | Light | 800 × 400 | Readable light header on narrow screens |
| `github-profile-header-mobile-dark.svg` | Mobile | Dark | 800 × 400 | Readable dark header on narrow screens |

GitHub renders the SVG assets directly. Keep the repository copies small and self-contained: no external image, font, badge, counter or rendering-service dependency is required for the header to appear.

## Responsive behavior

The root README uses the Mobile variants when the viewport is no wider than `600px`. Mobile assets shorten the supporting copy and use a `2:1` ratio so David's name and role remain readable instead of scaling the `4:1` desktop artwork to an unusably small size.

Source ordering is specific-first:

1. Mobile Dark.
2. Mobile Light.
3. Desktop Dark.
4. Desktop Light.
5. Desktop Light fallback image.

## Usage rules

- Keep David's name and professional role primary.
- Keep Logo v2 as a supporting signature, never the main subject.
- Do not redraw, reinterpret, recolor, rotate, crop or distort Logo v2 geometry in consumer files.
- Do not restore the historical literal `</>` mark.
- Do not add technology-logo walls, counters, stats, animations, glow or profile-decoration effects.
- Keep Light and Dark assets synchronized within each format.
- Keep Desktop and Mobile copy semantically equivalent; reduce detail rather than changing the positioning.
- Do not add the portrait to these files. The GitHub avatar is a separate people-facing identity surface and is updated manually by David.
- Preserve the `1600 × 400` Desktop and `800 × 400` Mobile master ratios.

## README integration

The root README selects the appropriate format and color mode with a `<picture>` element. The Desktop Light asset remains the final fallback.

The README should stay human-first and evidence-bounded:

- lead with David as a person and Software Engineer;
- describe professional experience with sanitized, defensible language;
- prioritize public projects that a reviewer can inspect directly;
- keep private-project caveats concise;
- avoid internal governance language in visitor-facing copy.
