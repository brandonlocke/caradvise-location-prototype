# CarAdvise map location prototype

Interactive, client-only review prototype based on the supplied Sep 21 CSS export, Pao's screenshots, and Figma file `1AR1kPwI3zA7BHbuWEzrqS`, node `11703:98791`.

The original Figma render provides the map and icon sprite. Layout, inputs, results, editors and scenario controls are live HTML/CSS/JavaScript. The supplied design tokens include Inter, #DB502D, 12px input corners and pill-shaped buttons. Vehicle switching is excluded.

All shop records, prices and device-location outcomes are fixtures. The map is a fixed design reference, not a geographic or geocoding service. Changes are in memory only. No external bookings, account writes or permission requests occur.

## Review flows

- Choose any of the four starting scenarios.
- Select the visible area to open search with Location focused.
- Search shop names within the chosen area; clearing a name preserves the area.
- Edit the default from the map or search screen. Saving does not change the current area unless the user selects that option.
- A first manually searched code establishes a default, with explanatory copy. Later manual searches only update the default when explicitly selected.
- Start a fresh search to exercise device-first, saved-default fallback behavior.
- Choose Canada for postal validation, no prices and walk-in copy.
- Permission denial and unavailable-location fixtures preserve the previous search.

The latest screenshot explicitly reintroduces a default-location row with Edit. The prototype keeps that row and separately labels the active search area in the search bar so the two values have distinct purposes.
