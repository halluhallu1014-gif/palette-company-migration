# Palette 会社PC移行パッケージ

## 目的

自宅PCで動作確認済みのPaletteを、ファイルコピーやVBA部品のインポートを使わず、会社PCの新しいxlsmへ再構築するためのパッケージです。

会社PCでは、UserFormとコントロールの器を作り、GitHubのRaw表示から完成コードをコピーします。位置、サイズ、Caption、色、フォント、シート、見出し、初期分類はセットアップマクロが設定します。

## 最初にすること

1. [01_会社PC作業手順.md](01_会社PC作業手順.md)を開きます。
2. 空のマクロ有効ブックを作成します。
3. [03_フォーム作成手順.md](03_フォーム作成手順.md)の順に3フォームとコントロールを作ります。
4. 下記の順に`code`内のRawコードを貼り付けます。
5. `Palette_Company_Setup`を実行します。
6. `Palette_Company_Check`を実行します。
7. `Palette_Open`を実行します。

## 事前準備

- Windows版Excel
- マクロを保存できる`.xlsm`
- VBAエディタを開けること
- GitHubのRaw表示を閲覧・コピーできること
- 追加の参照設定は不要です
- 「VBAプロジェクト オブジェクトモデルへのアクセスを信頼する」は不要です

## コード貼り付け順

1. [modUIStyle.txt](code/modUIStyle.txt)
2. [modExMain.txt](code/modExMain.txt)
3. [modExPaste.txt](code/modExPaste.txt)
4. [modPalette.txt](code/modPalette.txt)
5. [modCompanySetup.txt](code/modCompanySetup.txt)
6. [modCompanyCheck.txt](code/modCompanyCheck.txt)
7. [frmPalette_code.txt](code/frmPalette_code.txt)
8. [frmExCollect_code.txt](code/frmExCollect_code.txt)
9. [frmExPaste_code.txt](code/frmExPaste_code.txt)

各ファイルはコードだけを収録しています。Raw表示で全選択して、そのまま対象モジュールへ貼り付けてください。

## 公開マクロ

- セットアップ：`Palette_Company_Setup`
- 診断：`Palette_Company_Check`
- Palette起動：`Palette_Open`
- 例文収集の直接起動：`ExCollect_Open`
- 例文貼付の直接起動：`ExPaste_Open`

## 詳細資料

- [移行の全体像](00_移行の全体像.md)
- [シート構成](02_シート構成.md)
- [コントロール一覧](04_コントロール一覧.md)
- [動作確認手順](05_動作確認手順.md)
- [トラブル確認](06_トラブル確認.md)
