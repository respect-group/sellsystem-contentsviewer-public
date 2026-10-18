[English](#english) | [日本語](#日本語)

## 日本語

# Easy Digital Content Viewer（イージーデジタルコンテンツビューワー）

販売者から配布されるデジタルコンテンツ（コンテンツパッケージ。拡張子 `.hbcontent`）を閲覧するための、**汎用ビューワー**です。Windows / macOS に対応します。

> **このリポジトリについて**
> このリポジトリにはソースコードは含まれていません。GitHub Actions でビルドされた成果物（バイナリ）のみを、**Releases ページ**で配布しています。

### 概要

- 商品ごとに別のアプリを入れる必要はありません。ビューワーは**一度だけ入手**し、以降は商品ごとのコンテンツパッケージ（`.hbcontent`）を追加していきます。
- 取り込んだパッケージは「書庫」の一覧に登録され、一覧から選ぶだけで開けます。複数の商品のパッケージをまとめて管理できます。
- アクティベーションキーが必要なコンテンツでは、購入時に届いたキーで有効化します。一度アクティベートしたコンテンツは、有効期限内であれば一覧から選ぶだけで開けます。
- PDF・画像・音声・動画・テキスト／Markdown を、ビューワー内で表示できます。音楽・動画にはプレイリスト機能があります。
- 表示言語は日本語・英語に対応します。
- Node.js などの開発環境は不要です。

### 入手方法

1. このリポジトリの **Releases** ページを開きます（画面右側の「Releases」、またはリポジトリ上部のリンクから開けます）。
2. 最新のリリースから、お使いのOS向けのファイルをダウンロードします。
   - Windows: `Windows-Portable-Folder.zip`
   - macOS: Mac版が配布されている場合のみ、リリースに添付されています。
3. 下記の「インストール方法」に従って展開・起動します。

Windows 版は展開後で約344MBあります。インストーラは使わず、展開したフォルダをそのまま使います（コピーして使う前提の形式です）。

### インストール方法

「イージーデジタルコンテンツビューワー」は署名なしで配布しているため、初回起動時に警告が出ることがあります。配布元とファイルを確認し、信頼できる場合に以下の手順で進めてください。Node.jsなどの開発環境は不要です。

#### Windows

1. 配布されたZIPファイル（`Windows-Portable-Folder.zip`）を、任意の場所に展開（解凍）します。
2. 展開したフォルダ内の `Easy Digital Content Viewer.exe` をダブルクリックして起動します。ほかのファイルも同じフォルダに保管してください（`.exe` だけを移動しないでください）。
3. 「WindowsによってPCが保護されました」と表示されたら、**「詳細情報」→「実行」**をクリックします。
4. 次回からは、同じ `Easy Digital Content Viewer.exe` をダブルクリックするか、ショートカットを作成して起動します。

「実行」が表示されない場合は、配布元またはPCの管理者にご相談ください。

#### macOS（Mac版が配布されている場合）

1. ダウンロードしたファイルを展開し、アプリ（`.app`）を「アプリケーション」フォルダに移動します。
2. アプリをダブルクリックします。開発元を確認できないという警告が出たら閉じます。
3. **Appleメニュー →「システム設定」→「プライバシーとセキュリティ」**を開き、アプリのブロック通知にある**「このまま開く」**をクリックします。
4. 確認画面で「開く」を選びます。認証を求められた場合は画面の案内に従います。

次回からは通常どおり起動できます。「このまま開く」が表示されない、または「壊れている」と表示される場合は、配布元にご相談ください。

#### 初回起動

使用許諾契約（EULA）を読み、同意する場合は「購入撤回権の放棄」と「契約全体への同意」の両方にチェックを入れ、「同意して開始」をクリックします。

### 基本的な使い方

#### コンテンツパッケージの開き方

1. 販売者から入手したコンテンツパッケージ（`.hbcontent`）をダブルクリックするか、ビューワーの「＋ パッケージを追加…」から選びます。取り込むと、書庫の一覧に登録されます。
2. アクティベーションキーが必要なコンテンツは、購入時に届いたキーを入力します。キーが不要な場合や試用がある場合は、画面の案内に従います。
3. 一度アクティベートしたコンテンツは、有効期限内であれば、一覧から選ぶだけで開けます。

#### 保存先フォルダの設定

書庫の画面の「設定」で、コンテンツパッケージの保存先フォルダを指定できます。ダウンロードしたパッケージが保存先と別の場所にあるときは、保存先へコピー（元のファイルは残す）または移動（元のファイルは削除）します。コンテンツの更新で内容が変わるときも、保存先の「コンテンツごとのフォルダ」に保存します。

### ご利用上の注意

- コンテンツには、ビューワー内でのみ閲覧でき、フォルダ外への持ち出しができない保護が掛かっている場合があります。保護の有無や、保存・印刷・右クリックメニューなどの可否はコンテンツごとに異なります。
- 右クリックの制限や保存ショートカットのブロックは、気軽なコピーを抑えるためのものです。スクリーンショットや画面録画を防ぐものではありません。
- 署名なしで配布しているため、Windows SmartScreen や macOS Gatekeeper の警告が出ます。配布元とファイルを確認したうえでお使いください。
- ご不明な点は、配布元（コンテンツの販売者）にご相談ください。

### OSの警告について

[Microsoft SmartScreen](https://learn.microsoft.com/en-us/windows/apps/package-and-deploy/smartscreen-reputation) · [Apple Support](https://support.apple.com/102445)

---

## English

# Easy Digital Content Viewer

A **generic viewer** for digital content (content packages with the `.hbcontent` extension) distributed by sellers. Supports Windows and macOS.

> **About this repository**
> This repository does not contain source code. Only artifacts (binaries) built by GitHub Actions are distributed, on the **Releases page**.

### Overview

- You do not need a separate app for each product. **Get the viewer once**, then keep adding the content packages (`.hbcontent`) for each product.
- Imported packages are registered in the library list, and you can open them just by choosing them from the list. Packages from multiple products are managed together.
- For content that requires an activation key, activate it with the key you received at purchase. Once activated, content can be opened just by choosing it from the list while its activation is still valid.
- PDFs, images, audio, video, and text/Markdown can be displayed inside the viewer. Music and video support playlists.
- The UI supports Japanese and English.
- You do not need Node.js or other developer tools.

### How to Get It

1. Open the **Releases** page of this repository (from the "Releases" section on the right side of the repository page, or the link at the top).
2. From the latest release, download the file for your OS.
   - Windows: `Windows-Portable-Folder.zip`
   - macOS: Attached to the release only if a Mac version is available.
3. Extract and launch it by following "Installation" below.

The Windows version is about 344 MB once extracted. No installer is used; you use the extracted folder as it is (it is designed to be copied and run).

### Installation

Easy Digital Content Viewer is distributed without a code signature, so a warning may appear on the first launch. Check the source and file, and follow these steps only if you trust them. You do not need Node.js or other developer tools.

#### Windows

1. Extract (unzip) the distributed ZIP file (`Windows-Portable-Folder.zip`) to any location.
2. Double-click `Easy Digital Content Viewer.exe` inside the extracted folder. Keep all files in the folder together (do not move the `.exe` alone).
3. If **Windows protected your PC** appears, click **More info → Run anyway**.
4. From the next time, double-click the same `Easy Digital Content Viewer.exe`, or create a shortcut to it.

If Run anyway is unavailable, contact the distributor or your PC administrator.

#### macOS (if a Mac version is available)

1. Extract the downloaded file and move the app (`.app`) to the Applications folder.
2. Double-click the app. If a warning says the developer cannot be verified, dismiss it.
3. Open **Apple menu → System Settings → Privacy & Security**, then click **Open Anyway** next to the notice that the app was blocked.
4. Click Open in the confirmation dialog. Follow any authentication prompts.

After this, you can open the app normally. If Open Anyway is unavailable or the app is reported as damaged, contact the distributor.

#### First Launch

Read the End User License Agreement (EULA). If you agree, check both the withdrawal-right waiver and agreement acceptance boxes, then click Agree and Start.

### Basic Usage

#### Opening a content package

1. Double-click the content package (`.hbcontent`) you received from the seller, or choose it with "+ Add package…" in the viewer. It is then registered in the library list.
2. For content that requires an activation key, enter the key you received at purchase. If no key is required, or a trial is available, follow the on-screen instructions.
3. Once activated, content can be opened just by choosing it from the list while its activation is still valid.

#### Setting the save folder

In "Settings" on the library screen you can choose the folder where content packages are stored. If a downloaded package is outside that folder, it is copied (the original is kept) or moved (the original is deleted) into it. When content is updated, the new version is also saved in the per-content folder inside the save folder.

### Notes

- Some content may be protected so that it can be viewed only inside the viewer and cannot be taken out of its folder. Whether protection applies, and whether saving, printing, or the right-click menu are allowed, differs from one content package to another.
- Right-click restrictions and blocked save shortcuts only deter casual copying. They do not prevent screenshots or screen recording.
- Because the app is distributed without a code signature, Windows SmartScreen and macOS Gatekeeper warnings appear. Use it only after checking the source and the file.
- If you have any questions, contact the distributor (the content seller).

### About OS warnings

[Microsoft SmartScreen](https://learn.microsoft.com/en-us/windows/apps/package-and-deploy/smartscreen-reputation) · [Apple Support](https://support.apple.com/102445)