# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `inspection_notice` | 检查通知或要求 | string | 是 |
| `campus_scope` | 检查校区范围 | array | 是 |
| `evidence_inventory` | 现有证据材料清单 | array | 是 |
| `responsible_roles` | 责任角色 | array | 是 |
| `deadline` | 提交截止日期 | string | 是 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `检查证据目录`：结构化条目数组，不允许空壳或占位文本。
- `材料索引`：结构化条目数组，不允许空壳或占位文本。
- `缺口表`：结构化条目数组，不允许空壳或占位文本。
- `责任人/截止时间`：结构化条目数组，不允许空壳或占位文本。
- `抽查问题`：结构化条目数组，不允许空壳或占位文本。
- `整改闭环`：结构化条目数组，不允许空壳或占位文本。
- `提交版目录`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
