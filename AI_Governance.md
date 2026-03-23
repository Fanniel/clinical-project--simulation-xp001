# XP-001项目 AI Governance政策（2026版）

**版本**：1.0  
**起草人**：CDM学员  
**日期**：2026-03-23  
**适用范围**：本项目所有AI辅助数据管理活动（异常检测、可视化、Query生成）

## 1. 引用法规
- EMA + FDA 《Guiding Principles of Good AI Practice in Drug Development》（2026联合指南）
- ICH E6(R3) AI章节要求

## 2. 10条核心原则（本项目落地方式）
1. **人本设计**：所有AI规则必须由CDM人工审核后生效（人类监督原则）  
2. **风险导向**：优先监控高风险变量（SBP_W12主要终点、AE严重度）  
3. **数据治理**：所有输入数据来自已批准的DMP_Variables.xlsx  
4. **透明度**：AI检测逻辑公开（见build_db.py + 后续Pandas代码）  
5. **可解释性**：每条AI Query必须附“为什么触发”（Pandas规则解释）  
6. **公平性**：亚洲人群数据无偏差（已纳入RACE变量）  
7. **稳健性**：AI规则经过至少50例模拟数据测试  
8. **安全性**：AI输出不直接修改CRF，必须人工确认  
9. **责任追溯**：所有AI活动记录在TMF（GitHub commit）  
10. **持续监控**：每周review AI检测准确率（步骤4中执行）

## 3. 本项目AI应用声明
- 当前阶段：规则-based AI（Pandas简单异常检测）  
- 未来可升级：机器学习模型（需额外GCP验证）  
- 审批状态：Pending Sponsor签字

**审批页**：Sponsor签字日期：________
