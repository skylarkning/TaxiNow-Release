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
