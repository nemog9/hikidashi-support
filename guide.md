---
title: 使い方ガイド｜Hikidashi
permalink: /guide/
---

[← Hikidashi トップ]({{ '/' | relative_url }})

# Hikidashi（引き出し）の使い方

集めたものを、すぐ取り出せる引き出し。

記事、動画、投稿、作品など、あとで見返したいものを、タイトル・URL・クリエイター・サムネイル・メモと一緒に集めて、素早く探せる iPhone アプリです。データは端末の中にあり、CSV でいつでも書き出し・読み込みができます。

<p><a href="https://apps.apple.com/jp/app/hikidashi-%E5%BC%95%E3%81%8D%E5%87%BA%E3%81%97/id6823911890" style="display:inline-block;background:#ed7305;color:#ffffff;font-weight:700;font-size:1.05em;line-height:1;padding:14px 26px;border-radius:12px;text-decoration:none;box-shadow:0 2px 6px rgba(237,115,5,0.35);">App Store でダウンロード</a></p>

## いろいろな場所から保存できます

| 使っている場所 | 保存のしかた |
|---|---|
| iPhone の **Safari** | [ショートカット](#safari)（タグなど、画面に出ている内容まで読み取る） |
| X・YouTube・pixiv などの**アプリ** | [共有ボタン](#share)から「Save to Hikidashi」 |
| **PC**（Chrome） | [Chrome 拡張](#chrome)（QR を iPhone で読み取る） |
| ほかのサービスから移りたい | [CSV](#csv)で読み込み |

## Safari から保存する（ショートカット） {#safari}
Safari の共有ボタンから「Hikidashi に保存」を選ぶだけで、開いているページの内容（タイトル、画像、投稿者、pixiv のタグなど）を読み取って、Hikidashi の追加の確認画面を開きます。

1. iPhone で、このリンクを開いて「ショートカットを追加」をタップ:
   **[Hikidashi に保存（iCloud リンク）](https://www.icloud.com/shortcuts/3feab5f321de4e95bbc9d09be8da001a)**
2. 「設定 → ショートカット → 詳細」で、「**スクリプトの実行を許可**」を**オン**にする。
3. Safari で保存したいページを開き、共有ボタン →「**Hikidashi に保存**」をタップする（一覧にないときは、一番下の「アクションを編集」でオン）。
4. Hikidashi が開くので、内容を確かめて追加する。

- **ログインが必要なページや、ブラウザの中で画面を組み立てるページ**（React などで作られたサイト）でも、画面に表示された内容を読めます。
- 読み取りは、Safari の中だけで行い、外部には何も送りません。

## 共有ボタンから保存する（アプリ） {#share}
X、YouTube、pixiv、ブラウザなどの共有ボタンから「**Save to Hikidashi**」を選ぶと、そのページの URL から、タイトル・サムネイル・作者・本文を取得して、保存できます。

- 見つからないときは、共有シートの一番右の「**その他**」から、「Save to Hikidashi」をオンにします。
- 保存前に、画像の候補を選び直したり、カテゴリやメモを編集したりできます。
- X の投稿は、本文がメモに入ります。メモの `#ハッシュタグ` をタップすると、その言葉で検索できます。

## PC から保存する（Chrome 拡張） {#chrome}
PC で見ているページを QR コードにして、iPhone のカメラで読み取るだけで保存できる拡張機能です。サーバーもアカウントも要りません。

- タイトル・サムネイル・作者・本文を自動で取得（YouTube と X は専用の取り方、pixiv はタグも）
- 画像の候補から選べる。QR の上で、内容を編集できる
- 外部には何も送らない（権限はクリックしたタブの読み取りだけ）
- 入れ方と使い方: [hikidashi-clip（GitHub）](https://github.com/nemog9/hikidashi-clip) ／ [最新版のダウンロード](https://github.com/nemog9/hikidashi-clip/releases/latest)

## CSV で出し入れする {#csv}
設定の「CSV をインポート」で読み込み、「CSV をエクスポート」で書き出せます。ほかのアプリやサービスから移るときも、CSV を作れば取り込めます。

- 列は `title, url, creators, thumbnail_url, category, note`（日本語の見出しも可）。クリエイターは「|」で区切って複数指定できます。
- [サンプル CSV]({{ '/sample.csv' | relative_url }})（架空の 6 件）で、すぐ試せます。

## サポート
- [プライバシーポリシー / Privacy Policy]({{ '/privacy-policy' | relative_url }})
- お問い合わせ・不具合の報告: [GitHub Issues](https://github.com/nemog9/hikidashi-support/issues)
