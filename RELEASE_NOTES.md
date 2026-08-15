# TaxiNow V1.4.1 — Build 119

Release date: August 14, 2026

## Changelog

- Removed the red runway-end capsules because available worldwide runway
  heading values are not consistently current magnetic headings. The original
  white runway numbers remain on the runway surface.
- Corrected touchdown-zone and aiming-point marking spacing so paired blocks
  retain a clear center gap and remain inside the runway edges.
- Added dark blast-pad/stopway surfaces with yellow chevron markings.
- Kept both map renderers consistent and added runway-geometry regression tests.

Close TaxiNow, then run `TaxiNow-V1.4.1-Build-119-Setup.exe`. It may be
installed over V1.4. If you uninstall first, choose to keep downloaded maps
and user data.

---

# TaxiNow V1.4.1 — 内部版本 119

发布日期：2026年8月14日

## 更新日志

- 移除跑道端红色胶囊。现有全球数据无法稳定提供准确且及时更新的磁航向，
  因此不再显示可能误导的数值；跑道表面的原有白色跑道编号继续保留。
- 修正接地区与瞄准点标线的横向间距，使成对标线之间留有清晰间隔，
  并始终位于跑道边线以内。
- 新增深色防吹坪/停止道与黄色人字形标线。
- 统一两套地图渲染器的效果，并增加跑道几何回归测试。

关闭TaxiNow后运行`TaxiNow-V1.4.1-Build-119-Setup.exe`，可覆盖安装V1.4。
如果先卸载旧版本，请选择保留已下载地图和用户数据。

## Acknowledgements and credits / 致谢

TaxiNow thanks the contributors and maintainers of OpenStreetMap, OurAirports,
FAA Airport Mapping Open Data, Geofabrik, Overture Maps, Microsoft Global ML
Building Footprints, X-Plane Scenery Gateway, SkyCharts, MapLibre GL JS,
Microsoft .NET, WebView2, SimConnect, SQLite, PyInstaller, and Inno Setup.

TaxiNow is free for personal, non-commercial flight-simulation use and is
provided **“AS IS”**, without warranties of any kind.
