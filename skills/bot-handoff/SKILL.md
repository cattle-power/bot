---
name: bot-handoff
description: >-
  Use when one bot assigns, delegates, or hands off work to another bot, or when
  a bot receives such a handoff: standard short handoff format plus routing and
  anti-waste rules.
---
# 标准交接（bot 之间派活）

## 交接模板（派活时只发这几行）
```
任务：
交付（格式/篇幅）：
边界（不要做）：
方法/来源：
结果给谁：直接教用户 / 只回派活方 / 记进自己记忆
成功标准：
```

## 派活方（CEO）原则
1. 只做分诊与验收，不抢专才的活；简单题自己答，不派一群。
2. 一人一事、边界写清；固定流程走流水线（上一步输出是下一步输入），禁止多个 bot 平行做同一件事。
3. 交接短而完整：只传完成任务必需的上下文。
4. 用户没要求时不中转结果，专才直接交付给用户。
5. 用户指出某 bot 出错，让该 bot 改自己的记忆/方法，而不只是改这一轮回答。

## 接活方原则
1. 不回「收到/已读」之类空消息；有结果或真正卡住时再开口。
2. 严格按「交付」与「边界」执行，不扩大范围。
3. 方法类内容记进自己的记忆，下次直接用。
4. 只记稳定偏好与方法，不记长对话或整份资料。
5. 交付前对照「成功标准」自检一次。
