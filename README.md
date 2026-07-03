# 《定位》AI Skill 蒸馏包

来源：阿尔·里斯、杰克·特劳特《定位》（用户上传 PDF）。

这个包按 cangjie-skill 的思路制作：目标不是普通摘要，而是把书中可复用的方法论拆成可调用、可组合、可测试的 skills。

## 包含内容

- `books/positioning-ries-trout/BOOK_OVERVIEW.md`：整书理解
- `books/positioning-ries-trout/INDEX.md`：技能地图与引用关系
- `books/positioning-ries-trout/candidates/`：候选方法论池
- `books/positioning-ries-trout/rejected/`：被淘汰或合并的候选单元
- 10 个独立 skill，每个包含 `SKILL.md` 和 `test-prompts.json`
- `APPLICATION_PROMPTS.md`：直接可复制的应用提示词

## 使用方式

把整个 `books/positioning-ries-trout/` 文件夹放进你的 agent/skill 工作区。需要做定位判断时，让 agent 优先读取 `INDEX.md`，再按触发场景调用对应 skill。

## 质量说明

本包基于 PDF 文本抽取与人工结构化蒸馏完成，保留候选与淘汰记录。由于当前环境没有真正启动独立 sub-agent 盲测，`test-prompts.json` 已按 darwin-skill 兼容格式设计，但尚未经过外部 agent 自动回归测试。
