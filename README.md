# AI 漫畫短劇製作

AI 漫畫短劇製作專案，目標是建立一套可重複使用的工作流程，快速產出 2 到 3 分鐘的短篇漫畫動畫內容。

## 專案目標

- 建立固定角色與世界觀
- 產出可系列化的短劇腳本
- 以 AI 協作完成分鏡、出圖、動畫、配音與剪輯
- 將每一集的素材與流程標準化，方便持續擴充

## 建議工具

- 劇本：ChatGPT / Claude
- 分鏡：ChatGPT
- 圖像生成：ComfyUI + SDXL
- 動畫：AnimateDiff
- 配音：ElevenLabs
- 音樂：Suno
- 剪輯：DaVinci Resolve

## 專案結構

```text
ai-comic-short-drama-production/
├── assets/
│   ├── characters/
│   ├── references/
│   └── style-guides/
├── docs/
│   ├── production-workflow.md
│   ├── project-brief.md
│   └── shot-template.md
├── episodes/
│   └── EP01/
│       ├── animation/
│       ├── audio/
│       ├── images/
│       ├── script/
│       ├── storyboard/
│       └── video/
├── prompts/
│   ├── image-prompt-template.md
│   ├── script-prompt-template.md
│   └── storyboard-prompt-template.md
└── tools/
```

## 標準流程

1. 先定義角色設定與視覺風格
2. 撰寫單集腳本，切成 4 到 6 個段落
3. 依段落建立分鏡與鏡頭描述
4. 產生角色一致的插圖素材
5. 將關鍵鏡頭轉為短動畫片段
6. 加入配音、字幕與背景音樂
7. 在剪輯軟體中拼接成完整短劇

## 單集建議規格

- 長度：2 到 3 分鐘
- 段落數：4 到 6 段
- 單鏡頭長度：3 到 10 秒
- 圖像解析度：768 x 1024
- 動畫片段：8 到 16 frames 起步

## 開始使用

1. 先閱讀 [docs/project-brief.md](docs/project-brief.md)
2. 依照 [docs/production-workflow.md](docs/production-workflow.md) 建立第一集
3. 使用 `prompts/` 內的模板生成腳本、分鏡與圖片提示詞
4. 將每一集素材集中放在 `episodes/EPxx/` 內

## GitHub 建議

- 使用 Issues 管理每一集的製作進度
- 使用 Projects 管理企劃、製作中、待修正、已發布狀態
- 使用 Releases 保存每一版最終影片與封面素材

## 後續可擴充

- 加入角色設定表
- 加入自動化命名規則
- 加入字幕與旁白生成腳本
- 加入發佈平台清單與上架流程
