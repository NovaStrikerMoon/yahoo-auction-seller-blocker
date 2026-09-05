# プライバシーポリシー / Privacy Policy

**拡張機能名:** ヤフオク出品者ブロッカー
**バージョン:** 1.0.0
**最終更新日:** 2026年8月31日

---

## 1. 収集する情報

**この拡張機能は、いかなる個人情報も収集・送信・共有しません。**

外部サーバーへの通信を行うコードは一切含まれておらず、開発者を含む第三者がユーザーのデータを参照する手段はありません。

## 2. ブラウザ内に保存される情報

すべてブラウザのローカル領域（`chrome.storage`）に保存され、端末の外には出ません。

| 保存先 | キー | 内容 | 目的 |
| --- | --- | --- | --- |
| `chrome.storage.sync` | `yasbSettings` | 表示方法などの設定 | 設定の保持 |
| `chrome.storage.sync` | `yasbIds0`〜 | ユーザーが登録した出品者IDのリスト（100件ずつ分割） | 非表示対象の判定 |
| `chrome.storage.local` | `yasbNames` | 出品者IDと、登録時の商品名（一覧での目印） | ブロックリストの表示 |
| `chrome.storage.local` | `yasbDonate` | 累計の非表示件数、支援案内の表示済み／非表示フラグ | 支援の案内を一度だけ出すための判定 |

`chrome.storage.sync` は Chrome 標準の同期機能です。ユーザーが Chrome にログインし同期を有効にしている場合に限り、設定が同一アカウントのブラウザ間で同期されます。同期は Google のアカウント機能によるもので、開発者のサーバーは経由しません。同期を望まない場合は Chrome の同期設定で「拡張機能」を除外してください。

## 3. 閲覧内容の扱い

拡張機能は Yahoo!オークションの検索結果ページ上で、商品カードに含まれる出品者IDを読み取ります。これはページ上の表示を切り替えるためだけに使用され、**保存も送信も行いません**。検索キーワード、閲覧履歴、Yahoo!アカウント情報、Cookie等を読み取ることはありません。

## 4. 権限について

| 権限 | 用途 |
| --- | --- |
| `storage` | 上記のブロックリストと設定をブラウザ内に保存するため |
| `auctions.yahoo.co.jp` へのコンテンツスクリプト | 検索結果ページ上で該当商品を非表示にするため |

これ以外の権限は要求しません。他のサイトの内容にアクセスすることはできません。

## 5. 外部リンクについて

ポップアップおよび検索結果のバナーに、開発者支援ページ（Ko-fi: https://ko-fi.com/novastriker）への任意のリンクを設置しています。**クリックした場合のみ**新しいタブで開きます。クリックの有無は記録されず、外部へ送信されることもありません。支援は完全に任意であり、支援の有無によって拡張機能の動作や機能が変わることは一切ありません。

## 6. 第三者への提供

一切ありません。収集していないため、販売・譲渡・分析利用のいずれも発生しません。

## 7. データの削除

Chrome の拡張機能管理画面から本拡張機能を削除すると、保存されたすべてのデータが同時に削除されます。ブロックリストのみを消したい場合は、ポップアップから各出品者の「解除」を押してください。

## 8. 免責

本拡張機能は個人開発の非公式ツールであり、ヤフー株式会社および LINEヤフー株式会社とは一切関係がありません。「Yahoo!オークション」「ヤフオク!」は同社の商標です。

## 9. 変更について

本ポリシーを変更する場合は、拡張機能の更新時に本ファイルを更新し、バージョン番号を改めます。

## 10. お問い合わせ

Chrome ウェブストアの掲載ページよりご連絡ください。

---

# Privacy Policy (English Summary)

This extension does **not** collect, transmit, or share any personal information. It contains no network requests to any server operated by the developer or any third party.

All data stays in the browser: the user's block list and display settings are stored in `chrome.storage.sync`, item labels in `chrome.storage.local`, and a local counter used to show a one-time support notice is stored in `chrome.storage.local`. Seller IDs on Yahoo! Auctions search pages are read only to decide which listings to hide; they are never stored or transmitted. The only permission requested is `storage`, plus a content script limited to `auctions.yahoo.co.jp`. Uninstalling the extension deletes all stored data.

This is an unofficial, independently developed tool and is not affiliated with LY Corporation (Yahoo! JAPAN).
