# 01-infinity.com

株式会社インフィニティ（INFINITY, K.K.）のコーポレートサイト。
GitHub Pages の**プロジェクトサイト**として公開し、独自ドメイン `01-infinity.com` を割り当てている。

## ⚠️ なぜユーザーサイト（YoshitetsuSuzuki.github.io）に置かないか

ユーザーサイトにカスタムドメインを設定すると `yoshitetsusuzuki.github.io` が
そのドメインへリダイレクトされる。あそこには AdMob の `app-ads.txt` が置いてあり、
ちりつも単語のストア登録 sellerUrl が `https://yoshitetsusuzuki.github.io` を指している。
リダイレクトが入ると app-ads.txt の検証が壊れるため、**必ず別リポジトリにする**。

## 構成

- `index.html` … 1ページのみ。依存なし
- `CNAME` … `01-infinity.com`

## DNS（Squarespace の DNS 設定に入れる値）

A レコード（4本）
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```
AAAA レコード（4本）
```
2606:50c0:8000::153
2606:50c0:8001::153
2606:50c0:8002::153
2606:50c0:8003::153
```
CNAME: `www` → `yoshitetsusuzuki.github.io`

**MX レコードには触らないこと**（Google Workspace のメールが止まる）。
