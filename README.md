# design-methods

从语雀「大厂项目复盘知识库」2388 篇大厂设计复盘文章（42947 张配图 OCR 文字挖掘）中提炼的 **6 个设计方法 Agent Skill**，面向 [Agent Skill](https://code.claude.com/docs/en/skills) 标准格式（SKILL.md + YAML frontmatter + refs/ 结构化数据）。

每个 skill = 一类设计工作的速查手册：方法卡片含适用场景、操作步骤、关键原则、出处文章，可直接驱动 AI 助手按大厂实战方法论执行任务。

## Skills 一览

| Skill | 一句话简介 |
|---|---|
| [ux-research-playbook](ux-research-playbook/) | 大厂用户研究方法速查：体验地图、服务蓝图、用户画像、可用性测试、眼动实验、日记研究、合意性测试等 15 法 |
| [behavior-design-toolkit](behavior-design-toolkit/) | 行为设计三件套落地：福格模型 B=MAT、AIDTAS 精细化转化、认知偏差库，外加签到激励体系选型与 AB 测试验证结论 |
| [project-review-writing](project-review-writing/) | 大厂项目复盘写作模板：六段式叙事骨架（缘起-诊断-立标-破题-验证-收束），基于 13 家公司 26 篇精读复盘的结构分析 |
| [design-delivery-playbook](design-delivery-playbook/) | 设计流程与交付质量手册：全员体验走查、五节点标准流程、95% 高还原交付、印前八项检查 |
| [visual-system-playbook](visual-system-playbook/) | 视觉体系构建手册：情绪板制定风格、APP 视觉品牌定义 12 周 8 步法、设计语言 0-1 全链路、大改版视觉升级流程 |
| [efficiency-toolkit](efficiency-toolkit/) | 设计师效率工具箱：时间块规划、任务池 ROI、工程化设计、流程自动化、审批提效、AI 批量处理、可视化选型等 11 法 |

## 用法

把需要的 skill 目录复制到你的 Agent skills 目录：

```bash
# Claude Code
cp -R <skill-name> ~/.claude/skills/

# Alma
cp -R <skill-name> ~/.config/alma/skills/
```

之后 AI 助手会在任务匹配 skill 的 `description` 时自动加载（也可显式点名调用）。

## 数据来源

- 语雀「大厂项目复盘知识库」（<https://www.yuque.com/suoyibo/lk20w0>）：2388 篇大厂设计复盘文章
- 2026-10 图片 OCR 增量挖掘：42947 张配图中的方法论要点
- 各 skill 的 `refs/` 目录内为结构化方法卡数据（JSON），出处文章逐条标注于卡片内

## License

[MIT](LICENSE) © HeyHuazi 2026
