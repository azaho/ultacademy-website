# ultacademy.org

Source code for the website of the **Ukrainian Leadership and Technology Academy (ULTA)** — [ultacademy.org](https://ultacademy.org). A static HTML / CSS / JS site hosted on GitHub Pages.

- **Bilingual:** English (`/en/`) and Ukrainian (`/ua/`), with a language switcher.
- **Self-contained:** images, fonts, CSS and JS are served from this repo. A few interactive embeds (YouTube, the Cognito application form, Telegram, Google Maps) load from their own providers.
- **Course materials:** see [`/files`](./files).

## Local preview

```bash
python3 -m http.server 8099
# then open http://localhost:8099/en/
```

Open it over `http://` (not `file://`) — some embeds (e.g. YouTube) refuse a `file://` origin.

## Pages

`en` / `ua` × `/` (home), `curriculum`, `faq`, `team`, `partners`, `contact-us`, `apply`, `apply/application`, `files`, `projects`.

## Deployment

Pushing to `main` triggers `.github/workflows/deploy.yml`, which publishes the site to GitHub Pages.
