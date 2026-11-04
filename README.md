# Drama Skills · short-drama-edit

> **[short-drama-edit](https://github.com/simlpandordinary/short-drama-edit)** —— 飞书《WorkBuddy 视频系列 · 全技能与提示词总目录》里推荐的开源技能，已拆分为独立仓库分发（一个技能一个仓库）。

| 项 | 内容 |
| - | - |
| 上游仓库 | <https://github.com/zenstory-ai/drama-skills> |
| 上游路径 | `skills/short-drama-edit` |
| 上游协议 | MIT |
| 上游 Star | 3.7k+ |
| 拆分方式 | 仅抽取该技能自身文件，独立可用 |

## 技能说明

将已生成的短剧镜头剪成成片，记录入出点、镜序、声音、字幕与交付规格。用于套剪、加字幕、统一响度、调整节奏或导出精修素材；需要补素材或修改故事时转回对应创作阶段。

## 目录结构

```
├── LICENSE
├── README.upstream.md
├── SKILL.md
├── scripts/
│   ├── edit_tool.py
│   └── selftest.py
├── references/
│   ├── cut-craft.md
│   ├── delivery-verify.md
│   ├── generated-footage.md
│   ├── sound-and-subtitles.md
│   ├── stage-contract.md
│   └── still-cuts.md
├── assets/
│   ├── 剪辑单.md
│   └── remotion/
│       ├── README.md
│       ├── package.json
│       ├── remotion.config.ts
│       ├── tsconfig.json
│       └── src/
│           ├── Overlay.tsx
│           ├── Root.tsx
│           ├── Subtitles.tsx
│           ├── font.ts
│           ├── index.ts
│           ├── rules.mjs
│           ├── schema.ts
│           └── screen/
│               ├── Card.tsx
│               ├── CornerChip.tsx
│               ├── ScreenText.tsx
│               ├── SystemPanel.tsx
│               ├── TaskPanel.tsx
│               ├── chrome.tsx
│               └── tokens.ts
└── agents/
    └── openai.yaml
```

- `SKILL.md` 是技能入口（触发条件 / 工作流 / 约束），安装时必须位于技能根目录。
- `references/`、`scripts/`、`assets/` 为该技能自带的参考文档、脚本与素材。
- `README.upstream.md` 为上游仓库原始说明，保留出处与版权信息。
- `LICENSE` 为上游许可证原件。

## 安装

WorkBuddy 技能目录为 `~/.workbuddy/skills/short-drama-edit/`：

```bash
git clone https://github.com/simlpandordinary/short-drama-edit.git ~/.workbuddy/skills/short-drama-edit
```

也可以直接对 AI 说：「把 <https://github.com/simlpandordinary/short-drama-edit> 装成 Skill」。

安装后用自然语言触发，例如「Drama Skills · short-drama-edit」「用 short-drama-edit 帮我处理这个任务」。

## 版权

原始作者与版权归上游仓库 `zenstory-ai/drama-skills` 所有。本仓库仅做独立分发与结构整理，未修改技能内容；商用请遵循上游许可证。
