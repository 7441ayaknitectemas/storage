# Changelog

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
