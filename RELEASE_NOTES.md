# TaxiNow V1.5.1 — Build 127

Release date: September 5, 2026

## Changelog

- Fixed a long-flight tracking failure where a legitimate telemetry gap could
  leave the aircraft icon missing at the destination until TaxiNow was
  restarted. Tracking now safely re-establishes itself after several
  consistent samples while still rejecting isolated invalid coordinates.
- TaxiNow now identifies the aircraft's current airport once ground tracking is
  stable. It switches automatically when that airport map is installed.
- If the current airport map is not installed, the airport picker opens with a
  clear download prompt. The downloaded map opens automatically when ready.
- A manual map choice made while on the ground is respected; automatic airport
  selection resumes after takeoff.
- Includes all V1.5 features, including optional VATSIM traffic, callsign
  labels, and space-separated customized taxi routes.

Close TaxiNow, then run `TaxiNow-V1.5.1-Build-127-Setup.exe`. It may be installed
over an earlier version. If you uninstall first, choose to keep downloaded maps
and user data.

---

# TaxiNow V1.5.1 — 内部版本 127

发布日期：2026年9月5日

## 更新日志

- 修复长途飞行中出现正常遥测间隔后，目的地机场的飞机图标可能一直不显示、
  必须重启 TaxiNow 才能恢复的问题。连续收到一致位置后会安全地自动重新同步，
  单次异常坐标仍会被过滤。
- 地面位置稳定后，TaxiNow 会自动识别飞机当前所在机场；地图已安装时自动切换。
- 当前机场地图未安装时，机场选择器会自动打开并提示下载；下载完成后自动显示。
- 在地面手动选择的地图不会被覆盖；起飞后自动机场选择恢复。
- 包含 V1.5 的全部功能，包括可选 VATSIM 交通、呼号标签和空格分隔的自定义
  滑行路线。

关闭 TaxiNow 后运行 `TaxiNow-V1.5.1-Build-127-Setup.exe`，可覆盖安装旧版本。
如先卸载旧版，请选择保留已下载地图和用户数据。

## Acknowledgements and credits / 致谢

TaxiNow thanks the contributors and maintainers of OpenStreetMap, OurAirports,
FAA Airport Mapping Open Data, Geofabrik, Overture Maps, Microsoft Global ML
Building Footprints, X-Plane Scenery Gateway, SkyCharts, MapLibre GL JS,
Microsoft .NET, WebView2, SimConnect, SQLite, PyInstaller, and Inno Setup.

TaxiNow is free for personal, non-commercial flight-simulation use and is
provided **“AS IS”**, without warranties of any kind.
