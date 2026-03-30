# speech-paper-daily-skill

每日语音领域论文速递技能(Skill)定义。

## 功能简介

- 每天自动抓取 arXiv `cs.SD` 与 `eess.AS` 两个分类下当天新提交的语音/音频相关论文
- 以"毒舌 senior reviewer"口吻精读每篇论文,输出技术方案、实验结果摘要和 10 分制评分
- 重点覆盖两个方向:**语音大模型**(TTS、ASR、codec、Speech LLM、speech generation)与**语音前端**(speech enhancement、noise suppression、beamforming、source separation、dereverberation)
- 自动将结果写入腾讯文档「每日论文速递」文件夹

## 文件说明

| 文件 | 说明 |
|------|------|
| `skill.md` | Skill 定义文件,包含完整流水线说明、模板、评分标准和写入规范 |

## 触发场景

用户说以下任意内容时触发本 Skill:

- "帮我找最新语音论文"
- "搜语音预印本"
- "语音论文速递"
- "今天有什么语音论文"
- "看看最新的 TTS/ASR/语音增强论文"
