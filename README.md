# Native Font Awesome

A lightweight Drupal module that serves **Font Awesome 6 Free** webfonts (Solid, Regular, Brands) 100% locally from your own web server with zero external CDN dependencies.

## Features

- **100% Self-Hosted:** No requests made to `cdnjs.cloudflare.com` or `use.fontawesome.com`. Fully compliant with GDPR / European privacy regulations.
- **High-Priority Loading:** Configured in `base:` CSS layer with negative weight (`weight: -100`) so that icon stylesheets are prioritized during aggregation.
- **Includes Font Awesome 6.5.1 Free:** Contains `.woff2` files for Solid, Regular, and Brands.

## Requirements

- Drupal 10, 11 or 12.

## Installation

Using Composer:

```bash
composer require javierms/native_fontawesome
drush en native_fontawesome -y
```

## Usage

In your custom theme or module `*.libraries.yml`:

```yaml
my_library:
  dependencies:
    - native_fontawesome/fontawesome
```

In your Twig templates or HTML:

```html
<i class="fa-solid fa-gear"></i>
<i class="fa-brands fa-github"></i>
```

## License

- Module code: GNU General Public License v2.0 or later (GPL-2.0-or-later).
- Font Awesome webfonts: SIL Open Font License 1.1 (Fonticons, Inc.).
- Font Awesome CSS: MIT License (Fonticons, Inc.).
