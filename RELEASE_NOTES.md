# TaxiNow V1.4.5 — Build 123

Release date: August 23, 2026

## Changelog

- Fixed an iPad WebKit rendering delay that could leave the aircraft-position
  icon hidden for roughly two minutes even though telemetry was already
  synchronized.
- Desktop and iPad now use the same SVG aircraft icon. The icon renders
  immediately on iPad and is 10% smaller for improved map visibility.
- Widened taxiway pavement and its outline by 20% in both the normal and
  fallback map renderers.

Close TaxiNow, then run `TaxiNow-V1.4.5-Build-123-Setup.exe`. It may be installed
over an earlier version. If you uninstall first, choose to keep downloaded maps
and user data.

---

# TaxiNow V1.4.5 — 内部版本 123

发布日期：2026年8月23日

## 更新日志

- 修复 iPad WebKit 的图标渲染延迟：即使遥测已同步，飞机位置图标此前仍可能约两分钟后才出现。
- 桌面端与 iPad 现在使用相同的 SVG 飞机图标；iPad 可立即显示，图标缩小 10%，减少地图遮挡。
- 普通地图与后备地图中的滑行道灰色铺装及其边缘均加宽 20%。

关闭 TaxiNow 后运行 `TaxiNow-V1.4.5-Build-123-Setup.exe`，可覆盖安装旧版本。
如先卸载旧版，请选择保留已下载地图和用户数据。

## Acknowledgements and credits / 致谢

TaxiNow thanks the contributors and maintainers of OpenStreetMap, OurAirports,
FAA Airport Mapping Open Data, Geofabrik, Overture Maps, Microsoft Global ML
Building Footprints, X-Plane Scenery Gateway, SkyCharts, MapLibre GL JS,
Microsoft .NET, WebView2, SimConnect, SQLite, PyInstaller, and Inno Setup.

TaxiNow is free for personal, non-commercial flight-simulation use and is
provided **“AS IS”**, without warranties of any kind.
