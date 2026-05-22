# Claude Code 講習会 デモ用リポジトリ

Claude Code 講習会で使う**デモ＆ハンズオン用**のリポジトリです。

## このリポジトリの構成

```
claude-code-demo/
├── README.md                   # このファイル
├── index.html                  # トップページ（参加者ページ一覧）
├── /demo/
│   └── headline.html           # 発表者デモ用（受講者は触らない）
└── /participants/
    ├── README.md              # 参加者向けの作り方ガイド
    ├── _template.html         # コピー元テンプレ
    └── <あなたの名前>.html    # 各受講者がここに自分のページを作る
```

## 受講者の方へ

`/participants/` の中に、**ご自身の好きな内容で1ページ**を作っていただきます。
題材は自由：自己紹介でも、お気に入りの何かでも、ミニ作品でも、なんでもOKです。

### 進め方（全部 Claude に日本語で頼めばOK）

1. `participants/_template.html` をコピーして `participants/<あなたの名前>.html` を作る
2. Claude に「こういう内容を入れて」「色をこう変えて」と頼む
3. `index.html` の参加者リンク一覧にも自分のリンクを1行追加
4. 完成したら commit & push → PR を作る、まで Claude に頼む

操作（ファイルコピー、編集、git操作、PR作成）はすべて **Claude に日本語で頼めばOK** です。

### お決まりプロンプト

| やりたいこと | Claudeへの依頼例 |
|---|---|
| ページの雛形作成 | `participants/_template.html をコピーして participants/taro.html を作って` |
| 内容を入れる | `taro.html を、私のプロフィールページにして。名前はXX、趣味はYY、好きな本はZZ` |
| 色やデザイン調整 | `背景を薄いピンクに、見出しの色を濃い緑にして` |
| 索引に追加 | `index.htmlの参加者リンク一覧に、私のページ taro.html を追加して` |
| 一連の操作を頼む | `新しいブランチを切って上の変更をして、commit & push、PRまで作って` |

### ルール

- 自分のファイル（`participants/<自分の名前>.html`）と `index.html` の自分の行 **以外は触らない**
- 機密情報・個人情報は **載せない**
- **公開リポジトリ**なので、公開されて困るものは書かない

### 動作確認

`participants/<あなたの名前>.html` を Finder からダブルクリックすればブラウザで開いて見えます（サーバー起動は不要）。

## 発表者デモ用

`/demo/headline.html` は発表者デモ用です。受講者は触らないでください。
