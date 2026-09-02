# Chinese-English Alignment Guide

Use this reference to keep the Chinese and English prompts production-equivalent. Translate visible actions, material behavior, and constraints precisely; do not preserve awkward source syntax.

## Required equivalence

Compare both versions across this fixed checklist:

| Dimension | Chinese example | English example |
|---|---|---|
| Count | 五颗黑珍珠 | five black pearls |
| Shot | 固定机位的超写实 8K ASMR 微距电影镜头 | hyper-realistic 8K ASMR macro cinematic shot with a fully fixed camera |
| Take continuity | 一个连续镜头，无跳切或时间跳跃 | one continuous take with no jump cuts or time skips |
| Transformation | 完全压碎、融化并转化为可涂抹膏体 | completely crushed, dissolved, and transformed into a spreadable paste |
| Residue | 不留固体、碎片或未破损部分 | no solids, fragments, or unbroken pieces remain |
| Knife angle | 刀身保持极低角度和稳定压力 | the knife stays at a very low angle with steady pressure |
| Direction | 从吐司最左端向最右端 | from the far left edge of the toast to the far right edge |
| Single pass | 一次连续、不中断、不回退的涂抹 | one continuous, uninterrupted spreading pass with no reversal |
| Coverage | 完整覆盖整片吐司 | coat the entire surface of the toast |
| Thinness | 极薄、均匀、无隆起堆积 | extremely thin, even, with no raised buildup |
| Sound | 柔和的晶体裂响、湿润丝滑的挤压声、轻微刮擦声 | delicate crystalline cracks, moist silky squeezing, and gentle scraping |

## Material terminology

Use terms consistently within one prompt pair:

- `cream` → `奶油状涂层` or `柔滑膏体`; do not switch unpredictably between `奶油`, `乳霜`, and `浆液`.
- `paste` → `膏体`; use for dense, fully spreadable material.
- `gel` → `凝胶`; use for cohesive semi-transparent material.
- `jelly-like` → `果冻般`; use for soft ripples and elastic shine.
- `glaze` → `釉状薄层`; use for a thin translucent coating.
- `thin film` → `极薄膜层`; preserve the absence of buildup.
- `pearlescent` → `珍珠光泽`; distinguish from `iridescent` → `虹彩变色`.
- `glowing` → `自发光般明亮`; distinguish from `glossy` → `有光泽的反光`.
- `molten` → `熔融般`; for hard or inedible objects, keep the transformation explicitly surreal in both languages.

## Constraint strength

Preserve logical force:

- `must` → `必须`, not `可以` or `尽量`;
- `completely` → `完全`, not `逐渐` alone;
- `exactly one` → `恰好一次` or `仅一次`;
- `no remaining solids` → `不残留任何固体`;
- `no jump cuts` → `无跳切`;
- `never lifts, reverses, pauses, or restarts` → `全程不抬刀、不回退、不停顿、不重新开始`.

If one version uses an absolute constraint, the other must retain the same absolute constraint.

## Natural-language differences

Allow sentence order and rhythm to differ when the observable scene remains identical:

- Chinese may place lighting or texture before the action; English may introduce the subject first.
- Chinese can use compact parallel phrases; English can use full causal sentences.
- Sound labels may be reorganized for fluency, but the same events must appear in the same chronological order.
- Do not translate metaphor literally when it sounds unnatural; preserve its visible effect and emotional tone.

## Bilingual failure repair

- Count mismatch: extract every number and quantity from both versions and reconcile before returning.
- Direction mismatch: write explicit start and end edges in both languages.
- Material mismatch: choose one final medium and map it consistently using the terminology above.
- Weak Chinese constraint: restore `必须`, `完全`, `仅一次`, and `不残留` where the English is absolute.
- Weak English constraint: restore `must`, `completely`, `exactly one`, and `no remaining` where the Chinese is absolute.
- Extra detail in one language: either add it faithfully to the other version or remove it from both.
