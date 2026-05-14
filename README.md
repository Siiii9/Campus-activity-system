# 校园活动报名与签到管理系统

## 项目背景
学校拟开发一套轻量级校园活动报名与签到管理系统，支持活动信息发布、学生报名、名单审核、二维码签到和签到统计导出。系统面向校内活动组织场景，强调流程清楚、记录完整和使用便捷。

## 项目目标
- 支持活动管理人员发布活动信息并维护报名时间、人数上限和活动地点
- 支持学生查看活动并完成在线报名
- 支持活动组织者对报名名单进行审核与查看
- 支持现场签到，并形成签到结果统计
- 支持活动结束后导出基本统计结果

## 团队成员与角色分工
| 姓名 | 角色 | 职责 |
|------|------|------|
| sunbo | 项目经理 + 配置管理员 | 仓库管理、配置管理方案、最终合并 |
| zhangdongze | 计划负责人 | WBS分解、进度计划 |
| chenjingpeng | 协作成员 | 冲突演练、协作编写 |

## 目录结构说明
Campus-activity-system/
├── README.md # 项目概况与协作约定
├── docs/ # 所有文档
│ ├── 01-project-charter.md # 项目章程
│ ├── 02-wbs.md # WBS分解文档
│ ├── 03-schedule.md # 简化进度计划
│ ├── 04-config-plan.md # 配置管理方案
│ ├── 05-summary-report.md # 总结报告
│ └── conflict.md # 冲突演练文件
├── src/ # 源代码
├── test/ # 测试代码
└── assets/ # 资源文件

## 分支说明
| 分支名 | 用途 |
|--------|------|
| main | 最终提交分支 |
| dev | 开发集成分支 |
| feature/config-plan | 配置管理方案分支（sunbo） |
| feature/plan | WBS + 进度计划分支（zhangdongze） |
| feature/conflict | 冲突演练分支（chenjingpeng） |

## 协作约定
- **提交规范**：`<类型>: <描述>`（如 `docs: 完成WBS分解`）
- **合并规则**：所有合并需通过 Pull Request，由项目经理审核
- **提交人名称**：每人使用姓名拼音（sunbo / zhangdongze / chenjingpeng）
- **版本标签**：vx.0-final