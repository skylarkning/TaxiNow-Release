# TaxiNow V1.4.4 — Build 122

Release date: August 23, 2026

## Changelog

- Fixed a race that could leave the aircraft position icon hidden when
  telemetry arrived while the map layer was still loading. A stationary
  aircraft no longer has to move before the icon appears.
- The aircraft icon now synchronizes as soon as either the native map layer or
  SVG fallback becomes ready, including after switching airports.
- Ownship animation now starts immediately after its map layer is created
  instead of waiting for the map idle event or fallback timeout.

Close TaxiNow, then run `TaxiNow-V1.4.4-Build-122-Setup.exe`. It may be installed
over an earlier version. If you uninstall first, choose to keep downloaded maps
and user data.

---

# TaxiNow V1.4.4 — 内部版本 122

发布日期：2026年8月23日

## 更新日志

- 修复飞机遥测数据在地图图层加载期间到达时，当前位置图标可能一直隐藏的竞态问题。飞机静止时也无需等到移动后才显示图标。
- 地图原生图层或 SVG 后备图层就绪后会立即同步飞机图标，切换机场后同样有效。
- 飞机位置动画会在图层创建后立即启动，不再等待地图空闲事件或超时兜底。

关闭 TaxiNow 后运行 `TaxiNow-V1.4.4-Build-122-Setup.exe`，可覆盖安装旧版本。
如先卸载旧版，请选择保留已下载地图和用户数据。

## Acknowledgements and credits / 致谢

TaxiNow thanks the contributors and maintainers of OpenStreetMap, OurAirports,
FAA Airport Mapping Open Data, Geofabrik, Overture Maps, Microsoft Global ML
Building Footprints, X-Plane Scenery Gateway, SkyCharts, MapLibre GL JS,
Microsoft .NET, WebView2, SimConnect, SQLite, PyInstaller, and Inno Setup.

TaxiNow is free for personal, non-commercial flight-simulation use and is
provided **“AS IS”**, without warranties of any kind.
