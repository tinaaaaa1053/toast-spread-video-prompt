# Toast Spread Video Prompt Skill

一个为任意物体生成“压碎并涂抹在吐司上”ASMR 视频提示词的 Codex Skill，适用于 Google Flow 及同类文生视频工具。

它不是简单替换物体名称，而会根据物体的结构、材质、颜色和声音，联动设计：

- 完整物体的外观与摆放方式
- 可见、连续的压碎或超现实融化过程
- 与物体特征一致的奶油、凝胶、果冻、釉面或薄膜
- 一次从吐司一端到另一端的连续涂抹
- 对应材质的 ASMR 声音
- 防跳切、防残渣、防重复物体和防动作回退等连续性约束

## 安装

将本仓库克隆到 Codex skills 目录：

```bash
git clone https://github.com/tinaaaaa1053/toast-spread-video-prompt.git ~/.codex/skills/toast-spread-video-prompt
```

重新打开 Codex 后即可使用。

## 用法

```text
使用 $toast-spread-video-prompt，把一只半透明的蓝色水母做成涂抹吐司的 Google Flow 视频提示词。
```

也可以只给一个物体名：

```text
使用 $toast-spread-video-prompt：翡翠莲花。
```

或者要求定向修复：

```text
使用 $toast-spread-video-prompt 改写这段提示词。上次生成有跳切、宝石没有完全融化，而且刀来回涂了三次。
```

默认输出一份可直接复制的英文提示词。你也可以指定颜色、物体数量、灯光、涂层厚度、移动方向或要求多个版本。

## 文件结构

```text
toast-spread-video-prompt/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── material-logic.md
    └── original-prompts.md
```

六份最初用于归纳规则的 Prompt（蜂巢、黑珍珠、马卡龙、火山模型、欧泊、土星模型）已在 [`references/original-prompts.md`](references/original-prompts.md) 中逐字保留，方便回溯和比较。

## 设计说明

Skill 将压碎阶段与最终涂抹阶段分开：压碎可以包含多次短促按压，但涂抹必须是一次连续、单向、不中断的动作。这可以避免“整个视频只能有一次刀具动作”与“物体需要先被完全压碎”之间的逻辑冲突。

文生视频具有随机性，提示词能显著强化连续性，但不能保证每次生成都严格服从。遇到具体失败时，建议把失败现象连同原提示词一起交给 Skill 定向修复。
