# Darbadar — Discover Pakistan

**Live app:** https://za1dgondal19-cmyk.github.io/Darbadar/

Darbadar is a mobile-first, installable travel companion prototype for exploring destinations across Pakistan.

## What works in this version

- Six destination guides: Hunza Valley, Fairy Meadows, Swat Valley, Lahore, Skardu and Mohenjo-daro.
- Destination search and region filters.
- Save destinations and trip plans on the current device.
- Destination information, suggested activities, food ideas, stay-search shortcuts and local travel guidance.
- OpenStreetMap destination maps and Google Maps directions/search links.
- Trip planner with starting city, duration, pace, travel date, group size and an editable budget breakdown.
- Indicative trip-planning budget ranges. These are not live quotations or guaranteed prices.
- Packing and pre-departure safety checklists.
- Links to official PMD weather, NDMA advisories and NHMP travel advisories.
- English/Urdu interface toggle for the main navigation and selected interface labels.
- Installable Progressive Web App shell and basic offline app-shell caching.

## Important limitations — read before relying on it

This is a frontend prototype, not a fully connected commercial booking platform.

- Saved places, itineraries, expense notes, checklists and road submissions are stored only in the browser/device using local storage. They do not sync to another phone and are not shared with other travellers.
- Road submissions are local notes, not a live feed, official report or verified community update.
- Destination content is editorial starter guidance. Conditions, opening hours, transport, prices and access can change; confirm them independently.
- Hotel, restaurant, guide and attraction buttons open external search results. Darbadar does not verify listings, display live inventory, accept bookings or process payments.
- Maps and route links are external. They do not guarantee road safety, route availability or route optimisation.
- Weather and road links open official external services. Live alerts are not embedded in the app.
- Urdu translation currently covers selected interface labels; destination descriptions and much of the detailed guide content remain in English.
- The Android project is a lightweight WebView wrapper around the live PWA. It is built as a debug-signed APK for testing; it is not yet a production-signed Play Store release.
- The app does not currently have accounts, a hosted database, admin moderation or push notifications.
- Offline mode caches the app shell; external photos, maps and search links still need an internet connection.

## Install on Android

1. Open the live app in Google Chrome.
2. Open Chrome's three-dot menu.
3. Choose Install app or Add to Home screen (the wording can vary).
4. Confirm installation.

## Android APK

A GitHub Actions workflow builds an installable debug APK when Android project files change or when manually triggered. The workflow publishes the APK under the repository's Releases and also stores it as a build artifact. The APK loads the live HTTPS app, so most content and external services require an internet connection. Debug signing is suitable for testing; a stable private release keystore and signing setup are required before public Play Store distribution.

## Free deployment

The project is hosted with GitHub Pages from the main branch, repository root. New commits are published by the repository's GitHub Pages workflow.

## Next production requirements

To turn this prototype into a public travel platform, the next engineering phase needs a secure backend/database, authentication, moderation tools, verified partner data, a live road/weather data strategy, privacy and security review, and device testing. Booking/payment integrations and a native APK would be separate phases.
