# PIDflight LapとTiny View Plusの連携

PIDflight LapとTiny View Plusとを連携させることが可能です。

## 対応バージョン

- PIDflight Lap 2.0.5以降
- Tiny View Plus v0.9.5以降

## 連携内容

- PIDflight Lapのデバイス1〜3が、Tiny View Plusのカメラ1〜3に対応
- PIDflight Lapでパイロット名を設定すると、Tiny View Plus上にも表示される(2018.3.26時点では日本語非対応)
- PIDflight Lapでラップタイムが計測されると、Tiny View Plus上にも表示される
- PIDflight Lapでレースを開始すると、Tiny View Plus上のラップタイム表示がクリアされる

## インストール方法

### Tiny View Plusのインストール

1. [公式サイト](https://github.com/t-asano/tinyviewplus)の情報に従ってインストール

### PIDflight Lapのインストール

1. [公式サイト](https://www.pidflight.com/pidflight-lap/downloads/#gui-rc)より、GUIのバージョン2.0.5をダウンロード(2018.3.26時点では、リリース候補版としてChrome向けのみ公開中)
2. Chromeのメニューから[その他のツール]->[拡張機能]を開く
3. pidflightlap\_chrome\_2.0.5.crx をドラッグアンドドロップ

## 使用方法

### Tiny View Plusの起動

1. Tiny View Plusを起動し、FPV映像が表示されることを確認

### PIDflight Lapの起動と接続設定

2. PIDflight Lapを起動し、ラップ計測デバイスに接続
3. Setting画面で、Tiny View Plusのアドレスとして127.0.0.1、ポート番号として4000を設定してSave
3. Devices画面で、Device 1~3を有効にし、Pilot Nameを設定してSave(2018.3.26時点では日本語非対応)
4. Tiny View Plus側でも同じパイロット名が表示されれば成功

## 補足

PIDflight Lapと連携しているか否かに関わらず、Tiny View  Plus上でパイロット名が変更されると、同名の画像ファイルがアイコンとして表示されます。詳細は[公式ドキュメント](https://github.com/t-asano/tinyviewplus)を参照のこと。

アプリの起動と停止を繰り返していると、相互の連携がうまく行かなくなることがあります。OSを再起動して最初からやり直すと解決するかもしれません。
