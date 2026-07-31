# TaxiNow regional map packs / TaxiNow 地区地图包

TaxiNow regional map packs are official, versioned offline-map bundles
published by **skylarkning**. The application downloads them directly from the
TaxiNow-Release GitHub release assets, verifies SHA-256 checksums, and falls
back to on-demand map sources for airports that are not yet packaged.

TaxiNow 地区地图包是由 **skylarkning** 发布的官方版本化离线地图包。应用会从
TaxiNow-Release 的 GitHub Release 资产中直接下载，校验 SHA-256；尚未包含在地图包
中的机场会自动回退到按需数据源。

The initial Beta 4 pilot covers:

- `CA-BC`: CYVR
- `US-DC`: KDCA

These pilot packs validate the download/import architecture and the updated
terminal-geometry fusion rules. They are not yet complete province/state
collections. Larger Geofabrik-based packs will be added incrementally.

首批 Beta 4 试点地图包包括：

- `CA-BC`：CYVR
- `US-DC`：KDCA

试点包用于验证下载/导入架构及新版航站楼图形融合规则，目前并非完整省/州机场合集。
后续将逐步加入基于 Geofabrik 地区数据构建的完整地图包。

Map data remains subject to the source licenses and attribution shown by
TaxiNow, including OpenStreetMap contributors under ODbL. See the repository
[NOTICE](../NOTICE) for third-party credits.
