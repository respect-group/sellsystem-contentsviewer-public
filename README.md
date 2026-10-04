[English](#english) | [日本語](#日本語)

## 日本語

# SecureViewer

SecureViewer は、デジタルコンテンツ商品（PDF・画像・音声・動画・テキスト／Markdownなど）を、アクティベーションキーによるライセンス管理とコピーガード付きで閲覧するための汎用ビューワーアプリです。Windows / macOS に対応しています。

このリポジトリは**ソースコードの開発用リポジトリではなく、GitHub Actions でビルドされた配布用バイナリ（実行ファイル一式）を公開するためのリポジトリ**です。SecureViewer を使ってコンテンツを閲覧したい方は、以下の手順でアプリ本体を入手してください。

### 特徴

- **1本のビューワーを様々な商品で使い回せます。** 商品ごとに別のアプリをインストールする必要はなく、SecureViewer 本体を一度インストールすれば、複数の商品コンテンツパッケージ（`.hbcontent` ファイル）を取り込んで管理できます。
- **配布コンテンツは `.hbcontent` という単一ファイル形式。** ダブルクリックで開く、またはアプリ内の「＋ パッケージを追加」からファイルを選んで取り込めます。
- **一度アクティベーションしたコンテンツは、有効期限内であれば次回からキー再入力なしで開けます。**
- PDF・画像・音声・動画・テキスト/Markdown など、複数のコンテンツ形式を一つのビューワー内で表示できます。
- 日本語・英語の表示切り替えに対応しています。

### 動作環境

- Windows（64bit）
- macOS（Intel / Apple Silicon 両対応のユニバーサルビルド）

### 入手方法（GitHub Releases）

1. このリポジトリの **[Releases](../../releases)** ページを開きます。
2. お使いのOSに対応したビルド成果物をダウンロードします。
3. ダウンロードしたファイル（zip等の圧縮アーカイブ）を展開します。
4. 展開してできたフォルダの中にある実行ファイルを起動します。
   - Windows: `SecureViewer.exe`
   - macOS: `SecureViewer.app`

※ 本アプリは**コード署名を行っていません**。初回起動時にWindowsのSmartScreenや、macOSのGatekeeperにより「発行元が確認できないアプリです」といった警告が表示される場合がありますが、これは既知の挙動です。内容を確認のうえ、必要に応じて「詳細情報」→「実行」（Windows）や、Finderでアプリを右クリック→「開く」（macOS）等の操作で起動してください。

### 基本的な使い方

1. **SecureViewer を起動します。** 初回起動時は、まだ何も取り込んでいない「書庫（ライブラリ）」の一覧画面が表示されます。
2. **コンテンツパッケージ（`.hbcontent` ファイル）を取り込みます。** 方法は2通りあります。
   - 購入・入手した `.hbcontent` ファイルをダブルクリックする（Windowsは初回起動時に自分自身をファイル関連付けへ自己登録します。macOSでうまく開かない場合は、アプリ内の「＋ パッケージを追加」から手動で選択してください）。
   - SecureViewer を起動した状態で「＋ パッケージを追加…」をクリックし、ファイル選択ダイアログから `.hbcontent` ファイルを選ぶ。
3. **利用規約（EULA）への同意画面が表示された場合は、内容を確認して同意します。**
4. **アクティベーション（ライセンスキーの入力）を行います。** 商品によっては体験版での利用や、キー入力が不要なコンテンツもあります。利用可能な台数の上限に達している場合は、その旨のメッセージが表示されます。
5. **アクティベーションが完了すると、コンテンツの一覧・閲覧画面に進みます。** PDF・画像・音声・動画・テキスト/Markdownなど、ファイルの種類に応じた表示形式で閲覧できます。
6. **画面上部などの言語切り替えから、表示言語（日本語／英語）を変更できます。**
7. **「← 書庫に戻る」から、いつでも最初の一覧画面に戻れます。** 一覧画面で「削除」を選ぶと、そのパッケージと関連するアクティベーション情報が書庫から削除されます（元のダウンロードファイル自体は影響を受けません）。
8. **アプリ起動時に、コンテンツの更新情報が確認されることがあります。** 更新がある場合は、画面上部に控えめな通知バナーが表示されるか（内容の閲覧は継続可能）、商品の設定によっては新しいバージョンの入手が必須であるとして一覧がブロックされる場合があります。

### ご利用にあたっての注意事項

- 本アプリの右クリック無効化やドラッグによる持ち出し防止などのコピーガード機能は、**カジュアルなコピーを抑止するためのものであり、技術的に高度な回避手段（スクリーンキャプチャ、画面録画、DevTools の利用など）を完全に防止するものではありません。**
- PDF・画像・動画等をアプリ内で表示する以上、**スクリーンショットや画面録画そのものを技術的に防ぐことはできません。**
- 購入時・配布時に提示された利用規約・ライセンス条件に従ってご利用ください。

### 不具合・お問い合わせ

本アプリに関するご質問・不具合報告は、コンテンツの購入元・配布元の案内に従ってご連絡ください。

---

## English

# SecureViewer

SecureViewer is a general-purpose viewer application for digital content products (PDFs, images, audio, video, text/Markdown, and more), providing license management via activation keys and copy-guard protection. It supports Windows and macOS.

This repository is **not a source-code development repository** — it is used to publish **pre-built distribution binaries produced by GitHub Actions**. If you want to use SecureViewer to view content, obtain the app using the steps below.

### Features

- **One viewer is shared across many different products.** You don't need to install a separate app for each product — install SecureViewer once, then import and manage multiple product content packages (`.hbcontent` files) within it.
- **Distributed content comes as a single `.hbcontent` file.** You can open it by double-clicking, or import it from within the app via "+ Add package".
- **Once a package has been activated, it can be reopened later without re-entering the license key**, as long as the activation is still valid.
- A single viewer displays multiple content types: PDF, images, audio, video, and text/Markdown.
- The UI can be switched between Japanese and English.

### System Requirements

- Windows (64-bit)
- macOS (universal build, supports both Intel and Apple Silicon)

### How to Get It (GitHub Releases)

1. Open this repository's **[Releases](../../releases)** page.
2. Download the build for your operating system.
3. Extract the downloaded archive (e.g. a zip file).
4. Launch the executable inside the extracted folder.
   - Windows: `SecureViewer.exe`
   - macOS: `SecureViewer.app`

Note: This application **is not code-signed**. On first launch, you may see a warning from Windows SmartScreen or macOS Gatekeeper saying the publisher cannot be verified. This is expected. After confirming the source, proceed via "More info" → "Run anyway" on Windows, or right-click the app → "Open" on macOS.

### Basic Usage

1. **Launch SecureViewer.** On first launch, you'll see the library list screen, which starts out empty.
2. **Import a content package (`.hbcontent` file).** There are two ways to do this:
   - Double-click a `.hbcontent` file you've obtained (on Windows, the app self-registers the file association on first launch; on macOS, if double-clicking doesn't open it, use "+ Add package" inside the app instead).
   - With SecureViewer running, click "+ Add package…" and choose the `.hbcontent` file from the file picker.
