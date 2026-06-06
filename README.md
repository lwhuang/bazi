![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)
![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)

# 賽博算命 Skill

基於 Claude Code 的八字排盤與命理分析工具。通過交互式對話收集出生信息，排出四柱八字，參照九本經典命理典籍進行專業分析。

## 功能

- **信息收集** — 逐步收集姓名、陽曆/農曆生日、出生時辰、性別、出生地等信息
- **排盤計算** — 自動排出年柱、月柱、日柱、時柱，計算大運與流年
- **綜合分析** — 日主強弱、十神關係、五行平衡、格局判定、大運流年解讀，以及事業、感情、健康等方面的建議

## 安裝

> **注意**：Claude Code 從 git 倉庫根目錄的 `.claude/skills/` 查找 skill，請在正確的位置執行。

```bash
# 安裝到當前項目（在 git 倉庫根目錄執行）
mkdir -p .claude/skills
git clone https://github.com/jinchenma94/bazi-skill .claude/skills/bazi

# 或安裝到全局（所有項目都能用）
git clone https://github.com/jinchenma94/bazi-skill ~/.claude/skills/bazi
```

## 使用

在 Claude Code 中輸入以下任意關鍵詞即可觸發：

`算八字` `看八字` `批八字` `排八字` `四柱` `命盤` `算命` `排盤` `bazi`

觸發後，Skill 會逐步引導你提供出生信息，然後進行排盤和綜合分析。

## 參考典籍

| 典籍 | 簡稱 |
|------|------|
| 《窮通寶典》 | 論日主調候 |
| 《三命通會》 | 論格局神煞 |
| 《滴天髓》 | 論五行旺衰 |
| 《淵海子平》 | 論十神六親 |
| 《千里命稿》 | 論命例實證 |
| 《協紀辨方書》 | 論擇日神煞 |
| 《果老星宗》 | 論星命合參 |
| 《子平真詮》 | 論用神格局 |
| 《神峰通考》 | 論命理辨誤 |

## 項目結構

```
bazi-skill/
├── SKILL.md                        # Skill 入口
├── references/                     # 參考文件
│   ├── wuxing-tables.md            #   五行、天干地支、十神參考表
│   ├── shichen-table.md            #   時辰對照表、日上起時法
│   ├── dayun-rules.md              #   大運順逆排規則、起運年齡計算
│   └── classical-texts.md          #   九本經典典籍核心規則摘要
├── LICENSE
└── README.md
```

## 免責聲明

本 Skill 僅供傳統文化學習與娛樂參考，分析結果不構成任何決策依據。命理學屬於傳統文化範疇，請理性看待。
