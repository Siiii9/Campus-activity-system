# 配置管理方案

## 1. 配置项识别

| 配置项ID | 文件名 | 责任人 | 说明 |
|----------|--------|--------|------|
| C-01 | 01-project-charter.md | sunbo, zhangdongze, chenjingpeng | 项目章程 |
| C-02 | 02-wbs.md | zhangdongze | WBS分解 |
| C-03 | 03-schedule.md | zhangdongze | 进度计划 |
| C-04 | 04-config-plan.md | sunbo | 配置管理 |
| C-05 | 05-summary-report.md | sunbo, zhangdongze, chenjingpeng | 总结报告 |
| C-06 | conflict.md | chenjingpeng | 冲突演练 |

## 2. 分支策略
main # 最终提交分支（受保护）
└── dev # 开发集成分支
├── feature/charter # 项目章程分支
├── feature/wbs # WBS分支
├── feature/schedule # 进度计划分支
├── feature/config # 配置管理分支
└── feature/conflict # 冲突演练分支

## 3. 分支命名规范
- `feature/xxx` - 新功能/文档开发
- `bugfix/xxx` - 问题修复

## 4. 提交规范

格式：`<类型>: <描述>`

| 类型 | 用途 | 示例 |
|------|------|------|
| docs | 文档更新       | `docs: 完成WBS三级分解` |
| chore | 初始化/配置 | `chore: 初始化目录结构` |
| fix | 错误修复          | `fix: 修正文档格式错误` |

## 5. 合并规则
1. 所有功能分支从 `dev` 创建
2. 完成后向 `dev` 发起 Pull Request
3. PR需至少1人审核
4. 由项目经理（sunbo）负责合并
5. 最终统一从 `dev` 合并到 `main`

## 6. 提交人名称规范

| 成员 | Git用户名 |
|------|-----------|
| sunbo | sunbo |
| zhangdongze | zhangdongze |
| chenjingpeng | chenjingpeng |

## 7. 版本标记
- 实验完成：`git tag -a v1.0-final -m "实验最终提交"`