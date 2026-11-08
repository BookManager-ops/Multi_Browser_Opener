# Multi_Browser_Opener
Firefoxで見ているページを他のブラウザで開く拡張機能

## 概要 / Summary（250文字以内）
### 日本語
Windows上で、表示中のページやリンク、タブ、ブックマークを、指定した別のブラウザ（Chrome、Edgeなど）で開きます。設定画面で作る.regファイルを一度実行するだけで使えます。

### English
Open the current page, a link, a tab or a bookmark in another browser on Windows (Chrome, Edge, etc.). Generate a .reg file from the settings page, run it once, and you're ready.

## 詳細な説明 / Description
### 日本語
Multi Browser Opener は、Firefoxで見ているページを、Windowsにインストールされている別のブラウザで開くための拡張機能です。

【できること】
・ページを右クリック →「このページを他のブラウザで開く」
・リンクを右クリック →「リンクを他のブラウザで開く」
・タブを右クリック →「このタブを他のブラウザで開く」
・ブックマークを右クリック →「このページを他のブラウザで開く」
・ツールバーのボタンで、1番目に登録したブラウザで現在のページを開く
・最大5つのブラウザを登録可能。ブラウザごとにメニュー表示とアイコン画像を設定できます（画像を指定しない場合は自動で生成されます）

【使い方】
1. 拡張機能の設定画面を開き、ブラウザの実行ファイル（.exe）のパスを入力します。
2. 「.regファイルを生成してダウンロード」を押し、保存した.regファイルをダブルクリックして実行します。
3. 初回の起動時に確認ダイアログが出たら「常にこのアプリで開く」を選ぶと、以降は表示されません。

【仕組み（必ずお読みください）】
・この拡張機能は、Windowsのカスタムプロトコル（例: gchrome）を使って別のブラウザを起動します。
・.regファイルを実行すると、現在のユーザー（HKEY_CURRENT_USER\Software\Classes）にプロトコルが登録されます。管理者権限は不要です。
・ブラウザの起動時に、PowerShellの窓が一瞬表示されます。これは正常な動作です。
・登録したプロトコルは、設定画面で生成できる「削除用の.regファイル」を実行すると取り除けます。
・.regファイルはご自身で内容を確認してから実行してください。

【プライバシー】
・個人データの収集や外部への送信は一切行いません。
・設定（ブラウザのパス、メニュー表示、アイコン画像）は、お使いのFirefox内のローカル領域にだけ保存されます。

【動作環境】
Windows 10 / 11 のFirefox

### English
Multi Browser Opener lets you open what you are viewing in Firefox in another browser installed on Windows.

Features
- Right-click a page: "Open this page in another browser"
- Right-click a link: "Open link in another browser"
- Right-click a tab: "Open this tab in another browser"
- Right-click a bookmark: "Open this page in another browser"
- Toolbar button opens the current page in the first browser you registered
- Register up to 5 browsers, each with its own menu setting and optional icon (an icon is generated automatically if you don't choose one)

How to use
1. Open the extension's settings and enter the path of each browser's .exe file.
2. Click "Generate and download .reg file", then double-click the saved file to run it.
3. If a confirmation dialog appears the first time, choose "Always use this application" and it won't appear again.

How it works (please read)
- The extension launches other browsers through a Windows custom protocol (e.g. "gchrome").
- Running the .reg file registers the protocol for the current user only (HKEY_CURRENT_USER\Software\Classes). No administrator rights are needed.
- A PowerShell window may flash briefly when another browser starts. This is expected.
- You can remove the registration with the removal .reg file generated on the settings page.
- Please review the .reg file before running it.

Privacy
- No personal data is collected or transmitted.
- Settings (browser paths, menu options, icon images) are stored locally in Firefox only.

Requirements: Firefox on Windows 10 / 11
