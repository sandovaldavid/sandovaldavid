# GitHub profile brand assets

These assets implement the approved personal-brand identity for David Sandoval's GitHub profile README.

## Source and ownership

| Responsibility | Source |
|---|---|
| Identity, semantic colors, typography and supporting isotype | Figma — `Identity System` |
| Production preview and profile-banner contract | Figma — `Search & Social Preview System` |
| Channel implementation and rendered README | `sandovaldavid/sandovaldavid` |
| Avatar | Managed manually by David in GitHub profile settings |

Identity System reference:

- File key: `sHPP8DGCfZ370Oc2oKGNPH`
- Component set: `Application / GitHub Profile Header`
- Component set node: `406:204`
- Light variant node: `406:138`
- Dark variant node: `406:171`
- Documentation node: `406:205`

The Identity System component is an implementation reference. Search & Social Preview System remains the owner of reusable production-preview masters and export contracts.

## Files

| File | Mode | Dimensions | Use |
|---|---|---:|---|
| `github-profile-header-light.svg` | Light | 1600 × 400 | GitHub README when the viewer prefers a light color scheme |
| `github-profile-header-dark.svg` | Dark | 1600 × 400 | GitHub README when the viewer prefers a dark color scheme |

The repository currently consumes SVG because GitHub can render the vectors directly. The approved export contract also permits a PNG derivative when a destination requires raster output.

## Usage rules

- Keep David's name and professional role primary.
- Keep the isotype as a supporting signature.
- Do not recolor, rotate, crop, distort or reconstruct the isotype.
- Do not add technology-logo walls, counters, stats, animations, glow or profile-decoration effects.
- Keep Light and Dark assets synchronized with the same copy and composition.
- Do not add the portrait to these files. The GitHub avatar is a separate people-facing identity surface and is updated manually by David.
- Preserve the `1600 × 400` master ratio.

## README integration

The root README selects the correct asset with a `<picture>` element and `prefers-color-scheme`. The light asset remains the fallback.
