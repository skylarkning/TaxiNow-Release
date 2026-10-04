# TaxiNow Pro V2.0: from airport taxiing to a clearer view of the whole flight

Released October 3, 2026 · Build 207

TaxiNow is now **TaxiNow Pro**. V2.0 brings airport surface maps, route exploration and a vertical situation profile into one workspace. Import a plan before departure, explore it on the globe, use traffic, weather and terrain overlays in flight, then return to the airport map after landing. The existing taxi tools remain, with a broader view of the journey around them.

## A new route workspace

The application now starts on the globe route view. Switch between 2D and 3D, zoom out to see the whole journey or inspect an individual leg, and use the compass at the top left to restore north-up orientation. Taxi remains a separate view in the left rail, while Profile has its own entry and does not cover the map at startup.

Two header rows have become one, with Flight and Route Info on the right. The airport name sits beside the flight number, and the airport selector in the left rail shows the current ICAO code. Source links, credits and status information share a compact footer, leaving more room for the map.

## Start your next flight with SimBrief

Import a SimBrief plan to see its route, waypoints, aircraft type and planned altitude in the same workspace. The Flight panel can fit the complete route to the map; Route Info provides waypoint coordinates. Both panels now share the same geometry, visual treatment and opening transition. Clear plan sits beside Import, and the SimBrief username is saved automatically in the current browser.

TaxiNow Pro attempts to download the departure and arrival airport maps from the plan and switches to the destination taxi map after touchdown. Availability still depends on network connectivity and airport data. Maps & storage provides download status and manual controls when a map is unavailable.

## See the route from the side

The new full-screen vertical profile plots route distance against altitude. Terrain and the planned vertical path appear together, making climb, cruise and descent easier to understand. Altitude constraints supplied by the imported plan receive their own markers. When the plan lacks vertical data, an estimated path is labelled as an estimate rather than presented as a published restriction.

With valid simulator telemetry, the profile shows the aircraft's position along the route, altitude above mean sea level and available height above ground. It also presents terrain clearance, the next altitude constraint and distance to destination. Stale telemetry clears the live aircraft display so old values do not continue to appear current. This is a flight-simulation visualization, not certified navigation or terrain-warning equipment.

## Traffic, weather and airspace context

The route map adds VATSIM controllers and aircraft, weather radar, GNSS interference overlays and terrain. Each layer can be toggled as needed. VATSIM aircraft remain orange in both themes, with readable callsign labels. Network traffic follows the official feed's refresh cadence rather than updating every frame.

BeyondATC and SayIntentions traffic options remain available through Settings. Traffic sources are mutually exclusive to avoid duplicate overlays. Weather, traffic and GNSS information depends on external services; coverage and freshness may vary.

## X-Plane 12 joins MSFS support

The Windows desktop application supports Microsoft Flight Simulator 2020, Microsoft Flight Simulator 2024 and X-Plane 12. X-Plane 12 supplies local position, heading, ground speed, on-ground state and altitude through its UDP DataRef interface, using port 49000 by default. Run the simulator and TaxiNow Pro on the same PC.

X-Plane simulator telemetry and X-Plane Scenery Gateway map data are separate capabilities: one supplies aircraft state, while the other provides a fallback source for airport mapping.

## Better aircraft follow and download recovery

Aircraft follow now handles both position and heading, addressing cases where the aircraft could taxi beyond the visible map without the camera keeping up. The route view also supports persistent aircraft follow. Location controls and icons have been refined to make their purpose clearer.

When an airport download appears stalled or fails, Maps & storage offers a manual fallback-source action. It bypasses OSM and map packs to try X-Plane Scenery Gateway, with OurAirports as the final runway-data fallback. The detail available from these sources varies, and some airports may have only basic runway information.

## Light and dark themes across the whole interface

Themes now cover the header, navigation rail, footer, map controls and popup panels. Airport names, simulator status and map summaries use readable dark text in light mode; dark mode retains clear contrast. Map controls share consistent dimensions and corner radii, zoom symbols are centred, the airport selector loses its extra arrow, and Settings can scroll again.

A sun/moon shortcut beside Settings makes appearance changes quick. The desktop WebView2 uses an sRGB colour profile to address yellow-tinted rendering in affected display environments. Minimizing goes to the taskbar by default, with a persistent Minimize to tray option for users who prefer it.

## Mobile access, feedback and updates

With TaxiNow Pro running on the PC, phones and tablets can open the address displayed in the header on the same local network. The supported baseline is Android 10 or later with Firefox 114 or later, or iOS/iPadOS 16.4 or later with Safari. The browser and GPU must support WebGL 2.0. The FAQ now includes these requirements and X-Plane connection guidance.

Report an issue in Settings opens the GitHub Bug Report / Feature Request chooser. Both forms request a summary, contact details, a problem description and the expected result. Submitted information is publicly visible.

The update dialog now distinguishes an available update, an up-to-date installation and a failed check. Contradictory headings and empty release-note boxes are gone. Open update installer folder provides access to downloaded installers for manual cleanup; it does not automatically delete files.

## Upgrading to V2.0

Close TaxiNow / TaxiNow Pro, then run `TaxiNow-Pro-V2.0-Build-207-Setup.exe`. It can install over an earlier version. Existing installation and data identifiers are retained for compatibility, and legacy shortcuts migrate to TaxiNow Pro. If you uninstall first, choose to keep maps and user data.

Advanced users can download `TaxiNow-Pro-V2.0-Build-207-Portable.zip`, extract it and run `TaxiNow.App.exe`. It contains the same application but does not provide the installer's shortcuts, uninstaller or prerequisite checks. Downloaded maps are not automatically stored inside the extracted application folder.

## Credits

Special thanks to **睡务局局长 ([@stewieqi-del](https://github.com/stewieqi-del))** for contributions to V2.0. Thanks also to the users who supplied reports, interface suggestions and testing feedback, and to the maintainers of the mapping sources, simulator interfaces and open-source components used by the application.

[Download V2.0 / Build 207](https://github.com/skylarkning/TaxiNow-Release/releases/tag/v2.0.0) · [Report a bug or request a feature](https://github.com/skylarkning/TaxiNow-Release/issues/new/choose)
