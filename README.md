[English](#english) | [日本語](#日本語)

## 日本語

# Easy Digital Content Viewer（イージーデジタルコンテンツビューワー）

デジタルコンテンツ商品（PDF・画像・音声・動画・テキスト／Markdownなど）を、アクティベーションキーで保護しながら閲覧するための汎用ビューワーアプリです。Windows / macOS に対応しています。

このリポジトリでは**ソースコードではなく、GitHub Actions でビルド済みの実行ファイル（バイナリ）のみ**を配布しています。商品（コンテンツパッケージ）ごとにアプリを入れ直す必要はなく、**このビューワー本体は一度だけインストールしておけば、以降は購入した商品のパッケージファイルを読み込むだけ**で利用できます。

### 主な特徴

- **1本のアプリで複数商品を管理**：取り込んだ商品は「書庫（ライブラリ）」の一覧に登録され、以降は一覧から選ぶだけで開けます（アクティベーション済みなら、有効期限内はキーの再入力不要）。
- **単一ファイルで配布される商品パッケージ**（拡張子 `.hbcontent`）：ダウンロードしたファイルをダブルクリックするだけで取り込めます。
- **PDF・画像・音声・動画・テキスト／Markdown** に対応したビューア内蔵（PDFは目次・しおり表示、販売者が許可した場合は印刷にも対応）。
- **音楽・動画のプレイリスト再生**：選択した順番での再生、並べ替え、繰り返し（なし／1件／全体）に対応。
- **コピーガード**：右クリックメニューの抑止やドラッグによる持ち出し防止など、カジュアルなコピーを抑止する仕組みを搭載（ただし下記「ご利用にあたっての注意」を参照）。
- **開発者からのお知らせ表示**、**コンテンツの更新確認**（起動時に新しいバージョンの有無を確認）など。
- **日本語／英語のUI切り替え**に対応。

### 入手方法

本アプリの実行ファイル一式は、このリポジトリの **[Releases（リリース）ページ](../../releases)** から入手してください。

- OSに応じて Windows 用 / macOS 用のアーカイブ（zipなど）が公開されます。該当するものをダウンロードしてください。
- **インストーラ形式ではなく、展開してそのまま使う形式（ポータブル形式）です。** ダウンロードしたアーカイブを展開し、好きな場所に置いて使用してください。
- 本アプリは**無料で配布される「書庫（ビューワー）本体」**であり、個々の商品（コンテンツ）は別途、各商品の販売ページ等から入手・購入する必要があります。

### インストール・起動方法

#### Windows

1. Releasesページから Windows 用のアーカイブをダウンロードし、展開します。
2. フォルダの中にある `Easy Digital Content Viewer.exe` を実行します。
3. **本アプリはコード署名を行っていません。** 初回起動時に Windows SmartScreen の「WindowsによってPCが保護されました」という警告が表示される場合があります。その場合は「詳細情報」→「実行」を選択してください。
4. 初回起動時に、`.hbcontent` ファイルをこのアプリに関連付ける処理が自動的に行われます（以降は `.hbcontent` ファイルをダブルクリックするだけでアプリが開きます）。

#### macOS

1. Releasesページから macOS 用のアーカイブをダウンロードし、展開します。
2. アプリ（`.app`）を `アプリケーション` フォルダ等に移動して起動します。
3. **本アプリはコード署名・公証を行っていません。** 初回起動時に Gatekeeper により「開発元が未確認のため開けません」等の警告が表示される場合があります。その場合は、Finderでアプリを右クリック（またはControl+クリック）し「開く」を選択することで起動できます。

### 基本的な使い方

1. **アプリを起動すると「書庫（ライブラリ）」の一覧画面が表示されます。** 最初は何も登録されていません。
2. **商品パッケージ（`.hbcontent` ファイル）を取り込みます。** 方法は2通りです。
   - ダウンロードした `.hbcontent` ファイルをダブルクリックする。
   - アプリを起動した状態で「＋ パッケージを追加…」から該当ファイルを選ぶ。
3. 取り込むと使用許諾契約（EULA）への同意画面が表示されます。内容を確認し、同意して進みます。
4. 初めて開く商品では、メールアドレスの入力・撤回権に関する同意・**アクティベーションキーの入力**が必要です（キーは各商品の購入ページ等から入手してください。画面内にも購入ページ・販売者の案内ページへのリンクが表示されます）。
5. アクティベーションが完了すると、その商品のコンテンツ一覧（目次）が表示され、PDF・画像・音声・動画・テキストなどを閲覧できます。
6. **一度アクティベートした商品は、有効期限内であれば次回以降キーの再入力なしで開けます。** 各画面にある「← 書庫に戻る」から一覧に戻り、別の商品を選ぶこともできます。
7. 一覧画面から商品を「削除」すると、取り込んだパッケージとアクティベーション状態がアプリから削除されます（元のダウンロードファイル自体は影響を受けません）。
8. 画面内の「設定」から、保存先フォルダの変更や表示言語（日本語／英語）の切り替えができます。
9. 画面内の操作マニュアルから、プレイリスト機能（連続再生・並べ替え・繰り返し設定）などの詳しい使い方を確認できます。

### ご利用にあたっての注意

- 本アプリの著作権保護機能（右クリック抑止・ドラッグ防止・ファイルの暗号化等）は、**カジュアルなコピーを抑止するためのものであり、完全な複製防止を保証するものではありません。**
- **スクリーンショットや画面録画は、本アプリの仕組みでは防止できません。**
- 技術的に踏み込んだ利用（開発者ツールの使用等）による回避についても、完全には防げません。

### 動作環境

- Windows（x64）または macOS。
- インターネット接続（アクティベーション時・コンテンツ更新確認時に必要。オフラインでも既にアクティベート済みのコンテンツは閲覧できます）。

---

## English

# Easy Digital Content Viewer

A general-purpose viewer app for browsing digital content products (PDFs, images, audio, video, text/Markdown, etc.) protected by an activation key. Supports Windows and macOS.

This repository distributes **only prebuilt binaries produced by GitHub Actions — not source code.** You do not need to reinstall the app for each product; **install this viewer once, and simply load each purchased product's package file afterwards.**

### Key Features

- **Manage multiple products from a single app**: imported products are registered in a "library" list, and from then on you can just pick them from the list to open them (no need to re-enter the activation key while it's still valid).
- **Products are distributed as a single file** (extension `.hbcontent`): just double-click a downloaded file to import it.
- **Built-in viewers for PDF, images, audio, video, and text/Markdown** (PDF supports a table of contents/bookmarks, and printing when allowed by the seller).
- **Playlist playback for music and video**: play in a chosen order, reorder tracks, and set repeat (none / one / all).
- **Copy-guard features**: context-menu suppression and drag-out prevention to deter casual copying (see "Important Notes" below).
- **Developer notices** shown in the app, and an **automatic content-update check** at startup.
- **Japanese/English UI language switch.**

### How to Get It

Download the app from this repository's **[Releases page](../../releases)**.

- Archives (e.g. zip files) are published for Windows and macOS. Download the one matching your OS.
- **This is not an installer — it's a portable, unpacked app.** Extract the archive and place it anywhere you like.
- This is the **free "library/viewer" application itself**. Individual content products must be purchased/obtained separately, typically from each product's sales page.

### Installation and Launch

#### Windows

1. Download and extract the Windows archive from the Releases page.
2. Run `Easy Digital Content Viewer.exe` inside the extracted folder.
3. **This app is not code-signed.** On first launch, Windows SmartScreen may show a "Windows protected your PC" warning. If so, click "More info" → "Run anyway".
4. On first launch, the app automatically registers itself as the handler for `.hbcontent` files, so afterwards you can just double-click an `.hbcontent` file to open it.

#### macOS

1. Download and extract the macOS archive from the Releases page.
2. Move the app (`.app`) to your `Applications` folder (or anywhere else) and launch it.
3. **This app is not code-signed or notarized.** Gatekeeper may show a warning such as "cannot be opened because the developer cannot be verified" on first launch. If so, right-click (or Control-click) the app in Finder and choose "Open" to launch it anyway.

### Basic Usage

1. **When you launch the app, you'll see the "library" list screen.** It starts out empty.
2. **Import a product package (`.hbcontent` file)** using either of two methods:
   - Double-click a downloaded `.hbcontent` file, or
   - With the app already running, use "+ Add package…" and choose the file.
3. After importing, you'll be shown the End User License Agreement (EULA). Review it and agree to proceed.
4. The first time you open a given product, you'll need to enter your email address, agree to a notice about waiver of the right of withdrawal, and **enter the activation key** (obtain the key from the product's sales page etc. — links to the purchase page and the seller's guide page are shown on screen).
5. Once activated, the product's content list (table of contents) appears, and you can browse PDFs, images, audio, video, text, and more.
6. **Once a product has been activated, you can reopen it directly from the library list without re-entering the key, as long as the activation is still valid.** Use "← Back to library" on any screen to return to the list and pick another product.
7. Choosing "Remove" from the list deletes both the imported package and its activation state from the app (the original downloaded file is unaffected).
8. Use the in-app "Settings" to change the save folder or switch the display language (Japanese/English).
9. The in-app manual explains features such as playlists (continuous playback, reordering, repeat settings) in more detail.

### Important Notes

- The app's copy-protection features (context-menu suppression, drag-out prevention, file encryption, etc.) are **intended to deter casual copying only — they do not guarantee that copying is completely impossible.**
- **Screenshots and screen recording cannot be prevented** by this app's mechanisms.
- Workarounds by technically sophisticated users (e.g. using developer tools) cannot be fully prevented either.

### System Requirements

- Windows (x64) or macOS.
- An internet connection is required for activation and for checking content updates (already-activated content can still be viewed offline).