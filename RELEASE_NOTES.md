# TaxiNow V1.2 — Build 111

Release date: August 6, 2026

TaxiNow V1.2 supports Microsoft Flight Simulator 2020 and 2024 on Windows x64.

## Changelog

- Added complete Traditional Chinese and Japanese interface translations.
- TaxiNow now opens the last successfully displayed airport when it is still
  installed, instead of always preferring CYYZ.
- Added an optional heading-up map lock. It keeps the aircraft heading at the
  top and follows the aircraft from the lower center, while preserving the
  existing free-rotation and north-reset controls.
- Improved arrival taxi routing with aircraft-heading-aware start snapping,
  rejection of reverse runway exits, and prevention of near-180-degree ground
  reversals.
- Rebalanced route scoring so main taxiways remain preferred without allowing
  a clearly longer loop to beat a practical direct connection.

Automatic routes are generic simulation guidance and may not reflect ATC
instructions, taxiway restrictions, aircraft limits, or real-world procedures.
TaxiNow must not be used for real-world navigation.

## Upgrade

Close TaxiNow, then run `TaxiNow-V1.2-Build-111-Setup.exe`. You may install it
over an earlier version. If you uninstall first, choose **Yes / Keep data** to
retain downloaded airport maps.

---

# TaxiNow V1.2 — 内部版本 111

发布日期：2026年8月6日

TaxiNow V1.2 支持 Windows x64 上的 Microsoft Flight Simulator 2020 与 2024。

## 更新日志

- 新增完整的繁体中文和日语界面。
- 启动时优先打开上次成功显示且仍已安装的机场，不再总是优先打开 CYYZ。
- 新增机头朝上地图锁定模式：飞机保持机头朝上并位于画面下方中央，同时保留原有自由旋转和恢复朝北功能。
- 到达滑行路线现在会结合飞机实时航向选择接入点，排除反向跑道脱离，并阻止接近180°的原地掉头路线。
- 重新平衡主滑行道权重，继续优先使用主滑行道，同时避免明显绕远的路线胜过合理直达路线。

自动路线仅为通用算法生成的模拟飞行参考，可能不会反映ATC指令、滑行道限制、
机型限制或真实运行程序。严禁将TaxiNow用于真实飞行导航。

## 升级方法

关闭TaxiNow，然后运行`TaxiNow-V1.2-Build-111-Setup.exe`，可直接覆盖安装旧版本。
如先卸载旧版，请选择**“是 / 保留数据”**，以继续使用已下载的机场地图。

## Acknowledgements and credits / 致谢

TaxiNow thanks the contributors and maintainers of OpenStreetMap, OurAirports,
FAA Airport Mapping Open Data, Geofabrik, Overture Maps, Microsoft Global ML
Building Footprints, X-Plane Scenery Gateway, SkyCharts, MapLibre GL JS,
Microsoft .NET, WebView2, SimConnect, SQLite, PyInstaller, and Inno Setup.

TaxiNow is free for personal, non-commercial flight-simulation use and is
provided **“AS IS”**, without warranties of any kind.
