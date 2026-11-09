# 年检与专项检查证据包示例

## 典型场景

年度检查要求提供师资、收费、课程、投诉、退费和安全材料，多个校区版本混乱。

## 具体示例

Agent 输出按检查要点组织的证据包，并把“缺签批”“两个版本价格表并存”列为重大缺口，不伪造或生成真实签批。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "inspection_notice": "检查通知或要求已核对（脱敏示例）",
  "campus_scope": [
    {}
  ],
  "evidence_inventory": [
    {}
  ],
  "responsible_roles": [
    {}
  ],
  "deadline": "2026-11-10",
  "resume_mode": "new"
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出检查证据目录、材料索引、缺口表等核心成果。
5. 由校区负责人/材料责任部门确认真实材料、原件、签批、责任人与对外提交版本后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。
