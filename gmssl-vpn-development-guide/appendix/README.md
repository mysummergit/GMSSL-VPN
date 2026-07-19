# 附录 A：索引与配套资料

附录保存需要查询、但不适合打断正文阅读主线的内容。

本版提供标准索引、开源能力索引和可直接用于开发与验证的配套资料。

## A.1 标准索引

| 标准章节 | 在指南中的主要位置 | 配套资料 |
|---|---|---|
| 第 5 章：密码算法与密钥 | 第 1、2、3、4 章 | [密码套件覆盖矩阵](cipher-suite-matrix.md)、符合性追踪矩阵 |
| 第 6 章：协议 | 第 1、2、3、4 章 | 密码套件覆盖矩阵、符合性追踪矩阵 |
| 第 7 章：产品要求 | 第 2、3、4 章 | 功能要求清单、管理与安全能力清单 |
| 第 8 章：检测要求 | 第 4 章 | [测试证据记录模板](test-evidence-template.md)、[符合性追踪矩阵](standard-compliance-matrix.md) |
| 第 9 章：判定规则 | 第 4 章 | 符合性追踪矩阵、发布门禁结论 |

## A.2 开源能力索引

| 来源 | 需要索引的内容 | 用途 |
|---|---|---|
| OpenVPN | TUN/TAP、Socket、事件循环、路由、配置、日志、多客户端管理 | 提取 VPN 工程底座 |
| GmSSL | SM2、SM3、SM4、X.509、双证书、TLCP、密码设备接口 | 建立国密和 TLCP 基础 |

这里的索引只说明开发时应查找什么，不表示相关开源代码可以原样进入标准通信路径。

## A.3 配套附录

| 文件 | 内容 |
|---|---|
| [cipher-suite-matrix.md](cipher-suite-matrix.md) | GM/T 0024-2023 表 2 的 12 个密码套件覆盖清单 |
| [terms.md](terms.md) | TLCP、双证书、保护域和接入会话等核心术语 |
| [standard-compliance-matrix.md](standard-compliance-matrix.md) | 标准要求到设计、实现和测试证据的追踪矩阵 |
| [test-evidence-template.md](test-evidence-template.md) | 协议、功能、安全和性能证据记录模板 |
| [sources-and-license-boundary.md](sources-and-license-boundary.md) | 标准、OpenVPN、GmSSL 与指南之间的来源和许可边界 |
