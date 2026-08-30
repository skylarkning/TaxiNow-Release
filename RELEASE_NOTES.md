# TaxiNow V1.5 — Build 126

Release date: August 30, 2026

## Changelog

- Added an opt-in **Show VATSIM Traffic** setting for desktop and browser/iPad
  maps. The local MSFS aircraft remains cyan; nearby VATSIM aircraft use small
  orange plane icons with upright callsign labels.
- TaxiNow's PC service reads the official public VATSIM network-data feed,
  caches it for about 15 seconds, and returns only aircraft within the selected
  airport area. Pilot names and VATSIM account IDs are not forwarded to the map.
- Added a FAQ explaining VATSIM's approximately 15-second official refresh
  cadence and TaxiNow's shared PC-side cache.
- Customized taxi routes now accept commas, spaces, or mixed separators.
  Destinations containing a space, such as `GATE B19`, remain supported.
- Retains the Build 123 iPad aircraft-icon synchronization fix, unified desktop
  and iPad SVG icon, 10% smaller icon, and 20% wider taxiway pavement.

Close TaxiNow, then run `TaxiNow-V1.5-Build-126-Setup.exe`. It may be installed
over an earlier version. If you uninstall first, choose to keep downloaded maps
and user data.

---

# TaxiNow V1.5 — 内部版本 126

发布日期：2026年8月30日

## 更新日志

- 设置中新增可选的 **显示 VATSIM 交通**。本机 MSFS 飞机保持青色，附近的
  VATSIM 飞机使用橘色小飞机图标，并在下方显示正向呼号。
- TaxiNow 电脑端服务读取 VATSIM 官方公开网络数据源，缓存约 15 秒，并只返回
  当前机场区域内的飞机。飞行员姓名和 VATSIM 账号 ID 不会发送到地图端。
- FAQ 新增 VATSIM 官方数据约 15 秒刷新一次及电脑端共享缓存的说明。
- 自定义滑行路线现在支持逗号、空格或混合分隔；`GATE B19` 等带空格的目的地
  仍可正常识别。
- 保留 Build 123 的 iPad 飞机图标即时同步修复、桌面与 iPad 统一 SVG 图标、
  图标缩小 10% 以及滑行道灰色铺装加宽 20%。

关闭 TaxiNow 后运行 `TaxiNow-V1.5-Build-126-Setup.exe`，可覆盖安装旧版本。
如先卸载旧版，请选择保留已下载地图和用户数据。

## Acknowledgements and credits / 致谢

TaxiNow thanks the contributors and maintainers of OpenStreetMap, OurAirports,
FAA Airport Mapping Open Data, Geofabrik, Overture Maps, Microsoft Global ML
Building Footprints, X-Plane Scenery Gateway, SkyCharts, MapLibre GL JS,
Microsoft .NET, WebView2, SimConnect, SQLite, PyInstaller, and Inno Setup.

TaxiNow is free for personal, non-commercial flight-simulation use and is
provided **“AS IS”**, without warranties of any kind.
