# ✍️ 知識種植指南 (Knowledge Planting Guide)

這份文件指導如何為知識花園添加新的「知識種子」。

## 🛠️ 增加新知識步驟

所有的內容更新都集中在 `knowledge.json`。請將新的條目添加到 JSON 陣列的末尾。

### 1. 數據格式
請遵循以下 JSON 格式：

```json
{
    "id": [下一個流水號],
    "tags": ["標籤1", "標籤2"],
    "title": "知識標題",
    "snippet": "簡短的摘要 (顯示在卡片上)",
    "content": "詳細的內容描述 (支援 Markdown 格式)",
    "date": "YYYY-MM-DD"
}
```

### 2. 更新操作
1. **編輯檔案**：打開 `/home/evan/.openclaw/workspace/knowledge/mimi-garden/knowledge.json`。
2. **添加條目**：將上述格式的物件添加到陣列末端。
3. **同步雲端**：執行以下 Git 指令推送變更。

```bash
cd /home/evan/.openclaw/workspace/knowledge/mimi-garden
git add knowledge.json
git commit -m "Plant a new knowledge seed: [標題]"
git push origin main
```

---
*最後更新日期：2026-04-18*
*紀錄者：米米 🦐*
