# Changelog

## 2026-09-04 - Script 1 progress UI

### Added
- Script 1 now opens a ReGui progress window ("Script 1") with separate Configs and Paints bars
- Burst-send remotes with response-counted progress (bars advance as server replies return, not on send)
- Part-count display (configs /3 for X/Y/Z, paints /2 for color+material)
- Close button + auto-close 3s after completion

### Changed
- Removed overflowing outer bar label; percentage shows inside the yellow bar only

Source: `C:\Users\samet\OneDrive\Desktop\testing\babft2\babftindex.html`

## 2026-08-30 - BABFT Index Update

### Added
- InstancedMesh batching for large builds (>2500 parts) with shared unit geometry
- Adaptive pixel ratio and shadow handling for large builds
- Bulk selection highlight limit (400) to avoid O(N) outline creation
- Selection overlay group and shared edge geometry

### Fixed
- `calculateModelOrigin` now filters invalid positions (>1e6) and outlier median filtering (P95 threshold)
- Fallback origin calculation excludes insane values (>1e12)
- Improved handling of placeholder/void positions (e.g. -3e38 in .Build)

### Changed
- Renderer init with high-performance powerPreference, capped DPR 1.5
- Updated `babftindex.html` (153970 -> 177922 bytes, +666/-146 lines)

Source: `C:\Users\samet\OneDrive\Desktop\testing\babftindex.html`
