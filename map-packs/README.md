# TaxiNow regional map packs / TaxiNow 地区地图包

TaxiNow regional map packs are official, versioned offline-map bundles
published by **skylarkning**. TaxiNow downloads a pack only when it is listed
in [`index.json`](index.json), verifies its SHA-256 checksum, and falls back to
on-demand sources when no complete pack is available.

TaxiNow 地区地图包是由 **skylarkning** 发布的官方版本化离线地图包。TaxiNow
只会下载 [`index.json`](index.json) 中列出的地图包，并验证 SHA-256 校验值；
当没有完整地图包时，软件会回退到按需数据源。

## Current availability / 当前可用情况

No regional map packs are currently published. The incomplete Beta 4 pilot
packs for `CA-BC` and `US-DC` were withdrawn because they did not meet the
required terminal-completeness standard. They must not be treated as complete
province/state packages.

目前没有已发布的地区地图包。Beta 4 的 `CA-BC` 与 `US-DC` 不完整试点包因未达到
航站楼完整性标准而被撤回，不应再被视为完整的省/州地图包。

Future packs will be listed only after the covered region and generated airport
maps pass the release quality checks.

未来的地图包仅会在覆盖范围与生成的机场地图通过发布质量检查后加入清单。

Map data remains subject to the source licenses and attribution shown by
TaxiNow, including OpenStreetMap contributors under ODbL. See the repository
[NOTICE](../NOTICE) for third-party credits.
