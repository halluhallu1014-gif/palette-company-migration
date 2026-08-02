# frmExPaste 仕様

- Name：`frmExPaste`
- 仮Caption：`例文貼付`
- コード貼付先：`code/frmExPaste_code.txt`

## 作成順

1. ヘッダーLabel：`lblPasteHeaderBand`、`lblTitle`、`lblPasteSubtitle`、`lblPasteHeaderLine`
2. 第1分類：`lblCat1`、`fraCat1`
3. `fraCat1`内：`optCat1`、`optCat2`、`optCat3`、`optCat4`、`optCatOther`
4. 第2分類：`lblCat2`、`cboCat2`
5. 候補見出し：`lblCandidates`、`lblHint`
6. 候補Label：`lblExample1`～`lblExample5`
7. ページ：`cmdPrev`、`lblPage`、`cmdNext`
8. 操作：`cmdEdit`、`cmdReload`、`cmdClose`

候補はCommandButtonではなくLabelで作ります。仮Captionは空欄で構いません。

## 完成イメージ

```text
例文貼付       例文をダブルクリックして貼り付けます
第1分類 (依頼) (通知) (案内) (お詫び) (その他)
第2分類 [                              ▼]
例文
┌────────────────────────┐
│ 候補本文                                   │
└────────────────────────┘ × 5件
[前へ]             1 / 1             [次へ]
[編集] [再読込] [閉じる]
```
