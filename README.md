# Mihomo Config

*Mihomo 内核* 覆写文件。

## 简介

该项目提供了一个覆写配置文件，符合 *Mihomo 内核* 规则，可用于任何使用 *Mihomo 内核* 的代理客户端。

## 使用方式

复制 [v0.7](https://raw.githubusercontent.com/NULLX9/Mihomo-Config-Public/refs/heads/main/version/v0.7.yaml) 地址，导入到 *代理客户端* 的**覆写**选项中。<br>

## 部分链接

[Clash Verge Rev 策略组图标](https://www.clashverge.dev/guide/group_icon/group_icon.html)<br>
[Mihomo 路由规则](https://wiki.metacubex.one/config/rules/)<br>
[代理规则集](https://ruleset.zcsouls.com/)<br>
[ClashMi](https://github.com/KaringX/clashmi)<br>
[Clash Party](https://github.com/mihomo-party-org/clash-party)<br>
[Clash Verge Rev](https://github.com/clash-verge-rev/clash-verge-rev)<br>
[clash-rules](https://github.com/Loyalsoldier/clash-rules)<br>
[v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)<br>
[ios_rule_script](https://github.com/blackmatrix7/ios_rule_script)<br>
~~[GFWList](https://github.com/gfwlist/gfwlist)~~<br>
[zashboard](https://github.com/Zephyruso/zashboard)<br>

## 更新日志

- v0.1<br>
  已知问题：Google Play商店无法下载应用。

- v0.2<br>
  使用[clash-rules](https://github.com/Loyalsoldier/clash-rules)仓库4个直连规则。<br>
  已知问题：使用[clash-rules](https://github.com/Loyalsoldier/clash-rules)时规则类型应为domain。<br>

- v0.3<br>
  使用geodata-cn规则作为主要直连规则。<br>

- v0.5<br>
  添加geosite:catetory-ads-all广告拦截规则；<br>
  取消覆写dns和域名嗅探。<br>

- v0.6<br>
  添加root权限相关配置。<br>

- v0.7<br>
  **修复**：移除与 `disable-keep-alive` 冲突的无效 Keep-Alive 参数；<br>
  **修复**：微软服务规则移至 `GEOSITE,CN` 之前，防止 CDN 误判直连；<br>
  **优化**：地区 url-test 组添加 `hidden` + `no-alert`，减少界面干扰；<br>
  **优化**：`geodata-loader` 改为 `standard` 提升匹配性能；<br>
  **优化**：规则重新排序为最佳实践（广告拦截 > 应用分流 > GeoIP > GeoSite > MATCH）；<br>
  **新增**：基础 DNS 防污染配置（Fake-IP 模式）；<br>
  **新增**：域名嗅探配置（默认注释，按需启用）；<br>
  **改进**：统一注释风格、添加文件头与区块说明。<br>
