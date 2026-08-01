# HANDICAPP Flutter Web Camera MVP

A browser-first Flutter Web proof of concept for HANDICAPP.

## Working flow

- Opens the device camera in the browser.
- Prefers the rear camera on mobile devices.
- Allows live capture only; there is no gallery upload control.
- Shows the captured image for review.
- Supports Retake and Use Photo actions.
- Includes a PWA manifest for later installability.

## Run

```bash
flutter pub get
flutter run -d chrome
```

## Build

```bash
flutter build web --release
```

Camera access requires HTTPS after deployment. Localhost is allowed during development.

## MVP boundary

This first build intentionally excludes Supabase upload, GPS, hashing, OCR, authentication, and the municipal dashboard. The next slice should add the three-photo incident sequence, geolocation, SHA-256 evidence hashing, and Supabase storage.
