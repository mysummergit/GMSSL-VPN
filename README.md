# GMSSL-VPN

本仓库保存早期基于 OpenVPN 与 GmSSL 开展的 GMSSL VPN 研究代码，以及面向 GM/T 0024-2023 的开发指南。

## 开发指南

从这里开始阅读：

**[《基于 OpenVPN 与 GmSSL 的 GM/T 0024-2023 SSL VPN 开发指南》](gmssl-vpn-development-guide/README.md)**

指南从技术地图、总体设计、开发路线和验证方法四个层次，说明怎样形成符合 GM/T 0024-2023 目标要求的完整 SSL VPN。指南描述的是目标架构与开发方法，不表示仓库中的历史代码已经完成对应实现或通过符合性检测。

## 仓库内容

| 目录 | 内容 |
|---|---|
| `gmssl-vpn-development-guide/` | GM/T 0024-2023 SSL VPN 开发指南及配套附录 |
| `src/`、`include/` 等 | 早期 OpenVPN/GmSSL VPN 研究代码 |
| `doc/` | 工程文档目录；本地标准文件不纳入版本控制 |

## 标准与许可说明

- GM/T 0024-2023 标准原文需通过合法渠道获取，本仓库不发布标准 PDF；
- 仓库既有代码的许可与版权信息见 [COPYING](COPYING) 和 [COPYRIGHT.GPL](COPYRIGHT.GPL)；
- OpenVPN 与 GmSSL 各自保留其上游许可。复制、修改或组合分发上游代码前，应核对具体源码版本及其许可义务。
