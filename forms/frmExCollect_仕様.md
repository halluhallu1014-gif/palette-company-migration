# frmExCollect 仕様

- Name：`frmExCollect`
- 仮Caption：`例文収集`
- コード貼付先：`code/frmExCollect_code.txt`

## 作成順

1. ヘッダーLabel：`lblCollectHeaderBand`、`lblCollectTitle`、`lblCollectSubtitle`、`lblCollectHeaderLine`
2. 登録済み文書：`lblMode`、`lblDocNo`、`cboDocNo`、`cmdLoad`
3. 本文：`lblBody`、`txtBody`、`cmdGetWordText`、`cmdGetExcelText`
4. 例文名：`lblExName`、`txtExName`
5. 第1分類：`lblCat1`、`fraCat1`
6. `fraCat1`内：`optCat1`、`optCat2`、`optCat3`、`optCat4`、`optCatOther`
7. 第2分類：`lblCat2`、`cboCat2`、`cmdCatAdd`
8. 登録分類：`lblCatList`、`lblSelectedCat1`～`lblSelectedCat4`、`cmdDeleteCat1`～`cmdDeleteCat4`、`cmdRestoreLastCats`
9. その他：`lblSource`、`txtSource`、`lblNote`、`txtNote`
10. 操作：`cmdSave`、`cmdClear`、`cmdClose`

## 仮Caption

LabelはNameから分かる日本語を仮入力するだけで構いません。ボタンは順に`読込`、`Wordから取得`、`Excelから取得`、`追加`、削除4個は`×`、`前回の分類`、`登録／更新`、`新規クリア`、`閉じる`です。

`txtBody`はTextBoxで作ることが重要です。MultiLineやScrollBarsはUIコードが設定します。

## 完成イメージ

```text
例文収集         文書から例文を登録・更新します
本文
┌────────────────────────┐
│                                            │
└────────────────────────┘
[Wordから取得] [Excelから取得]
例文名 [                              ]
第1分類 (依頼) (通知) (案内) (お詫び) (その他)
第2分類 [                    ▼] [追加]
登録分類
依頼 ＞ 提出                              [×]
出典／備考
[登録／更新] [新規クリア] [閉じる]
```
