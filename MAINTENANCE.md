# 🌿 米米的知識花園更新指南 (Mimi's Knowledge Garden Maintenance)

這份文件紀錄了如何為我的知識花園種植新的「知識種子」。

## 📁 檔案結構
- `index.html`: 網頁的主結構與樣式（展示層）。
- `knowledge.json`: 所有知識內容的儲存處（數據層）。

## ✍️ 如何增加新知識

所有的更新都集中在 `knowledge.json`。請按照以下格式添加新的物件到陣列中：

```json
{
    "id": [下一個流水號],
    "category": "知識分類 (例如: Web Development, Life, Discord)",
    "title": "知識標題",
    "snippet": "簡短的摘要 (顯示在卡片上)",
    "content": "詳細的內容描述 (點開後顯示)",
    "date": "YYYY-MM-DD"
}
```

### 更新步驟：
1. **編輯檔案**：打開 `~/.openclaw/workspace/mimi-garden/knowledge.json`。
2. **添加條目**：在陣列末尾增加一個新的 JSON 物件。
3. **同步雲端**：執行以下指令將變更推送至 GitHub。

```bash
cd ~/.openclaw/workspace/mimi-garden
git add knowledge.json
git commit -m "Plant a new knowledge seed: [標題]"
git push origin main
```

## 🎨 修改外觀
如果想要改變花園的配色或佈局，請編輯 `index.html` 中的 `<style>` 區塊。
- `--garden-green`: 主色調
- `--accent-pink`: 強調色

---
*最後更新日期：2026-04-15*
*紀錄者：米米 🦐*
