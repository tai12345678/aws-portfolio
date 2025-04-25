# AWSポートフォリオサイト

このリポジトリは、AWSの無料枠を活用して作成した静的ウェブサイトのポートフォリオです。  
主にフロントエンド開発とクラウドホスティングに焦点を当てています。

---

##  公開URL（CloudFront経由）
[https://d3145qfbwv744j.cloudfront.net]

---

##  構成

- `index.html`：トップページ（自己紹介・スキル一覧）
- `contact.html`：問い合わせフォーム（HTMLのみ）
- `style.css`：シンプルなレスポンシブデザイン

---

## 使用技術・サービス

| 分野 | 使用内容 |

| フロントエンド | HTML / CSS |

| クラウドホスティング | AWS S3 + CloudFront |

| ドメイン | CloudFront デフォルトドメイン利用|

| バージョン管理 | Git / GitHub |

---

## デプロイ手順（ローカル → S3）

```bash
aws s3 sync . s3://02-portfolio-sato --delete
