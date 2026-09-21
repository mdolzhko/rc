# Shell RC Controller

Control Shell/BrandBase promotional RC toy cars from the browser via Web
Bluetooth, instead of the official Shell Racing app.

## Status

Early stage. `index.html` is a working single-file prototype: connect,
protocol auto-detection, keyboard/on-screen controls, battery level, and
a debug log.

## Requirements

- Chrome or Edge (desktop or Android) — Web Bluetooth is not supported on
  iOS (except third-party browsers like Bluefy).
- A secure context (HTTPS or `localhost`).

## Running locally

Web Bluetooth requires a secure context, so opening `index.html` directly
as a `file://` URL will not work — `navigator.bluetooth` needs `https://`
or `http://localhost`.

Until this project has a proper dev server (planned as part of the
Next.js migration below), serve the file locally with:

```
npx serve
```

This downloads and runs the [`serve`](https://www.npmjs.com/package/serve)
package on demand (no global install) and starts a static file server at
`http://localhost:3000`. Open that URL in Chrome or Edge.

## Roadmap

- Migrate to a proper framework (Next.js) and deploy on Vercel for a
  shareable link.
- Protocol adapters for supported car models.
- Support for controlling multiple cars at once on one device.
- Gamepad and touch controls.
