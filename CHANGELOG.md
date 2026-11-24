# Titanium X Repository — Changelog

## 2026-11-24 — Initial publication (Stable channel)
- script.module.titaniumx.artwork 0.1.0 — shared artwork engine
- service.titaniumx.artwork 0.1.0 — cache maintenance service
- script.titaniumx.artwork 0.1.0 — Artwork Downloader Pro (Phase 1 dashboard)
- plugin.video.titaniumx 0.2.0 — dynamic catalog prototype
- repository.titaniumx 0.1.0 — this repository

## 2026-11-24 — Engine 0.2.0 / Downloader Pro 0.2.0 (Phase 2)
- Alternatives API (fanart.tv + TMDb), artwork locks, hash duplicate detection
- TVDb series enrichment bridge, bulk download-missing job (progress + cancel)
- Downloader Pro dashboard: Artwork Manager with alternatives gallery

## 2026-11-24 — Titanium X Wizard 0.1.0
- Update check against the official repository, backup/restore (credential-safe), artwork cache cleaning

## 2026-11-24 — Build Creator Pro 0.1.0
- Build manifest assembly + credential-safe export (core unit-tested), initial UI

## 2026-11-24 — Engine 0.3.0: artwork repositories are live in enrichment
- Enrichment now consults Titanium X Assets + user repo manifests (priority above fanart.tv/TMDb per the registry); verified against the real published Assets manifest (E.T. resolves its animated fanart by IMDb ID)

## 2026-11-24 — Titanium X flagship skin 1.0.0 (Stage 1) + Build Creator Pro 0.1.1
- NEW skin.titaniumx: original flagship skin — 4 home layouts (Cinema/Netflix/Disney/Apple styles), Showcase/Wall/Wide/List views, animated poster + character art + clearlogo + rotating disc support, 4 colour themes, 3 font sets, Titanium X tools dashboard, full dialog set (94 XML files, all validated)
- Build Creator Pro 0.1.1: cancel-safe dialogs + self-diagnosing error display (any future error shows its own cause on screen)

## 2026-11-24 — Skin family: Cinema, Ultra, Elite 1.0.0
- skin.titaniumx.cinema: fullscreen fanart, animated posters, character overlays, large info panels (List/Showcase/Wall)
- skin.titaniumx.ultra: streaming-style home, horizontal widget rows, List/Showcase/Wall/Wide
- skin.titaniumx.elite: rotating discs, 4 colour themes, 3 fontsets, extensive artwork toggles (List/Showcase/Wall/Wide)
- All validated: XML parses, texture references resolve, declared views defined

## 2026-11-24 — The Build update: catalogs, providers, one-click install, first-run setup
- plugin.video.titaniumx 0.3.0: 20 catalog sections (Trending/Popular/New/Upcoming/Top Rated, TV, Genres, Decades, Anime, Documentaries, Kids, Collections) via TMDb discovery + keyless fallbacks; provider page per title (info, trailer, Torus/TMDb Helper playback, watchlist); local watchlist; Universal Search
- NEW script.titaniumx.providers: Universal Provider Manager (install/enable/configure compatible providers)
- NEW script.titaniumx.setup: first-run welcome wizard (layout, performance, artwork, TMDb key, providers); service launches it once
- Wizard 0.2.0: one-click build installer with Lite/Balanced/Ultimate device profiles
- Build Creator Pro 0.2.0: graphical add-on picker (multiselect over installed add-ons)
- Engine 0.4.0: TMDb catalog client + watchlist storage
- All skins 1.0.1: home widgets feed from the live Trending catalogs

## 2026-11-24 — Theme Studio
- NEW script.titaniumx.themestudio: apply the 12 colour themes live, create/save custom themes, import community themes from the Assets repository, export share packs, glass/glow/character/startup toggles, icon packs, Day/Night quick apply
- All skins 1.1.0: named theme colours throughout (any theme x any layout), tintable focus frames with glow toggle, glass menu panels, navigation sounds, Neon icon pack included
- Shared themes live in titanium-x-assets/themes (index.json + 12 XML)

## 2026-11-24 — Kodi 22 Piers editions of all skins (1.2.0, xbmc.gui 5.18.0)
- Kodi picks the highest compatible edition per install: 1.2.0 on Kodi 22, 1.1.0 on Kodi 21

## 2026-11-24 — Kodi 22 audit pass: skin editions 1.2.1 add MyPVRProviders (Piers-only window); audit in docs/KODI22-AUDIT.md

## 2026-11-24 — Dependency pass (verified against the official Kodi 22 repo)
- Wizard 0.3.0: skin helper pack installer + Ultimate profile includes the verified Piers-repo helpers
- Provider Manager 0.2.0: helper add-ons listed; Torus annotated (needs its own repo)
- Verified ABSENT from Kodi 22 repo: script.skin.helper.service, script.module.metadatautils, script.artwork.downloader — Titanium X depends on none of them
