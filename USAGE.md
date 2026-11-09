# 使用说明

## 适用任务

年度检查要求提供师资、收费、课程、投诉、退费和安全材料，多个校区版本混乱。

## 准备输入

检查通知/要求、校区信息、现有制度与记录、资质、合同、财务与教务样本、材料责任人、截止日期。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 解析检查要求
2. 建立证据树
3. 盘点现有材料
4. 核验版本与签批
5. 生成补证任务
6. 进行抽样模拟
7. 形成提交包索引

## 校验命令

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 状态使用

- `completed`：核心成果完整。
- `completed_with_limits`：只完成可验证部分，并说明受阻范围。
- `needs_input`：缺少关键输入。
- `needs_confirmation`：资料冲突或需人工确认。
- `failed`：工具或计算失败，提供恢复动作。

## 人工确认

校区负责人/材料责任部门复核真实材料、原件、签批、责任人与对外提交版本后，成果才可进入正式业务使用。
