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
