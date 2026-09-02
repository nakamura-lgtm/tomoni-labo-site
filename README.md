# tomoni Labo サイトリニューアル

株式会社ハーバルアイの健康食品ECブランド「**tomoni Labo(トモニラボ)**」のサイトリニューアル。
機能性表示食品「**コレステップ**」の販売強化を目的に、現行サイト( https://tomoni-labo.com/ ・STUDIO製)を静的HTML/CSSで作り直したもの。

## 確認用URL

| ページ | URL |
|---|---|
| トップ | https://nakamura-lgtm.github.io/tomoni-labo-site/ |
| tomoni Laboについて | https://nakamura-lgtm.github.io/tomoni-labo-site/about.html |
| 商品一覧 | https://nakamura-lgtm.github.io/tomoni-labo-site/products.html |

デザイン案(Claudeカンバス): https://claude.ai/code/artifact/7f1b56ed-19b3-4965-978e-d3f6c6c5d11e

## ファイル構成

```
├── index.html      … トップページ
├── about.html      … tomoni Laboについて(ブランドページ)
├── products.html   … 商品一覧
├── css/style.css   … 全ページ共通スタイル(レスポンシブ: 1080px/900px/560px)
└── assets/         … ロゴ・商品画像
```

## 更新の手順

1. 各HTML・`css/style.css` を編集
2. `git add -A && git commit && git push` → 1〜2分でGitHub Pagesに反映

## デザイン仕様(B案「ともに・ウォーム」)

- **配色**: クリーム地 `#faf3e7`、メイン=ロゴのオレンジ `#e8590c` / `#c2410c`、文字=ブラウン `#3d2c20` / `#46352a`、商品セクションのみパッケージ準拠の深緑 `#0f3d28`、LINEボタン=`#06c755`
- **フォント**: 見出し=Zen Maru Gothic、本文=Zen Kaku Gothic New(Google Fonts)
- **キャラクターは使用しない**(確定済み)
- トップ構成: ヒーロー(コンセプトコピー+商品画像+初回価格バッジ)→ 信頼バー → tomoni Laboの約束(「ともに」5連)→ お悩み共感 → 商品セクション(W対策・価格・CTA)→ コラム/お知らせ → サポート → 注意書き → フッター

## ブランドコンセプト

> 自分らしく輝くために 今を、そしてこれからを「ともに」
> 「ともに」悩み 「ともに」頑張り 「ともに」叶え 「ともに」笑う そして「ともに」明日へ

## 制作の経緯(2026-09-02)

1. 現状調査 — 現サイトはSTUDIO製。購入・ログインは shop.tomoni-labo.com(ecforce)に分離
2. 方針決定 — まずデザイン案のみ/トップページから/狙いはコレステップ販売強化
3. デザイン案2方向(案A クリーン・トラスト/案B ともに・ウォーム)を作成
4. キャラクターは使わない方針に変更
5. B案ベースに決定。案Aの信頼要素(信頼バー・お悩み共感・W対策ブロック)を統合
6. HTML/CSSで実装、GitHub Pagesで公開
7. 「tomoni Laboについて」「商品一覧」ページを追加

## 残タスク・要確認

- [ ] 単品購入リンクの商品URL確認(現サイトの `P-CLSXXXXX-01O00000` を流用中。ecforce管理画面で要確認)
- [ ] aboutページ「ともに」5つの約束の説明文レビュー
- [ ] コラム・お知らせの記事リンク(現在は一覧ページへのリンク)
- [ ] 本番切り替え: tomoni-labo.com ドメインをSTUDIOから切り替える手順の整理
- [ ] コラム・お知らせの更新運用をどうするか(STUDIOに残す/移行する)
- [ ] ファビコン・OGP画像の用意

---

🤖 Generated with [Claude Code](https://claude.com/claude-code)
