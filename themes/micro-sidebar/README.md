# Micro Sidebar (Hugo + Micro.blog)

A minimal, readable sidebar theme built for Micro.blog and Hugo `0.140+`.

## Features

- Left sidebar on desktop, stacked header/sidebar on mobile
- Site title + subtitle/tagline in the sidebar
- Navigation links via Hugo menu
- Clean sans-serif typography
- Single CSS file, no build step, no JS dependency

## Install in a Hugo site

1. Copy this folder into `themes/micro-sidebar`.
2. In your site config, set:

```toml
theme = "micro-sidebar"
```

## Micro.blog compatibility

This theme uses standard Hugo templates and includes optional Micro.blog partial hooks when they exist.

## Customize subtitle/tagline

Set this in your site config (recommended place for future edits):

```toml
[params]
  subtitle = "Short line beneath the site title"
```

## Add navigation links

```toml
[[menu.main]]
  name = "Archive"
  url = "/archive/"
  weight = 10

[[menu.main]]
  name = "About"
  url = "/about/"
  weight = 20
```

## Customize colors and fonts

Edit CSS variables near the top of:

- `static/css/style.css`

Key variables:

- `--sidebar-bg` (sidebar background)
- `--sidebar-text` and `--sidebar-muted`
- `--body-bg`, `--text-color`, `--link-color`
- `--font-sans` (font stack)

That is the main customization surface for non-designers.
