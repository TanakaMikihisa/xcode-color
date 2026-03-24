# Xcode Color

[EN](./README.md) / [JP](./README-JP.md)

Provides an Xcode-style color theme for Visual Studio Code/Cursor, along with Swift color mappings.

To get the full Swift color highlighting from this theme, connect VS Code/Cursor to your Xcode project using `xcode-build-server`.

Quick setup:

1. Install `xcode-build-server`.
   - Run in terminal: `brew install xcode-build-server`
2. Generate `buildServer.json` in your project root (where `.xcodeproj` exists).
   - `xcode-build-server config -project <ProjectName>.xcodeproj -scheme <ProjectName>`
   - If you use `.xcworkspace` (for example with CocoaPods):
   - `xcode-build-server config -workspace <ProjectName>.xcworkspace -scheme <ProjectName>`
3. Reload the VS Code/Cursor window.
   - Open Command Palette (`Cmd + Shift + P`)
   - Run `Developer: Reload Window`
4. Wait a few seconds for SourceKit-LSP to load `buildServer.json`, then run "Inspect Editor Tokens and Scopes" on a Swift symbol.
   - If `semantic token type` appears at the top, semantic tokens are active.

![Sample Code](./assets/sample-code.png)

### [1.0.2] -- 2026.3.24

Various fixes and improvements.

### [1.0.1] -- 2026-3-24

Changed the supported VS Code version from 1.110.0 to 1.80.0.

### [1.0.0] -- 2026-3-23

Released the initial version.
