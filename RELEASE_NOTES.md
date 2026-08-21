# TaxiNow V1.4.3 — Build 121

Release date: August 21, 2026

## Changelog

- Corrected EDDF Runway 18 so its single operational designator appears only
  at the correct threshold instead of being duplicated at both ends.
- Added an optional vMAS presence integration for the authorized
  `https://vmas.my` origin.
- The integration is disabled by default and exposes only whether TaxiNow is
  available plus its version and build number. It does not expose simulator or
  aircraft telemetry.
- Added localized settings and explanatory text for the integration.

Close TaxiNow, then run `TaxiNow-V1.4.3-Build-121-Setup.exe`. It may be installed
over an earlier version. If you uninstall first, choose to keep downloaded maps
and user data.

---

# TaxiNow V1.4.3 — 内部版本 121

发布日期：2026年8月21日

## 更新日志

- 修正EDDF的18号跑道标号，使其仅在正确的跑道端显示，不再在两端重复标注18。
- 新增针对已授权来源`https://vmas.my`的可选vMAS在线状态集成。
- 该功能默认关闭，仅提供TaxiNow是否在线、版本号和内部构建号，不提供模拟器或飞机遥测数据。
- 为该功能添加了多语言设置与说明。

关闭TaxiNow后运行`TaxiNow-V1.4.3-Build-121-Setup.exe`，可覆盖安装旧版本。
如先卸载旧版，请选择保留已下载地图和用户数据。

## Acknowledgements and credits / 致谢

TaxiNow thanks the contributors and maintainers of OpenStreetMap, OurAirports,
FAA Airport Mapping Open Data, Geofabrik, Overture Maps, Microsoft Global ML
Building Footprints, X-Plane Scenery Gateway, SkyCharts, MapLibre GL JS,
Microsoft .NET, WebView2, SimConnect, SQLite, PyInstaller, and Inno Setup.

TaxiNow is free for personal, non-commercial flight-simulation use and is
provided **“AS IS”**, without warranties of any kind.
