# NT Design Assets

Brand assets organized for stable GitHub + jsDelivr CDN usage.

## Folder layout
- `logos/marks/`
- `logos/wordmarks/`
- `banners/`
- `social/`
- `backgrounds/`
- `maps/`

## CDN base URL
Use this format:

`https://cdn.jsdelivr.net/gh/neutral-trade/design-assets@<ref>/<path>`

- `<ref>` can be `main` (quick updates) or a tag like `v1.0.0` (recommended for production).

## Example asset URLs
- `https://cdn.jsdelivr.net/gh/neutral-trade/design-assets@main/logos/marks/nt-logo-mark-gradient-v1.0.0.svg`
- `https://cdn.jsdelivr.net/gh/neutral-trade/design-assets@main/logos/marks/nt-logo-mark-gradient-on-black-v1.0.0.png`
- `https://cdn.jsdelivr.net/gh/neutral-trade/design-assets@main/social/nt-social-biweekly-report-01-v1.0.0.png`

## HTML embed snippets

### Preferred logo setup (SVG + PNG fallback)
```html
<picture>
  <source
    srcset="https://cdn.jsdelivr.net/gh/neutral-trade/design-assets@v1.0.0/logos/marks/nt-logo-mark-gradient-v1.0.0.svg"
    type="image/svg+xml"
  />
  <img
    src="https://cdn.jsdelivr.net/gh/neutral-trade/design-assets@v1.0.0/logos/marks/nt-logo-mark-gradient-on-black-v1.0.0.png"
    alt="NT Logo"
    width="160"
    height="160"
    loading="lazy"
    decoding="async"
  />
</picture>
```

### Wordmark image
```html
<img
  src="https://cdn.jsdelivr.net/gh/neutral-trade/design-assets@v1.0.0/logos/wordmarks/nt-wordmark-neutral-font1-white-v1.0.0.svg"
  alt="Neutral Wordmark"
  width="360"
  height="98"
/>
```

## Versioning workflow
1. Add or update assets in this repository.
2. Commit changes.
3. Create a release tag (for example `v1.0.1`).
4. Update external URLs from `@v1.0.0` to the new tag only when you want to publish.

## Migration reference
See `MAPPING.md` for the full old-name to new-path mapping list.
