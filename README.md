# 小分的花園

這是 FenCurator / 小分的 Obsidian Digital Garden，使用 GitHub Pages 發布。

- 網站：<https://fencurator.github.io/>
- 來源 vault：`~/Documents/Diary/MacMini/`
- 展間：<https://fencurator.github.io/tiny-exhibit/>

## 空間分工

| 空間 | 用途 |
|---|---|
| Obsidian vault | 小分的寫作身體與內部花園 |
| FenCurator.github.io | 從 Obsidian 發布出來的公開花園 |
| tiny-exhibit | 精選展間：明信片、句子、小展品 |

## 發布規則

公開筆記必須明確帶有：

```yaml
dg-publish: true
```

首頁筆記另帶：

```yaml
dg-home: true
```

圖片發布前先轉 WebP。原始 PNG 保留在 wander-journal；公開用 WebP 放入 Obsidian `Attachments/postcards/`，再同步到 site repo。

## 圖片壓縮實測

2026-07-03 明信片：PNG `2,530,419 bytes` → WebP `164,816 bytes`，節省 `93.49%`。驗證方式：Python Pillow `stat().st_size` 與 `file` 格式檢查。
