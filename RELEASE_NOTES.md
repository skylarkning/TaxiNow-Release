# TaxiNow V1.0 Beta 4

## English

> **Important:** Uninstall any earlier TaxiNow version before installing Beta 4.
> Choose **Yes** when asked to keep downloaded maps and user data, so they can
> be reused after installation.

### Changelog

- Keeps OpenStreetMap as the preferred detailed-map source while reducing
  response time with smaller runway-based requests, adaptive endpoint
  selection, and endpoint cooldowns.
- Adds a clear 120-second OSM wait limit, visible **Stalled** and **Failed**
  states, and in-app guidance for normal and abnormal download times.
- Bundles the airport/runway catalog, adds a second catalog mirror, and reuses
  a stale local catalog when the network is reset or unavailable. This avoids
  many first-run `WinError 10054` failures.
- Removes isolated nearby-airport and heliport geometry that could make
  **Fit airport** zoom too far out, including the reported KLGA and KDCA cases.
- Adds an English / Simplified Chinese language selector and localized app,
  map controls, download manager, asset library, status text, welcome screen,
  and About page.
- Shows names such as Beijing and Tokyo instead of codes such as `CN-11` and
  `JP-13` in the downloaded-asset hierarchy.
- Moves **Fit airport** into an icon above the position-refresh and zoom
  controls, and renames **Asset storage** to **Downloaded Asset**.
- Beta 4 update: restores the fixed bilingual welcome screen, completes the
  Chinese About page, adds a globe language menu, and makes the long Chinese
  download-help bubble scroll safely within the window.
- Beta 4 update: suppresses unreliable whole-country ETAs until enough
  airports have completed, explains the expected duration of large country
  downloads, and conditionally supplements incomplete OSM terminal coverage
  with X-Plane terminal footprints while keeping OSM primary.
- Beta 4 update: the uninstaller now defaults to preserving downloaded maps
  and user data for upgrades, with an explicit option to delete everything.

TaxiNow is free for personal, non-commercial flight-simulation use and is
provided **“AS IS”**, without warranties of any kind. It must not be used for
real-world navigation. Please read the repository introduction, license, EULA,
and disclaimer before installation.

## 中文

> **重要：**安装 Beta 4 前，请先卸载任何旧版 TaxiNow。卸载器询问是否保留地图和
> 用户数据时请选择 **“是”**，安装新版后即可继续使用。

### 更新日志

- 继续优先使用 OpenStreetMap 详细地图数据，同时通过基于跑道范围的更小请求、
  自适应节点选择和节点冷却机制改善响应速度。
- OSM 最长等待时间明确为 120 秒；新增清晰的“疑似卡住”和“失败”状态，并在
  下载页面说明正常与异常的等待时间。
- 内置机场与跑道目录，增加第二个目录镜像，并在网络重置或不可用时复用本地旧
  目录，减少首次运行时的 `WinError 10054` 错误。
- 过滤附近其他机场或直升机场的孤立图形，修复 KLGA、KDCA 等机场“适配机场范围”
  缩放过远的问题。
- 新增英文 / 简体中文切换，应用界面、地图控制、下载管理、资源库、状态文字、
  欢迎界面和关于页面均支持中文。
- 已下载资源层级会显示“北京市”“东京都”等实际名称，不再只显示 `CN-11`、
  `JP-13` 等代码。
- “适配机场范围”改为位于位置刷新和缩放按钮上方的图标按钮；“Asset storage”
  更名为“Downloaded Asset（已下载资源）”。
- Beta 4 更新：恢复固定的英中双语欢迎页，补全中文“关于”页，语言按钮改为地球仪
  下拉菜单，并让较长的中文下载说明气泡在窗口内安全滚动。
- Beta 4 更新：整国下载完成足够机场样本前不再显示不可靠的夸张 ETA；新增整国下载
  时间提示；在 OSM 航站楼覆盖不完整时仅补充 X-Plane 航站楼轮廓，仍保持 OSM 优先。
- Beta 4 更新：卸载器默认保留已下载地图和用户数据以便升级复用，同时提供彻底删除选项。

TaxiNow 完全免费，仅供个人、非商业模拟飞行使用，并按“现状”提供，不作任何
形式的担保。严禁用于真实飞行导航。安装前请阅读仓库介绍、许可协议、最终用户
许可协议及免责声明。

## Acknowledgements and credits / 致谢与 Credits

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
  Microsoft Flight Simulator SimConnect SDK.
- [SQLite](https://www.sqlite.org/), [SQLitePCLRaw](https://github.com/ericsink/SQLitePCL.raw),
  [PyInstaller](https://pyinstaller.org/), and
  [Inno Setup](https://jrsoftware.org/isinfo.php).

Each third-party component or dataset remains subject to its own license and
terms. See [NOTICE](NOTICE) for the formal notices.