3. **If a EULA (End User License Agreement) screen appears, review it and accept to continue.**
4. **Activate the content with your license key.** Some products support trial access or require no key at all. If the number of allowed devices has been exceeded, a corresponding message will be shown.
5. **Once activated, you'll proceed to the content list/browsing screen,** where files are displayed using a viewer appropriate to their type — PDF, image, audio, video, or text/Markdown.
6. **Use the language toggle (e.g. near the top of the screen) to switch between Japanese and English.**
7. **Use "← Back to library" to return to the library list at any time.** Choosing "Remove" from the list deletes the package and its activation state from the library (the original downloaded file itself is unaffected).
8. **On startup, the app may check for content updates.** If an update is available, a subtle banner may appear at the top of the screen (you can continue browsing as normal), or, depending on the product's settings, the content list may be blocked until you obtain the newer version.

### Important Notes

- Copy-guard features such as disabling right-click or preventing drag-out are meant only to **deter casual copying**; they **cannot fully prevent technically sophisticated workarounds** such as screenshots, screen recording, or the use of developer tools.
- Since PDFs, images, and videos are displayed within the app itself, **screenshots and screen recordings cannot be technically prevented.**
- Please use this application in accordance with the terms of use and license conditions provided at the time of purchase or distribution.

### Support

For questions or to report issues with this application, please follow the contact instructions provided by the seller/distributor from whom you obtained the content.