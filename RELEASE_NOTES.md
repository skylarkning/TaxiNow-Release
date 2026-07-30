# TaxiNow V1.0 Beta 3

## English

> **Important:** Uninstall any earlier TaxiNow version before installing Beta 3.
> The uninstaller removes downloaded map assets, so those maps must be
> downloaded again after installation.

### Short changelog

- Keeps OpenStreetMap as the preferred source during parallel country/region
  downloads by queueing requests instead of falling back after 25 seconds.
- Waits through short Overpass endpoint cooldowns without excessive polling or
  CPU use.
- Retries OSM sooner after a temporary Gateway or OurAirports fallback.
- Retains Gateway and OurAirports only as fallbacks when OSM is unavailable or
  lacks sufficient airport detail.

TaxiNow is free for personal, non-commercial flight-simulation use and is
provided **“AS IS”**, without warranties of any kind. It must not be used for
real-world navigation. Please read the repository introduction, license, EULA,
and disclaimer before installation.

### Acknowledgements and credits

TaxiNow thanks the contributors and maintainers of the following data sources,
projects, and technologies:

- [OpenStreetMap contributors](https://www.openstreetmap.org/copyright) —
  airport map data made available under the ODbL.
- [OurAirports](https://ourairports.com/data/) — public-domain airport and
  runway datasets.
- [X-Plane Scenery Gateway](https://gateway.x-plane.com/) — fallback airport
  layout data.
- [SkyCharts](https://github.com/skylarkning/SkyCharts) — airport-map visual
  conventions and rendering reference.
- [MapLibre GL JS](https://github.com/maplibre/maplibre-gl-js) — interactive
  map rendering.
- [Microsoft .NET](https://github.com/dotnet/runtime),
  [ASP.NET Core SignalR](https://github.com/dotnet/aspnetcore),
  [WebView2](https://developer.microsoft.com/microsoft-edge/webview2/), and the
  Microsoft Flight Simulator SimConnect SDK — application runtime, live
  updates, Windows interface, and simulator integration.
- [SQLite](https://www.sqlite.org/) and
  [SQLitePCLRaw](https://github.com/ericsink/SQLitePCL.raw) — local asset
  storage.
- [PyInstaller](https://pyinstaller.org/) and
  [Inno Setup](https://jrsoftware.org/isinfo.php) — Windows packaging and
  installation.

Each third-party component or dataset remains subject to its own license and
terms. See the repository
[NOTICE](https://github.com/skylarkning/TaxiNow-Release/blob/main/NOTICE) for
the formal data notices.

## 中文

> **重要：**安装 Beta 3 前，请先卸载任何旧版 TaxiNow。卸载程序会删除已下载的
> 地图资源，因此安装完成后需要重新下载地图。

### 简短更新日志

- 国家/地区并行下载时延长 OSM 请求排队时间，不再等待 25 秒后过早切换来源。
- Overpass 服务短暂冷却时继续低资源等待，避免频繁轮询。
- 临时使用 Gateway 或 OurAirports 后会更快重试 OSM。
- 仅在 OSM 不可用或机场数据不足时使用 Gateway 与 OurAirports 作为后备来源。

TaxiNow 完全免费，仅供个人、非商业模拟飞行使用，并按“现状”提供，不作任何形式的担保。
严禁用于真实飞行导航。安装前请阅读仓库介绍、许可协议、最终用户许可协议及免责声明。

### 致谢与 Credits

TaxiNow 感谢以下数据来源、项目、技术的贡献者与维护者：

- [OpenStreetMap 贡献者](https://www.openstreetmap.org/copyright) —
  依据 ODbL 提供机场地图数据。
- [OurAirports](https://ourairports.com/data/) — 提供公有领域机场及跑道数据集。
- [X-Plane Scenery Gateway](https://gateway.x-plane.com/) —
  提供后备机场布局数据。
- [SkyCharts](https://github.com/skylarkning/SkyCharts) —
  提供机场地图视觉规范与绘制方式参考。
- [MapLibre GL JS](https://github.com/maplibre/maplibre-gl-js) —
  提供交互式地图绘制能力。
- [Microsoft .NET](https://github.com/dotnet/runtime)、
  [ASP.NET Core SignalR](https://github.com/dotnet/aspnetcore)、
  [WebView2](https://developer.microsoft.com/microsoft-edge/webview2/) 及
  Microsoft Flight Simulator SimConnect SDK —
  用于程序运行、实时更新、Windows 界面及模拟器连接。
- [SQLite](https://www.sqlite.org/) 与
  [SQLitePCLRaw](https://github.com/ericsink/SQLitePCL.raw) —
  用于本地资源存储。
- [PyInstaller](https://pyinstaller.org/) 与
  [Inno Setup](https://jrsoftware.org/isinfo.php) —
  用于 Windows 打包及安装程序制作。

各第三方组件及数据集仍分别受其自身许可证及条款约束。正式数据声明请参阅
[NOTICE](https://github.com/skylarkning/TaxiNow-Release/blob/main/NOTICE)。
