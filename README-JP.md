# Xcode Color

[EN](./README.md) / [JP](./README-JP.md)

Visual Studio Code/Cursor向けのXcode風のカラーテーマ、およびSwiftのカラーマッピングを提供します。

このテーマのSwift向けカラーを最大限に利用するには、`xcode-build-server` を使って VS Code/Cursor と Xcode プロジェクトを連携させてください。

セットアップ手順:

1. `xcode-build-server`のインストール
   - ターミナルで`brew install xcode-build-server`を実行
2. `buildServer.json`の作成
   - `xcode-build-server config -project <プロジェクト名>.xcodeproj -scheme <プロジェクト名>`
   - CocoaPods などで `.xcworkspace` を使っている場合:
   - `xcode-build-server config -workspace <プロジェクト名>.xcworkspace -scheme <プロジェクト名>`

![サンプルコード](./assets/sample-code.png)

### [1.0.2] -- 2026.3.24

いくつかのワードに対応しました。

### [1.0.1] -- 2026-3-24

VS Code の対応バージョンを 1.110.0 から 1.80.0 に変更

### [1.0.0] -- 2026-3-23

初期バージョンをリリース