# 直连

## 前言

本项目的直连规则由《规则生成器》自动整合与去重。

分流规则是互联网公共服务的域名和IP地址汇总，所有数据均收集自开源项目，仅为解决引用过多外部资源引起的规则重复问题，不代表我们支持或使用这些服务。

请通过我国(中华人民共和国)合法的互联网出入口信道访问规则中的地址，并确保在使用过程中符合相关法律法规。

## 规则统计

总计规则：2584 条。

各类型规则统计：

| 类型 | 数量(条) |
| ---- | ---- |
| DOMAIN-SUFFIX | 2579 |
| DOMAIN-KEYWORD | 1 |
| DOMAIN | 4 |
## 配置说明

实时版：程序定时更新，更新频率高，能尽快同步数据源变化，适合希望尝鲜的人。

稳定版：不定时手动更新，更新频率低，适合不希望规则频繁变化的人。

### Clash 
实时版：

https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Direct/Direct.yaml
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Direct/Direct_Domain.yaml
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Direct/Direct_Classical.yaml


稳定版：

https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/release/rule/Clash/Direct/Direct.yaml
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/release/rule/Clash/Direct/Direct_Domain.yaml
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/release/rule/Clash/Direct/Direct_Classical.yaml


如果稳定版无法访问 ，可能是尚未从实时版的分支合并，建议您先使用实时版，或等待下次稳定版分支合并。

### 特别说明

Direct.yaml 请使用 behavior: "classical"。

Direct_Classical.yaml 请使用 behavior: "classical"。

Direct_Domain.yaml 请使用 behavior: "domain"。

Direct_Classical.yaml 可以单独使用，其他规则必须同时使用。

文件名带Resolve，指对于IP-CIDR、IP-CIDR6的规则，不增加no-resolve，其余与上述相同。

#### 最简单的用法

使用 Direct_Classical.yaml。

## 子规则/排除规则

当前分流规则，已包含以下子规则：

- WhiteList

除非特殊需求，否则不建议重复引用。

当前分流规则，已排除以下规则：

- AppleProxy

- China

- ChinaIP

- ChinaIPs

- ChinaIPsBGP

- ChinaMedia

- ChinaMobile

- ChinaNews

- ChinaTelecom

- ChinaTest

- ChinaUnicom

- Proxy

## 数据来源

本项目的直连复写规则的数据来自以下链接，通常已涵盖所有数据来源的复写规则。

如果你正在使用这些复写规则，建议不要与本项目的直连复写规则混合使用，以免造成规则重复。

- https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/UnBan.list
- https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/Unbreak.list
- https://raw.githubusercontent.com/DivineEngine/Profiles/master/Surge/Ruleset/Unbreak.list
- https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/direct.txt
- https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/source/rule/WhiteList/WhiteList.list
- https://raw.githubusercontent.com/sve1r/Rules-For-Quantumult-X/develop/Rules/Services/Unbreak.list


感谢以上复写规则作者的辛勤付出（排名不分先后）。

## 最后

### 感谢

[@fiiir](https://github.com/fiiir) [@Tartarus2014](https://github.com/Tartarus2014) [@zjcfynn](https://github.com/zjcfynn) [@chenyiping1995](https://github.com/chenyiping1995) 

提供规则数据源及改进建议。

### 其他

请不要对外宣传本项目。