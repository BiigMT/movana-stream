# MOVANA — Movies, Series & Live Streaming

MOVANA is a mobile-first streaming platform project by MT.

## Live site
- Production: https://movana-stream.vercel.app
- Main app: `src/index.html`
- Root entry: `index.html` redirects to the app.

## Current MVP
- Public catalog browsing and search (movies / series / genre)
- Supabase email/password sign-up and sign-in
- Published title playback with signed private-media URLs
- Personal watchlist
- Creator video/poster uploads for review
- Admin submission review and title publishing
- Live channel requests, listings, and admin playback URL setup
- Responsive mobile navigation and full-screen video player
- Android WebView app scaffold and GitHub Actions APK workflow

## Backend
Supabase project `bfcppzretyjthodjbnkh` contains the MOVANA tables, RLS policies, and media buckets. The frontend uses the project's publishable API key only; no service-role key is included in the browser.

## Production requirements still external
- Payment provider merchant account + secret credentials + webhook configuration for paid subscriptions and episode purchases
- Live broadcast ingest provider (e.g. managed HLS/live streaming) for creator-generated live streams; current admin supports an existing HLS playback URL
- Licensed/cleared movies, series, posters, and other catalog assets
- Production auth email delivery configuration and final user testing

The site does not claim to process payments until checkout and webhook verification are connected.
