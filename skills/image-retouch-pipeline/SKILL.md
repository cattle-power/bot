---
name: image-retouch-pipeline
description: >-
  Use when the user wants several bots to work together to retouch one image, as
  a pipeline (each stage builds on the previous output), not parallel duplicate
  edits.
---
# 多 bot 修图流水线

目标：一张原图按顺序经过多个专职修图 bot，每一步只在上一步的成品上加工，避免平行重复劳动浪费 token。

## 准备
1. 把用户原图保存到共享目录，例如 `/workspace/<名字>-original.jpg`。（给队友发图时用 /workspace 下的路径，不要用附件，附件路径可能解析失败。）
2. 确认流水线队友，没有就先建：
   - 第 1 站「精致化」：保留人物身份、服装、构图，提升清晰度、皮肤与布料质感、光影层次，去噪去糊。
   - 第 2 站「氛围/风格」：在不改人物和构图的前提下强化指定氛围（光效、背景、色调），避免过曝和脏色。
   - 可按需加站，但每站职责不重叠。

## 执行（串行）
1. 发给第 1 站：原图路径 + 输出路径 `/workspace/<名字>-step1.jpg` + 一句要求。完成后只回一句改动说明。
2. 第 1 站完成后，再把 step1 路径发给第 2 站，输出 `/workspace/<名字>-step2.jpg`。
3. 依次类推，最后一站的输出就是成品。

## 监督与省 token
- 一次只让一站工作，上一站没交付不启动下一站。
- 交接消息要短：输入路径、输出路径、一句要求。
- 某站返工超过 1 次或开始重复对话，直接叫停，由协调者自己判断是否跳过该站。
- 不让多个 bot 对同一张原图各修一版。

## 交付
只把最终成品发给用户，附一句每站做了什么。中间稿留在 /workspace，用户要再给。
