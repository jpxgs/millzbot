# 2026-11-01
- Added FIELDNOTES — Signal Video to Selected work. Live at https://signal-video.vercel.app.

# Changelog

All notable changes to Millzbot are listed here, newest first. Dates follow the git history. Entries use conventional commit wording. The 2026-10-29 lines describe what shipped together in the initial commit; they were not separate commits.

## 2026-10-31

- feat: keep a playing video in a floating mini player. Scrolling a playing YouTube embed out of view, or opening another section, docks that same player in the corner. Return goes back to the entry, Close stops it, and the player follows night mode without covering the nav.
- feat: default embedded YouTube videos to 50% volume. The IFrame API sets the volume when the player is ready and again when playback starts.
- feat: add a Work With Me link on the home About card. The line matches the signal-red mono link in the “Have something in mind?” box and opens `/about/#offers`.
- feat: add an optional night mode. The header control follows `prefers-color-scheme` until a choice is saved, applies before first paint, and stays on the paper, ink, and signal-red palette.
- fix: pause other YouTube embeds when one starts. Leaving a section also stops a hidden player so two videos cannot play at once. A docked mini player is the exception until another video starts.
- style: redesign the home About Me card. A red rail, a clearer “View About Me” action, and a hover state make the closer easier to click. It still links to `/about/`.

## 2026-10-29

- feat: publish Millzbot as a single dependency-free file with client-side routing.
- feat: add the Mind, Body, and Soul notebooks, with one YouTube embed on each entry.
- feat: add the About page, including contact, selected work, experience, offers, and the Creations gallery.
- feat: set the editorial type system to IBM Plex Mono and Inter on warm paper `#F4F1EA` with signal red `#FC3D21`.
- feat: add per-route titles and descriptions, Open Graph and Twitter cards, `sitemap.xml`, and `robots.txt`.
- chore: mirror the site in `404.html` so deep links resolve on static hosts.
