# Shell RC Controller

Control Shell/BrandBase promotional RC toy cars from the browser via Web
Bluetooth, instead of the official Shell Racing app.

## Status

Early stage. The repository currently contains a placeholder landing page
(`index.html`). Working prototypes exist locally but are not yet part of
this repository.

## Requirements

- Chrome or Edge (desktop or Android) — Web Bluetooth is not supported on
  iOS (except third-party browsers like Bluefy).
- A secure context (HTTPS or `localhost`).

## Running locally

Open `index.html` in a supported browser.

## Roadmap

- Migrate to a proper framework (Next.js) and deploy on Vercel for a
  shareable link.
- Protocol adapters for supported car models.
- Support for controlling multiple cars at once on one device.
- Gamepad and touch controls.
