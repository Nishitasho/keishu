# 焼肉慶州 公式サイト

静的HTML/CSS/JSで制作した8ページ構成のブランドサイトです。

## ローカル起動

```bash
python3 -m http.server 4173 -d outputs/keishu-brand-site
```

## Cloudflare Pages

ビルドコマンドなし、出力ディレクトリは `outputs/keishu-brand-site` を指定します。独自ドメイン公開時は `sitemap.xml` と canonical の `https://example.com` を本番URLへ変更してください。

## 更新方法

店舗情報、営業時間、メニュー、FAQ、NEWS、外部リンクは `assets/data/*.json` に同内容を保存しています。HTML側に反映する場合は同じ文言を更新してください。

## 画像差し替え

Drive素材が取得できなかったため、料理写真・店内写真は写真差し替え枠として実装しています。提供素材を `assets/images/` に配置し、各 `.photo-slot` を `<picture>` または `<img>` に置換してください。料理写真の生成AI利用や外部転載は行っていません。

## 注意

プライバシーポリシー、サイトポリシーは公開前に店舗側または専門家の最終確認が必要です。
