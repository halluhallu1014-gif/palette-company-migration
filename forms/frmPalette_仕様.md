# frmPalette 仕様

- Name：`frmPalette`
- 仮Caption：`Palette`
- コード貼付先：`code/frmPalette_code.txt`

## 作成順

1. Labelを4個追加し、`lblPaletteHeaderBand`、`lblPaletteTitle`、`lblPaletteSubtitle`、`lblPaletteHeaderLine`にします。
2. Frameを8個追加し、`fraTool1`～`fraTool8`にします。
3. 各Frameの内側へLabelを3個、CommandButtonを1個追加します。
4. 1番のFrameなら`lblToolAccent1`、`lblToolName1`、`lblToolDesc1`、`cmdTool1`とします。8番まで同じ規則です。
5. フォームへCommandButtonを1個追加し、`cmdClose`にします。

仮Captionは、タイトルを`Palette`、閉じるボタンを`閉じる`、各`cmdTool`を`開く`にします。ほかは空欄で構いません。

## 完成イメージ

```text
Palette
仕事で使う機能を選択
────────────────────────
┌ 例文収集 ─────────┐  ┌ 例文貼付 ─────────┐
│ 文書から例文を登録・整理 │  │ 登録した例文を呼び出す │
│                [開く] │  │                [開く] │
└────────────────┘  └────────────────┘
                                      [閉じる]
```

未使用の3～8番タイルはフォーム初期化時に非表示になります。
