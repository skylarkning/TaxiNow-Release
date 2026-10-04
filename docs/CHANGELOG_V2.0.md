# TaxiNow Pro V2.0 — Build 206

Release date: October 3, 2026

TaxiNow is now **TaxiNow Pro**. V2.0 connects airport taxiing, globe route exploration and the vertical situation profile in one workspace.

[Read the full English V2.0 blog](https://github.com/skylarkning/TaxiNow-Release/blob/main/docs/BLOG_V2.0.en.md) · [阅读完整中文 V2.0 更新文章](https://github.com/skylarkning/TaxiNow-Release/blob/main/docs/BLOG_V2.0.zh-CN.md)

## What's new

- New Route workspace with a globe, 2D/3D switching and a north-up compass; Route is the default startup view.
- SimBrief import with route waypoints, aircraft type, planned altitude and fit-route controls; the username is saved in the browser.
- Departure and arrival airport map downloads from the flight plan, with a destination taxi-map switch after touchdown.
- Full-screen vertical route profile with terrain, planned altitude, available altitude constraints, MSL/AGL telemetry, terrain clearance and destination distance; estimated paths are labelled.
- Stale telemetry clears the live profile display after 15 seconds, and incomplete X-Plane reconnect data cannot restore old position or altitude.
- Windows telemetry support for MSFS 2020, MSFS 2024 and X-Plane 12 through the local UDP DataRef interface.
- VATSIM controllers and traffic, weather radar, GNSS interference and terrain overlays in the route workspace.
- VATSIM aircraft remain orange in both themes; existing BeyondATC and SayIntentions traffic options remain available with mutually exclusive sources.
- Continuous position and heading follow for taxiing, plus persistent aircraft follow in the route view.
- Manual fallback-source action for stalled or failed airport downloads: bypass OSM and map packs to try X-Plane Scenery Gateway, with OurAirports as the final runway fallback.
- Compact single-row header, current ICAO airport selector, airport name beside the flight number and a combined attribution/status footer.
- Consistent Flight and Route Info drawers, popup styling, transitions, button corners and map-control sizes; centred zoom symbols and improved aircraft location icon.
- Light and dark appearance across the full workspace, improved text contrast and a sun/moon shortcut beside Settings.
- Desktop WebView2 sRGB configuration to address yellow-tinted rendering in affected environments.
- Scrollable Settings; taskbar minimization by default with an optional persistent Minimize to tray setting.
- Clear plan beside Import, improved import spacing and airport shortcut spacing.
- Localization improvements across all seven interface languages; Profile uses normal title casing.
- FAQ updates for X-Plane 12 and mobile access: Android 10+ / Firefox 114+, or iOS/iPadOS 16.4+ / Safari, with WebGL 2.0 and a shared local network.
- In-app Report an issue button and required Bug Report / Feature Request forms for Summary, contact details, problem description and expected result.
- Clear available/current/error update-dialog states; empty release-note boxes are hidden.
- Open update installer folder for manual cleanup, without automatic file deletion.
- TaxiNow Pro application branding, corrected runtime window title and legacy shortcut migration; existing data identifiers remain compatible.

## Upgrade

Close TaxiNow / TaxiNow Pro, then run `TaxiNow-Pro-V2.0-Build-206-Setup.exe`. It may be installed over an earlier version. If uninstalling first, choose to keep downloaded maps and user data.

For Portable, extract `TaxiNow-Pro-V2.0-Build-206-Portable.zip` and run `TaxiNow.App.exe`. WebView2 Runtime is required; Portable does not perform the installer's prerequisite checks or create shortcuts. Maps remain in the configured user-data location rather than automatically moving into the extracted folder.

## Credits

Special thanks to **睡务局局长 ([@stewieqi-del](https://github.com/stewieqi-del))** for contributions to V2.0, and to everyone who provided reports and testing feedback. Thank you to the mapping-source and open-source maintainers whose work supports TaxiNow Pro.

---

# TaxiNow Pro V2.0 — 内部版本 206

发布日期：2026年10月3日

TaxiNow 正式更名为 **TaxiNow Pro**。V2.0 将机场滑行、地球航线浏览与垂直剖面连接到同一工作区。

## 更新日志

- 新增航线地球工作区、2D/3D 切换和正北指南针；启动默认显示航线页。
- 新增 SimBrief 导入，展示航路点、机型、计划高度并支持完整航路适配；用户名在浏览器中自动保存。
- 根据飞行计划尝试下载出发及到达机场地图，落地后切换到目的地地面地图。
- 新增全屏垂直航线剖面，展示地形、计划高度、可用高度限制、实时 MSL/AGL、高度间隔及目的地距离；估算路径明确标注。
- 遥测过期 15 秒后清除实时剖面状态，X-Plane 重连的不完整数据不会恢复旧位置或高度。
- Windows 端支持 MSFS 2020、MSFS 2024，以及通过本机 UDP DataRef 接口连接的 X-Plane 12。
- 航线地图加入 VATSIM 管制及飞机交通、天气雷达、GNSS 干扰和地形图层。
- 亮色和暗色模式的 VATSIM 飞机均为橘色；保留 BeyondATC、SayIntentions 交通选项，交通来源互斥避免重复。
- 修复地面持续位置及航向跟随，并支持航线视图持续跟随飞机。
- 机场下载卡住或失败时可尝试后备资源：跳过 OSM 和地图包，尝试 X-Plane Scenery Gateway，最终以 OurAirports 跑道数据后备。
- 顶部两行合并为一行，增加当前 ICAO 机场选择器，机场名称置于航班号旁，合并底部来源与状态栏。
- 统一飞行计划、航路信息及弹出菜单的样式和动画；统一地图工具尺寸和圆角，加减号居中，改进定位飞机图标。
- 亮暗主题覆盖完整外框及工作区，提高文字对比度，恢复设置旁太阳/月亮快捷切换。
- 桌面 WebView2 使用 sRGB 配置，改善特定显示环境中的泛黄渲染。
- 修复设置菜单滚动；默认最小化到任务栏，可选择并保存最小化到托盘。
- 清除计划移到导入右侧，增加导入按钮及机场快捷按钮的间距。
- 改进全部七种界面语言的本地化；Profile 不再全部大写。
- FAQ 更新 X-Plane 12 和移动端要求：Android 10+ / Firefox 114+，或 iOS/iPadOS 16.4+ / Safari，并要求 WebGL 2.0 与同一局域网。
- 设置新增报告问题按钮，GitHub Bug Report / Feature Request 表单要求填写 Summary、联系方式、问题描述和预期结果。
- 更新弹窗明确区分发现新版本、已是最新版及检查失败，隐藏空白发行说明。
- 增加打开更新安装包目录按钮，供用户手动清理，不自动删除文件。
- 全面更新 TaxiNow Pro 品牌名称，修复运行时窗口标题并迁移旧快捷方式，同时保持已有数据兼容。

## 升级方法

关闭 TaxiNow / TaxiNow Pro 后运行 `TaxiNow-Pro-V2.0-Build-206-Setup.exe`，可覆盖安装旧版本。如先卸载，请选择保留已下载地图和用户数据。

Portable 用户解压 `TaxiNow-Pro-V2.0-Build-206-Portable.zip` 后运行 `TaxiNow.App.exe`。需要 WebView2 Runtime，Portable 不提供安装器的前置环境检查或快捷方式创建。地图保留在配置的用户数据目录，不会自动移到解压目录。

## 致谢

特别感谢 **睡务局局长（[@stewieqi-del](https://github.com/stewieqi-del)）** 对 V2.0 的贡献，以及提供问题反馈和测试结果的用户。感谢各地图数据源及开源组件的维护者。

## SHA-256

- `TaxiNow-Pro-V2.0-Build-206-Setup.exe`: `8E018885B6F4D82E424ADCF21DBA761520E2A83FA24A2972E6E8F4C89DB5EDAE`
- `TaxiNow-Pro-V2.0-Build-206-Portable.zip`: `EBEFDEFC90BF0C5C5E3A328BB2245BDEF04DE13207AC9D379EED21D8339BCE9C`

Flight simulation use only. Not for real-world navigation.
仅供模拟飞行使用，严禁用于真实导航。
