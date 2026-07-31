# TaxiNow V1.0 Beta 6 — Build 103

Release date: July 31, 2026

## Upgrade instructions

1. Close TaxiNow and uninstall the previous version before installing Beta 6.
2. When the uninstaller asks about downloaded maps and user data, choose
   **Yes / Keep data** so your existing airport assets remain available.
3. Install `TaxiNow-V1.0-Beta-6-Build-103-Setup.exe`.

Existing airport maps do not need to be downloaded again for this update.

## Changelog

- Correct runway-end designators from physical runway geometry instead of
  assuming that source references and LineString coordinates use the same
  order. This fixes reversed labels at ZBAA, ZGGG, and other airports while
  preserving L/C/R parallel-runway suffixes.
- Apply the correction in both the MapLibre renderer and the compatibility
  fallback renderer. Existing downloaded airport maps do not need to be
  downloaded again.
- Add regression coverage for north/south, east/west, correctly ordered,
  reversed, and parallel runways.
- Add bilingual FAQ guidance for X-Plane fallback terminal limitations,
  retrying an airport through OSM, and position refresh after simulator warp.
- Add official Microsoft Flight Simulator 2020 ground-position support without
  changing the existing MSFS 2024 telemetry path. TaxiNow now detects either
  simulator, reports the accepted edition through the API, and keeps 2024 as
  the deterministic preference if both editions are running.
- Verify MSFS 2020 live at CYYZ Gate B19: SimConnect returned latitude,
  longitude, true heading, on-ground state, and ground speed; normal tracking
  and force refresh both passed.
- Expand the bilingual About-page FAQ with supported simulators, the current
  X-Plane support position, issue-reporting guidance, TaxiNow's permanent-free
  intent, privacy and network behavior, independent security review, and the
  no-donations policy.

---

# TaxiNow V1.0 Beta 6 — 内部版本 103

发布日期：2026 年 7 月 31 日

## 升级说明

1. 安装 Beta 6 前，请先关闭 TaxiNow 并卸载旧版本。
2. 卸载器询问是否保留已下载地图和用户数据时，请选择
   **“是 / 保留数据”**，以继续使用已有机场资源。
3. 安装 `TaxiNow-V1.0-Beta-6-Build-103-Setup.exe`。

本次更新不需要重新下载已有机场地图。

## 更新日志

- 根据跑道真实几何方向匹配两端编号，不再假设数据源中的跑道编号顺序与坐标
  顺序一致。该修复可纠正 ZBAA、ZGGG 及其他机场中颠倒的跑道编号，同时保留
  L/C/R 平行跑道后缀。
- MapLibre 主渲染和兼容备用渲染均已采用相同修复。用户不需要重新下载已有
  机场地图。
- 新增南北向、东西向、原本顺序正确、顺序颠倒以及平行跑道的回归测试。
- 新增中英双语常见问题，说明 X-Plane 后备数据的航站楼限制、如何重新尝试
  获取 OSM 数据，以及模拟器瞬移后如何刷新飞机位置。
- 新增 Microsoft Flight Simulator 2020 地面位置官方支持，不改动现有 MSFS
  2024 遥测通道。TaxiNow 现可识别两代模拟器，通过 API 报告实际连接的版本；
  如果两者同时运行，优先保持 MSFS 2024 连接。
- 已在 CYYZ B19 机位完成 MSFS 2020 实机测试：SimConnect 成功返回经纬度、
  真航向、地面状态和地速，正常跟踪和强制刷新均通过。
- 扩充“关于”页面的中英双语常见问题，新增支持平台、暂不支持 X-Plane 的
  原因、问题反馈方式、永久免费计划、隐私与联网行为、独立安全审查以及暂不
  接受捐赠等说明。

## Acknowledgements and credits / 致谢

TaxiNow thanks the contributors and maintainers of
[OpenStreetMap](https://www.openstreetmap.org/copyright),
[OurAirports](https://ourairports.com/data/),
[FAA Airport Mapping Open Data](https://adds-faa.opendata.arcgis.com/),
[Geofabrik](https://download.geofabrik.de/),
[Overture Maps](https://overturemaps.org/),
[Microsoft Global ML Building Footprints](https://github.com/microsoft/GlobalMLBuildingFootprints),
[X-Plane Scenery Gateway](https://gateway.x-plane.com/),
[SkyCharts](https://github.com/skylarkning/SkyCharts),
[MapLibre GL JS](https://github.com/maplibre/maplibre-gl-js), Microsoft .NET,
WebView2, SimConnect, SQLite, PyInstaller, and Inno Setup.

感谢以上数据源、开源项目与相关技术的贡献者和维护者。各第三方数据及组件仍受
其各自许可与使用条款约束，完整说明请参阅 [NOTICE](NOTICE)。

TaxiNow is free for personal, non-commercial flight-simulation use and is
provided **“AS IS”**, without warranties of any kind. It must not be used for
real-world navigation. / TaxiNow 完全免费，仅供个人、非商业模拟飞行使用，并按
“现状”提供，不作任何形式的担保；严禁用于真实飞行导航。
