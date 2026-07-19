# 附录 D：GM/T 0024-2023 密码套件覆盖矩阵

> 本附录列出 GM/T 0024-2023 表 2 定义的 12 个密码套件，用于建立实现、互操作和测试覆盖关系。

## D.1 标准套件清单

| 密码套件 | 密钥交换 | 加密 | 校验 | 编码值 |
|---|---|---|---|---|
| `ECDHE_SM4_CBC_SM3` | ECDHE（SM2） | SM4-CBC | SM3 | `{0xE0, 0x11}` |
| `ECDHE_SM4_GCM_SM3` | ECDHE（SM2） | SM4-GCM | SM3 | `{0xE0, 0x51}` |
| `ECC_SM4_CBC_SM3` | ECC（SM2） | SM4-CBC | SM3 | `{0xE0, 0x13}` |
| `ECC_SM4_GCM_SM3` | ECC（SM2） | SM4-GCM | SM3 | `{0xE0, 0x53}` |
| `IBSDH_SM4_CBC_SM3` | IBSDH（SM9） | SM4-CBC | SM3 | `{0xE0, 0x15}` |
| `IBSDH_SM4_GCM_SM3` | IBSDH（SM9） | SM4-GCM | SM3 | `{0xE0, 0x55}` |
| `IBC_SM4_CBC_SM3` | IBC（SM9） | SM4-CBC | SM3 | `{0xE0, 0x17}` |
| `IBC_SM4_GCM_SM3` | IBC（SM9） | SM4-GCM | SM3 | `{0xE0, 0x57}` |
| `RSA_SM4_CBC_SM3` | RSA | SM4-CBC | SM3 | `{0xE0, 0x19}` |
| `RSA_SM4_GCM_SM3` | RSA | SM4-GCM | SM3 | `{0xE0, 0x59}` |
| `RSA_SM4_CBC_SHA256` | RSA | SM4-CBC | SHA-256 | `{0xE0, 0x1C}` |
| `RSA_SM4_GCM_SHA256` | RSA | SM4-GCM | SHA-256 | `{0xE0, 0x5A}` |

## D.2 实现覆盖表

实现时为每个套件填写同一组结果：

| 密码套件 | 客户端 | 服务端 | 软件后端 | 产品密码部件 | 正常协商 | 互操作 | 负向测试 | 证据编号 |
|---|---|---|---|---|---|---|---|---|
| 待填写 | 未开始 | 未开始 | 未开始 | 未开始 | 未开始 | 未开始 | 未开始 | 待填写 |

覆盖矩阵至少验证：

1. 客户端按优先级发送套件列表，服务端只选择双方共同支持的标准套件；
2. 无共同套件时返回握手失败报警，不静默降级到非标准协议或套件；
3. CBC 与 GCM 分别验证记录保护、篡改拒绝、长度边界和错误状态清理；
4. ECC/ECDHE 使用 SM2，IBC/IBSDH 使用 SM9，证书或标识参数与套件一致；
5. 每个“已支持”结论都能关联到具体代码基线、密码后端和测试证据。
