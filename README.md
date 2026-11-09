# 年检与专项检查证据包

按检查主题建立证据目录，逐项核验制度、记录、资质、合同、财务与整改闭环，编排补证任务。

## 适用用户

校长、行政主管、合规负责人、财务/教务协作人员

## 主要输出

- 检查证据目录
- 材料索引
- 缺口表
- 责任人/截止时间
- 抽查问题
- 整改闭环
- 提交版目录

## 安装

将Agent目录按平台要求导入，并保留`.codebuddy-plugin/plugin.json`、`agents/`、`skills/`与`avatars/`的相对结构。

本地验证：

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 使用

1. 阅读`USAGE.md`。
2. 按`contract/input.schema.json`准备输入。
3. 调用产品或Agent完成专业处理。
4. 使用`scripts/validate_output.js`检查成果。
5. 高风险结论交由校区负责人/材料责任部门确认。

## 边界

- 不使用外部收费API。
- 不依赖其他产品完成核心任务。
- 不自动执行正式审批、退款、人员处罚或系统变更。
- 客户可见内容不包含公司品牌推广或内部研发资料。

## 状态

- 版本：`1.0.0`
- 本地契约与自动化测试：见`test-results/`
- 生成式模型运行：`MODEL_RUNTIME_NOT_VERIFIED`
- WorkBuddy安装、调用、审核、上架：`NOT_EXECUTED`
- 安装包：`dist/edu-education-inspection-evidence-agent-v1.0.0.zip`

## 许可证

Apache-2.0。详见`LICENSE`。
