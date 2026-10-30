# TnBoost

International agency website in Arabic, English and French. Includes the current responsive layout, compact mobile menu, six project concepts and WhatsApp inquiry flow.

## Cloudflare Pages

Connect `tnboostagency-hue/tnboost` in Cloudflare → Workers & Pages → Create application → Pages → Import an existing Git repository.

| Setting | Value |
| --- | --- |
| Framework preset | None |
| Production branch | main |
| Root directory | Repository root |
| Build command | node --check dist/tnboost.js |
| Build output directory | dist |

No environment variables, paid APIs, build dependencies or server-side runtime are required for the website. Cloudflare can redeploy automatically after GitHub pushes once the repository integration is authorized.

## Files

- `dist/index.html`: page structure and English source copy.
- `dist/tnboost.js`: translations, menu behavior, service selections and inquiry form.
- `dist/style.css`: visual design and liquid glass treatment.
- `dist/responsive.css`: responsive layout and mobile menu.

The inquiry form opens WhatsApp with a draft. It does not submit messages or reserve calendar availability automatically. Project previews are illustrative concepts, not client work.

## Local check

Run `node --check dist/tnboost.js`. Serve `dist` using any static HTTP server to preview.

Official deployment guide: https://developers.cloudflare.com/pages/framework-guides/deploy-anything/
