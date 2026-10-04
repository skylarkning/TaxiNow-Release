<p align="center">
  <img src="assets/taxinow-logo.png" width="540" alt="TaxiNow Pro" />
</p>

# TaxiNow Pro V2.0 (Build 206)

**[English](#english) | [中文](#中文)**

> Flight simulation use only. Not for real-world navigation.<br>
> 仅供模拟飞行使用，严禁用于真实飞行导航。

## V2.0 · Build 206

- **[Windows installer / 安装包](https://github.com/skylarkning/TaxiNow-Release/releases/download/v2.0.0/TaxiNow-Pro-V2.0-Build-206-Setup.exe)**
- **[Portable ZIP / 便携版](https://github.com/skylarkning/TaxiNow-Release/releases/download/v2.0.0/TaxiNow-Pro-V2.0-Build-206-Portable.zip)**
- [Release notes / 发布说明](https://github.com/skylarkning/TaxiNow-Release/releases/tag/v2.0.0) · [SHA-256 checksums / 校验值](docs/SHA256SUMS_V2.0.txt)
- [English V2.0 blog](docs/BLOG_V2.0.en.md) · [中文 V2.0 更新文章](docs/BLOG_V2.0.zh-CN.md) · [Bilingual changelog / 双语更新日志](docs/CHANGELOG_V2.0.md)
- [Report a bug or request a feature / 报告问题或建议](https://github.com/skylarkning/TaxiNow-Release/issues/new/choose)

## Official downloads

Official TaxiNow Pro releases are published only by **skylarkning** through:

- the official [TaxiNow Pro listing on flightsim.to](https://flightsim.to/addon/112712/taxinow); and
- this [TaxiNow-Release repository](https://github.com/skylarkning/TaxiNow-Release)
  and its [Releases page](https://github.com/skylarkning/TaxiNow-Release/releases).

Copies from any other website, marketplace, file-sharing service, group, or
individual are unofficial and may have been modified. TaxiNow Pro is 100% free.
If you paid for it, the seller was not authorized by Sky Ning.

TaxiNow Pro 官方版本仅由 **skylarkning** 通过以下两处发布：

- [flightsim.to 上的 TaxiNow Pro 官方页面](https://flightsim.to/addon/112712/taxinow)；以及
- 本 [TaxiNow-Release 仓库](https://github.com/skylarkning/TaxiNow-Release)
  及其 [Releases 页面](https://github.com/skylarkning/TaxiNow-Release/releases)。

其他网站、平台、网盘、群组或个人提供的版本均非官方版本，并可能已被修改。
TaxiNow Pro 完全免费；如果你付费购买了本软件，卖家并未获得 Sky Ning 授权。

---

## English

### Introduction

TaxiNow Pro is a Windows application running locally on your PC. V2.0 brings
airport ground maps, a 2D/3D globe route workspace, SimBrief import and a vertical
route profile together. It displays live aircraft position, heading and altitude
from MSFS through SimConnect or X-Plane 12 through the local UDP DataRef interface.

TaxiNow Pro is intended exclusively for personal flight-simulator use. It is not
certified or suitable for real-world aviation, navigation, flight planning, or
operational training.

### Simulator compatibility

- **Microsoft Flight Simulator 2024:** tested and supported
- **Microsoft Flight Simulator 2020:** tested and supported
- **X-Plane 12:** supported through local UDP DataRefs (default port 49000); run on the same PC as TaxiNow Pro

### Main features

- Default Route workspace with a 2D/3D globe and north-up compass
- SimBrief route import with waypoints, aircraft type, planned altitude and browser-saved username
- Full-screen vertical profile with terrain, planned altitude, available constraints and live MSL/AGL; estimated paths are labelled and stale telemetry is cleared
- Flight-plan departure/arrival map downloads and destination taxi-map switching after touchdown
- VATSIM controllers, weather radar, GNSS interference and terrain overlays
- Continuous aircraft position and heading follow in Taxi, plus persistent Route follow
- Manual fallback downloads through X-Plane Scenery Gateway, with OurAirports as the final runway fallback; detail varies by source
- Compact header and footer, ICAO selector, matching Flight/Route Info drawers and consistently sized map controls
- Readable light/dark themes throughout the interface and desktop WebView2 sRGB rendering
- In-app issue forms, clear update-dialog states and manual access to downloaded installer files
- Detailed airport ground maps
- Runways, taxiways, taxilanes, aprons, terminals, parking stands, and labels
- Live aircraft position and heading through MSFS SimConnect or X-Plane 12 UDP DataRefs
- Optional nearby VATSIM traffic from the official public network-data feed,
  shown as orange aircraft with upright callsign labels; the local MSFS
  aircraft remains cyan
- Optional nearby BeyondATC traffic injected into MSFS, read through SimConnect
  and shown as violet aircraft with heading-aware callsign labels
- Dedicated SayIntentions traffic integration using the active local flight ID
  and the official SayIntentions Tracker, preserving real callsigns while
  matching aircraft to live SimConnect positions
- VATSIM, BeyondATC, and SayIntentions traffic displays are mutually exclusive;
  selecting one automatically disables and clears the other two
- Reliable aircraft-icon synchronization as soon as the map layer becomes
  ready, including for stationary aircraft and after switching airports
- Automatic recovery after legitimate long-distance telemetry gaps, so the
  destination-airport icon no longer requires restarting TaxiNow Pro
- Automatic switching to the aircraft's current airport after landing; if the
  map is missing, TaxiNow Pro opens the airport picker with a download prompt
- One consistent SVG aircraft icon on desktop and iPad, with immediate iPad
  rendering and a compact 32.4 px display size
- Taxiway pavement and outlines widened by 20% for clearer ground-map reading
- Simulator connection and synchronization status
- Manual position refresh
- English, Simplified Chinese, Traditional Chinese, Japanese, French, German, and Korean interface
- Settings menu with language selection and an optional **Keep window visible** mode
- Collision-aware header layout that folds content only when the rendered text would overlap
- Automatic taxi-route planning with multiple route choices
- Blue route highlighting, live progress, and turn guidance
- Experimental customized taxi-route entry with connected-taxiway filtering;
  commas, spaces, or mixed separators are accepted
- Manual taxi start and destination placement by right-click or touch-and-hold
- Dark and light appearances with a one-click sun/moon switch
- Detailed runway threshold, aiming-point, touchdown-zone, runway-number, and blast-pad/stopway graphics
- Automatic update checks with official download and in-app installer choices
- Remembers the last successfully displayed airport between launches
- Optional heading-up navigation lock with the aircraft followed at the lower center
- Airport search and quick ICAO map acquisition
- Map acquisition by ICAO, Country/Region, or Province/State
- Configurable batch workers: 1, 2, 4, 8, or 16; use 1 for public OSM
- Verified, resumable regional map packs when available, with automatic
  on-demand fallback for missing airports
- Progress, speed, elapsed time, and estimated remaining time
- Human-readable Chinese province and Japanese prefecture names
- Map library grouped by Country/Region → Province/State → Airport
- Storage usage, free-space information, and customizable storage location
- Optional access from another device on the same trusted local network
- Optional privacy-minimized vMAS online-presence integration, disabled by
  default and restricted to the authorized `https://vmas.my` origin
- Minimizes to the taskbar by default, with an optional persistent **Minimize to tray** setting

TaxiNow Pro uses continuous OSM and available FAA building footprints ahead of
modular X-Plane facade pieces. Preprocessed packs can additionally use
strictly filtered Overture and Microsoft global building footprints. Complete
parent-building outlines suppress overlapping building parts, and reliable
nearby terminal/concourse names are transferred to accepted unnamed
footprints. This improves fragmented or missing terminals while retaining
Gateway taxi-route and parking-position detail.

TaxiNow Pro now includes a repeatable worldwide preprocessing pipeline that splits
large countries by available province/state extracts and publishes bounded,
resumable, checksum-verified shards. A country becomes a fast batch download
after its generated packs are uploaded to the official index; countries not
yet published continue to use the slower on-demand fallback. Incomplete pilot
packs have been withdrawn and will not be offered to TaxiNow Pro clients.

Taxi-route guidance is generated by a generic pathfinding algorithm for flight
simulation. It may not reflect ATC instructions, taxiway direction, aircraft
wingspan limits, closures, or real-world procedures. Review every route before
use; customized taxi routes are available when an automatic route is unsuitable.

### Installation

1. Close TaxiNow Pro. V2.0 may be installed over an earlier version. If you prefer
   to uninstall first, choose **Yes** when asked to keep downloaded maps and
   user data so the new installation can reuse them.
2. Download the installer from one of the two official channels above.
3. Run `TaxiNow-Pro-V2.0-Build-206-Setup.exe`.
4. Read and accept the EULA.
5. Complete setup and launch TaxiNow Pro.

TaxiNow Pro installs for the current Windows user and normally does not require
administrator privileges. Required Windows components are detected or
installed automatically.

### Getting started

1. Start TaxiNow Pro and MSFS 2020/2024 or X-Plane 12 on the same PC.
2. The Route globe is the default view. Open **Flight → Import** to load a SimBrief plan.
3. Use **Route Info** for waypoint details or **Profile** for the vertical route display.
4. Select an airport using its ICAO code, download its map if needed, and switch to **Taxi** for ground navigation.
5. Once simulator synchronization is green, enable aircraft follow as needed.
6. Use **Maps & storage** for downloads and storage. For a stalled or failed airport download, try the fallback-source action.

Portable users: extract the ZIP and run `TaxiNow.App.exe`. WebView2 Runtime is
required. Portable does not create shortcuts or perform installer prerequisite
checks, and maps remain in the configured user-data location.

### Access from another device

TaxiNow Pro can display the active map on another device connected to the same
trusted private network. Use the local-network address shown in the header.
Supported baseline: Android 10+ with Firefox 114+, or iOS/iPadOS 16.4+ with Safari.
The browser and GPU must support WebGL 2.0; keep the PC application running.

The local companion view uses HTTP without authentication. Do not expose its
port through a router, and do not use this feature on public or untrusted
networks. If Windows Firewall asks, allow Private networks only.

### Security and privacy

TaxiNow Pro does not require an account, contain advertising, include built-in
behavioral analytics, or automatically upload crash reports. Maps, settings,
logs, caches, and the asset database are stored locally.

For ground tracking, TaxiNow Pro reads latitude, longitude, true heading,
on-ground state, ground speed, and available MSL/AGL altitude from the simulator. It does not intentionally
send live aircraft position to map-data providers.

The optional VATSIM traffic setting is off by default. When enabled, TaxiNow Pro's
PC service requests the official public VATSIM network-data feed, caches it for
about 15 seconds, and forwards only the nearby aircraft fields needed for the
map. Local simulator telemetry is not sent to VATSIM.

The optional BeyondATC and SayIntentions traffic settings are also off by
default. BeyondATC traffic is read from non-user aircraft already injected into
MSFS through SimConnect. For SayIntentions, TaxiNow Pro reads only the active
`flight_id` from the documented local SAPI response, then requests that flight's
traffic from the official SayIntentions Tracker so real callsigns can be matched
to live simulator positions. TaxiNow Pro does not expose or log the SayIntentions
API key, email address, or other account fields. Only one of VATSIM, BeyondATC,
or SayIntentions traffic can be displayed at a time.

TaxiNow Pro source code is not publicly available. Qualified independent security
or privacy experts may request limited review access from Sky Ning solely to
verify TaxiNow Pro's security or privacy behavior. Approval and review conditions
are at the developer's discretion. Review access does not grant permission to
copy, modify, compile, publish, disclose, or redistribute the source code.

### License and disclaimer

TaxiNow Pro is copyrighted software and is not open-source or public-domain
software. It is provided free of charge for personal, non-commercial
flight-simulation use. Commercial use, real-world navigation, modification,
derivative works, resale, rehosting, and redistribution are prohibited unless
Sky Ning gives prior written permission.

**TaxiNow Pro is provided “AS IS” and “AS AVAILABLE”, without warranties of any
kind.**

See the [License](LICENSE), [EULA](EULA.txt), [Disclaimer](DISCLAIMER.md), and
[third-party notices](NOTICE) for the complete terms.

### Uninstallation

Use **Windows Settings → Apps → Installed apps → TaxiNow Pro → Uninstall**, or the
TaxiNow Pro uninstall shortcut in the Start menu.

Uninstallation always removes the application. It then asks whether to retain
downloaded maps and user data. Choose **Yes** (recommended for upgrades) to
reuse maps and settings after reinstalling, or **No** to permanently delete
TaxiNow Pro databases, caches, settings, logs, and downloaded assets.

### Troubleshooting

- **Already running:** restore TaxiNow Pro from the notification-area icon, or
  right-click it and select **Quit**.
- **Blank window:** close TaxiNow Pro, run setup again to repair required
  components, restart Windows, and try again.
- **Red simulator status:** start MSFS 2024, MSFS 2020 or X-Plane 12 and load a flight, then restart
  TaxiNow Pro if necessary.
- **Orange simulator status:** finish loading the flight, remain on the ground,
  wait briefly, and use position refresh.
- **Missing aircraft icon:** select the correct airport and confirm the
  synchronization status is green.
- **VATSIM traffic refreshes only occasionally:** the official VATSIM
  network-data feed is regenerated about every 15 seconds. TaxiNow Pro follows
  that cadence and shares one PC-side cache between desktop and iPad views.
- **BeyondATC labels are missing or incorrect:** confirm BeyondATC has injected
  traffic into the current MSFS flight, then enable only **Show BeyondATC
  Traffic** in TaxiNow Pro. SimConnect does not identify which application injected
  an AI aircraft, so other MSFS AI traffic should be disabled.
- **SayIntentions traffic shows no aircraft:** confirm SayIntentions is running
  an active flight with AI traffic enabled, then select **Show SayIntentions
  Traffic**. TaxiNow Pro obtains the active flight ID locally and uses the official
  Tracker for callsigns; VATSIM and BeyondATC display will turn off automatically.
- **Slow map acquisition:** use 1 batch worker and retry later. Public OSM
  server-side processing is often slower when several requests compete for
  the same per-user slots. OSM normally takes 5–30 seconds; busy airports can take
  30–90 seconds. TaxiNow Pro marks an unchanged request as stalled after 45
  seconds and stops waiting for OSM after 120 seconds.

- **Stalled airport download:** use the fallback-source button in Maps & storage; fallback maps may contain less detail.
- **Old update installers:** Settings → Open update installer folder opens the folder for manual cleanup; wait until downloading or installation has finished.

### Airport-map limitations

TaxiNow Pro combines several imperfect datasets and cannot guarantee correct,
complete, or current drawing for every airport worldwide. A building-footprint
source may have no terminal name, while an aviation source may have a
“Terminal X” point but no usable outline. TaxiNow Pro matches trustworthy labels,
gate clusters, and nearby geometry automatically, but does not invent terminal
numbers and does not maintain manual per-airport drawing corrections.

---

## 中文

### 简介

TaxiNow Pro 是一款运行于本地 Windows 电脑的软件。V2.0 将机场地面地图、2D/3D
地球航线、SimBrief 导入和垂直航线剖面整合到同一工作区，通过 SimConnect 连接
MSFS，或通过本机 UDP DataRef 接口连接 X-Plane 12，显示飞机实时位置、航向和高度。

TaxiNow Pro 仅限个人模拟飞行使用，严禁用于真实飞行、真实导航、飞行计划或运行
训练。

### 模拟器兼容性

- **Microsoft Flight Simulator 2024：**已经测试并支持
- **Microsoft Flight Simulator 2020：**已经测试并支持
- **X-Plane 12：**支持本机 UDP DataRef 遥测，默认端口 49000；与 TaxiNow Pro 在同一电脑运行

### 主要功能

- 默认打开 2D/3D 地球航线工作区，提供正北指南针
- SimBrief 导入航路点、机型及计划高度，用户名在浏览器中自动保存
- 全屏垂直剖面展示地形、计划高度、可用高度限制和实时 MSL/AGL；估算路径明确标注，过期遥测及时清除
- 根据飞行计划下载出发/到达机场地图，落地后切换目的地地面地图
- VATSIM 管制、天气雷达、GNSS 干扰及地形叠加图层
- 地面视图持续跟随飞机位置和航向，航线视图支持持续飞机跟随
- 下载卡住时手动尝试 X-Plane Scenery Gateway，最终以 OurAirports 跑道数据后备；数据细节因来源而异
- 紧凑顶部及底部、ICAO 机场选择器、统一飞行计划/航路信息面板和地图按钮尺寸
- 完整界面亮暗主题及可读性改进，桌面 WebView2 使用 sRGB 渲染
- 应用内问题表单、明确更新检查状态及手动打开更新安装包目录
- 详细的机场地面地图
- 显示跑道、滑行道、机坪、航站楼、停机位及相关编号
- 通过 MSFS SimConnect 或 X-Plane 12 UDP DataRef 显示飞机位置和航向
- 长途飞行中出现正常遥测间隔后可自动恢复位置跟踪，无需重启 TaxiNow Pro
- 落地后自动切换到飞机当前所在机场；地图未下载时自动打开机场选择器并提示下载
- 可选显示官方公开网络数据源中的附近 VATSIM 交通；其他飞机使用带呼号的
  橘色图标，本机 MSFS 飞机保持青色
- 可选显示由 BeyondATC 注入 MSFS 的附近交通；TaxiNow Pro 通过 SimConnect 读取，
  并使用带航向和呼号标签的紫色飞机图标显示
- 新增独立的 SayIntentions 交通功能：读取当前本地航班 ID，通过官方
  SayIntentions Tracker 保留真实呼号，并与 SimConnect 实时位置匹配
- VATSIM、BeyondATC 与 SayIntentions 三种交通来源互斥；选择一种会自动关闭
  并清除另外两种，避免重复显示
- 地图图层就绪后立即可靠同步飞机图标，飞机静止或切换机场后同样有效
- 桌面端与 iPad 使用相同的 SVG 飞机图标；iPad 可立即显示，图标尺寸统一为 32.4 px
- 滑行道灰色铺装及其边缘加宽 20%，提高地面地图辨识度
- 模拟器连接及位置同步状态
- 手动刷新飞机位置
- 英文、简体中文、繁体中文、日语、法语、德语和韩语界面
- 设置菜单包含语言选择及可选的**保持窗口始终可见**功能
- 页头会根据实际文字碰撞自动折叠，避免窄窗口下重叠或过早隐藏
- 自动规划滑行路线并提供多条路线选择
- 在地图上以蓝色高亮路线，提供实时进度与转向提示
- 支持实验性的自定义滑行路线输入，并按相邻关系筛选可选滑行道；可使用
  逗号、空格或混合方式分隔
- 支持通过右键或触摸长按地图指定滑行起点和目的地
- 新增深色与浅色外观，以及一键太阳/月亮切换按钮
- 新增详细的跑道入口、瞄准点、接地区、跑道号码及航向图形
- 新增自动检查更新、官方渠道下载及应用内下载安装选项
- 启动时恢复上次成功显示且仍已安装的机场
- 新增机头朝上导航锁定，并将飞机自动保持在画面下方中央
- 机场搜索及 ICAO 快速地图获取
- 按 ICAO、国家/地区或省/州获取地图
- 支持 1、2、4、8、16 个批量任务工作线程；公共 OSM 推荐使用 1
- 存在官方地区地图包时支持校验、断点续传，并对未包含的机场自动按需回退
- 显示进度、速度、已用时间和预计剩余时间
- 中国省级行政区与日本都道府县使用可读名称显示
- 按“国家/地区 → 省/州 → 机场”管理地图库
- 显示资源占用、剩余空间并支持自定义保存位置
- 可选的同一可信局域网内其他设备访问
- 默认最小化到任务栏，可在设置中启用并保存**最小化到托盘**

TaxiNow Pro 会优先使用连续的 OSM 及可用 FAA 建筑轮廓，不再让 X-Plane 模块化外墙
片段覆盖权威航站楼图形。预处理地图包还可严格筛选 Overture 与 Microsoft 全球
建筑轮廓；完整父建筑会压制重叠的建筑分块，可信的邻近航站楼/指廊名称会自动
传递到已接受的无名轮廓，从而尽量改善航站楼支离破碎、形状或标注缺失的问题。

TaxiNow Pro 现已包含可重复的全球预处理流水线，可按照可用的省/州提取包拆分大型国家，
并生成可断点续传、可并行且经过校验的有限大小分片。某个国家的地图包上传至官方
索引后，按国家下载才会进入高速路径；尚未发布地图包的国家仍使用较慢的按需回退。

滑行路线由通用寻路算法生成，仅供模拟飞行参考，可能不会考虑 ATC 指令、滑行道方向、
机翼跨度限制、临时关闭或真实运行程序。使用前请自行检查；自动路线不合适时可输入
自定义滑行路线。

### 安装方法

1. 关闭 TaxiNow Pro。V2.0 可以直接覆盖安装旧版本；如果希望先卸载，卸载器询问是否
   保留地图和用户数据时请选择 **“是”**，新版安装后即可继续使用。
2. 从上述两个官方渠道之一下载安装程序。
3. 运行 `TaxiNow-Pro-V2.0-Build-206-Setup.exe`。
4. 阅读并同意最终用户许可协议。
5. 完成安装并启动 TaxiNow Pro。

TaxiNow Pro 按当前 Windows 用户安装，通常不需要管理员权限。必要的 Windows
组件会由安装程序自动检测或安装。

### 使用方法

1. 在同一电脑启动 TaxiNow Pro 和 MSFS 2020/2024 或 X-Plane 12。
2. 默认显示地球航线。打开**飞行计划 → 导入**，载入 SimBrief 计划。
3. **航路信息**查看航路点，**垂直 / Profile**查看垂直航线剖面。
4. 通过 ICAO 选择机场，地图缺失时先下载，切换到**地面**查看滑行地图。
5. 模拟器同步为绿色后，可按需要开启飞机跟随。
6. 在**地图管理 / Maps & storage**管理下载及存储；机场下载卡住或失败时可尝试后备资源。

Portable 用户解压 ZIP 后运行 `TaxiNow.App.exe`，需要 WebView2 Runtime。
便携版不创建快捷方式或进行安装器前置检查，地图仍保存在配置的用户数据目录。

### 其他设备访问

TaxiNow Pro 可以在同一可信私人局域网中的其他设备上显示当前地图。请使用软件
顶部显示的局域网地址，并保持电脑端运行。支持基线为 Android 10+ 与 Firefox 114+，
或 iOS/iPadOS 16.4+ 与 Safari；浏览器及 GPU 需支持 WebGL 2.0。

该本地辅助功能使用不带身份验证的 HTTP。请勿在路由器中开放其端口，也不要
在公共或不可信网络中使用。如果 Windows 防火墙询问权限，请仅允许专用网络。

### 安全与隐私

TaxiNow Pro 不要求注册账号，不包含广告，不包含内置行为分析，也不会自动上传
崩溃报告。地图、设置、日志、缓存和资源数据库均保存在本机。

为了显示地面位置，TaxiNow Pro 仅从模拟器读取纬度、经度、真航向、是否在地面及
地速以及可用的海拔/离地高度。TaxiNow Pro 不会主动将实时飞机位置发送给地图数据提供方。

可选的 VATSIM 交通功能默认关闭。启用后，TaxiNow Pro 的电脑端服务会请求 VATSIM
官方公开网络数据源，缓存约 15 秒，并仅向地图提供显示附近飞机所需的字段。
TaxiNow Pro 不会把本机模拟器遥测发送给 VATSIM。

可选的 BeyondATC 与 SayIntentions 交通功能同样默认关闭。BeyondATC 交通直接通过
SimConnect 读取已经注入 MSFS 的非本机飞机。SayIntentions 模式仅从官方文档所述的
本地 SAPI 响应读取当前 `flight_id`，再通过官方 SayIntentions Tracker 获取该航班的
交通，以便将真实呼号与模拟器实时位置匹配。TaxiNow Pro 不会公开或记录 SayIntentions
API Key、邮箱地址或其他账户字段。VATSIM、BeyondATC 与 SayIntentions 一次只能
显示一种交通来源。

TaxiNow Pro 源代码不公开。符合条件的独立安全或隐私专家，可以仅以核验 TaxiNow Pro
安全与隐私行为为目的，向 Sky Ning 申请有限审查访问。是否批准及具体审查条件
由开发者决定。审查权限不包含复制、修改、编译、公开、披露或再发布源代码的
授权。

### 许可与免责声明

TaxiNow Pro 是受版权保护的软件，不是开源或公有领域软件。软件完全免费，仅供个人、
非商业模拟飞行使用。未经 Sky Ning 事先书面授权，禁止商业使用、真实飞行导航、
修改、二次创作、倒卖、重新托管或重新分发。

**TaxiNow Pro 按“现状”和“可用状态”提供，不作任何形式的担保。**

完整条款请参阅[许可协议](LICENSE)、[最终用户许可协议](EULA.txt)、
[免责声明](DISCLAIMER.md)和[第三方声明](NOTICE)。

### 卸载方法

通过 **Windows 设置 → 应用 → 已安装的应用 → TaxiNow Pro → 卸载**，或使用开始
菜单中的 TaxiNow Pro 卸载快捷方式。

卸载会删除 TaxiNow Pro 程序，并询问是否保留已下载地图和用户数据。升级时建议选择
**“是”**，重新安装后可继续使用地图与设置；选择 **“否”** 才会永久删除数据库、
缓存、设置、日志和已下载资源。

### 常见问题

- **提示已经运行：**从系统托盘恢复 TaxiNow Pro，或右键选择 **Quit**。
- **窗口空白：**退出 TaxiNow Pro，重新运行安装程序修复必要组件，重启 Windows
  后再次尝试。
- **模拟器状态为红色：**启动 MSFS 2024、MSFS 2020 或 X-Plane 12 并进入飞行，必要时重新启动 TaxiNow Pro。
- **模拟器状态为橙色：**等待飞行完全加载并保持飞机在地面，然后刷新位置。
- **没有飞机图标：**选择正确机场并确认同步状态为绿色。
- **VATSIM 交通不是持续刷新：**VATSIM 官方网络数据源约每 15 秒生成一次。
  TaxiNow Pro 遵循这一频率，并让桌面端与 iPad 共用电脑端缓存。
- **BeyondATC 呼号缺失或不正确：**确认 BeyondATC 已向当前 MSFS 飞行注入交通，
  并只启用 TaxiNow Pro 的**显示 BeyondATC 交通**。SimConnect 无法识别 AI 飞机由哪个
  程序注入，因此应关闭其他 MSFS AI 交通来源。
- **SayIntentions 没有显示交通：**确认 SayIntentions 正在运行有效航班且已开启
  AI 交通，然后选择**显示 SayIntentions 交通**。TaxiNow Pro 会在本地取得当前航班 ID，
  并使用官方 Tracker 获取呼号；VATSIM 与 BeyondATC 显示会自动关闭。
- **地图获取较慢：**选择 1 个批量任务工作线程并稍后重试。公共 OSM
  会按用户分配请求槽位，同时发送更多请求往往反而更慢。OSM 通常需要
  5–30 秒，繁忙或复杂机场可能需要 30–90 秒。连续 45
  秒无有效进展时 TaxiNow Pro 会标记为疑似卡住，等待 OSM 的最长时间为
  120 秒。中国大陆用户如果持续遇到连接重置或超时（部分中国电信线路
  尤其明显），可更换网络，或在遵守当地法律及服务条款的前提下使用可靠的
  VPN/网络加速服务后重试。

- **机场下载疑似卡住：**在地图管理中尝试后备资源，后备地图的细节可能较少。
- **清理旧更新包：**设置 → 打开更新安装包目录，下载或安装结束后自行清理，程序不会自动删除文件。

### 机场地图技术限制

TaxiNow Pro 融合多种并不完美的数据源，无法保证全球每一座机场的绘制都正确、完整或
保持最新。建筑轮廓数据可能没有航站楼名称，航空数据也可能只有“Terminal X”
名称点而没有可用轮廓。TaxiNow Pro 会自动匹配可信名称、登机口簇与邻近图形，但不会
凭空编造航站楼编号，也不维护逐机场的人工绘图修正。

---

## Acknowledgements and credits / 致谢与 Credits

Special thanks to **睡务局局长 ([@stewieqi-del](https://github.com/stewieqi-del))** for contributions to V2.0.<br>
特别感谢 **睡务局局长（[@stewieqi-del](https://github.com/stewieqi-del)）** 对 V2.0 的贡献。

TaxiNow Pro thanks the contributors and maintainers of the following data sources,
projects, and technologies. TaxiNow Pro 感谢以下数据来源、项目、技术的贡献者与维护者：

- [OpenStreetMap contributors](https://www.openstreetmap.org/copyright) —
  airport map data under the ODbL.<br>
  OpenStreetMap 贡献者——依据 ODbL 提供机场地图数据。
- [OurAirports](https://ourairports.com/data/) — public-domain airport and
  runway datasets.<br>
  OurAirports——提供公有领域机场及跑道数据集。
- [FAA Airport Mapping Open Data](https://adds-faa.opendata.arcgis.com/) —
  authoritative US airport geometry where available.<br>
  FAA Airport Mapping Open Data——在有覆盖时提供美国机场权威图形。
- [Geofabrik](https://download.geofabrik.de/) — regional OpenStreetMap extracts
  for preprocessing.<br>
  Geofabrik——提供预处理所用的地区 OpenStreetMap 提取数据。
- [Overture Maps Foundation](https://overturemaps.org/) — supplemental open
  building footprints.<br>
  Overture Maps Foundation——提供辅助开放建筑轮廓。
- [Microsoft Global ML Building Footprints](https://github.com/microsoft/GlobalMLBuildingFootprints)
  — supplemental global building geometry.<br>
  Microsoft Global ML Building Footprints——提供辅助全球建筑图形。
- [X-Plane Scenery Gateway](https://gateway.x-plane.com/) — fallback airport
  layout data.<br>
  X-Plane Scenery Gateway——提供后备机场布局数据。
- [SkyCharts](https://github.com/skylarkning/SkyCharts) — airport-map visual
  conventions and rendering reference.<br>
  SkyCharts——提供机场地图视觉规范与绘制方式参考。
- [MapLibre GL JS](https://github.com/maplibre/maplibre-gl-js) — interactive
  map rendering.<br>
  MapLibre GL JS——提供交互式地图绘制能力。
- [Microsoft .NET](https://github.com/dotnet/runtime),
  [ASP.NET Core SignalR](https://github.com/dotnet/aspnetcore),
  [WebView2](https://developer.microsoft.com/microsoft-edge/webview2/), and the
  Microsoft Flight Simulator SimConnect SDK — application runtime, live
  updates, Windows interface, and simulator integration.<br>
  Microsoft .NET、ASP.NET Core SignalR、WebView2 及 Microsoft Flight
  Simulator SimConnect SDK——用于程序运行、实时更新、Windows 界面及模拟器连接。
- [SQLite](https://www.sqlite.org/) and
  [SQLitePCLRaw](https://github.com/ericsink/SQLitePCL.raw) — local asset
  storage.<br>
  SQLite 与 SQLitePCLRaw——用于本地资源存储。
- [PyInstaller](https://pyinstaller.org/) and
  [Inno Setup](https://jrsoftware.org/isinfo.php) — Windows packaging and
  installation.<br>
  PyInstaller 与 Inno Setup——用于 Windows 打包及安装程序制作。

Each third-party component or dataset remains subject to its own license and
terms. See [NOTICE](NOTICE) for the formal data notices.<br>
各第三方组件及数据集仍分别受其自身许可证及条款约束。正式数据声明请参阅
[NOTICE](NOTICE)。

---

Developed by Sky Ning (`skylarkning`).<br>
TaxiNow Pro 由 Sky Ning（`skylarkning`）开发。
