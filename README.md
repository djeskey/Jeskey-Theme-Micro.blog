# Micro Sidebar (Micro.blog + Hugo 0.140+)

Minimal left-sidebar theme for Micro.blog custom themes.

## Important repo layout (for Micro.blog sync)

Use these paths at repo root:

- `layouts/_default/baseof.html`
- `layouts/_default/list.html`
- `layouts/_default/single.html`
- `layouts/index.html`
- `layouts/partials/head.html`
- `layouts/partials/sidebar.html`
- `layouts/partials/post-list.html`
- `static/css/style.css`
- `theme.toml`

Do not nest active templates under `themes/micro-sidebar/...` for Micro.blog custom-theme sync.

## Subtitle and author params in `config.json`

In your site config (`config.json`), add:

```json
{
  "params": {
    "subtitle": "Short line beneath the site title",
    "author": {
      "name": "Your Name",
      "avatar": "https://example.com/avatar.jpg"
    }
  }
}
```

Template usage:

- `site.Params.subtitle`
- `site.Params.author.name`
- `site.Params.author.avatar`

## Hugo deprecation safety

This theme avoids deprecated author access and uses `site.Params.author`.

## CSS customization

Edit variables in `static/css/style.css`:

- `--sidebar-bg`
- `--sidebar-text`
- `--sidebar-muted`
- `--body-bg`
- `--text-color`
- `--link-color`
- `--font-sans`
