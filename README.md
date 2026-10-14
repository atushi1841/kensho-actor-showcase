# kensho-actor-showcase

**55+ Free Japanese Market Data Scrapers** — ready-to-use Apify Actors for EC, auction, and marketplace data.

[![GitHub stars](https://img.shields.io/github/stars/atushi1841/kensho-actor-showcase)](https://github.com/atushi1841/kensho-actor-showcase)
[![Smithery](https://smithery.ai/badge/@atushi1841/kensho-actor-showcase)](https://smithery.ai/@atushi1841/kensho-actor-showcase)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![X (Twitter)](https://img.shields.io/twitter/url?url=https%3A%2F%2Fx.com%2Fatushi1841)](https://x.com/atushi1841)

Kensho Project のオープンソース Apify Actor コレクション。メルカリ・Yahoo!オークション・楽天など日本の主要EC・マーケットプレイスのデータを無料で取得できるスクリプトが59本揃っています。

---

## 🚀 Quick Start

```bash
# 1. Apify アカウントを作成: https://apify.com
# 2. プロジェクトをクローン
git clone https://github.com/atushi1841/kensho-actor-showcase.git
cd kensho-actor-showcase

# 3. token を設定
echo "APIFY_TOKEN=your_token_here" > .env

# 4. Actor を実行
python3 run_actor.py --name mercari-japan-search-scraper --max-items 100
```

---

## 📊 Top 5 Actors（実行回数順）

### 1. Japan Market MCP — cross-shop price comparison
| 項目 | 値 |
|------|-----|
| 合計実行 | 603回 |
| カテゴリ | 比較検索 |
| 用途 | 複数ショップの価格を一度に比較 |

**Apify**: [japan-market-mcp](https://apify.com/atushi1841/japan-market-mcp)
**Smithery**: `npx -y smithery cli install @atushi1841/japan-market-mcp`

---

### 2. Japan OffMall Market Scraper — ハードオフ/オフモール
| 項目 | 値 |
|------|-----|
| 合計実行 | 339回 |
| カテゴリ | 中古品 |
| 用途 | ハードオフ・オフモールの出品価格取得 |

**Apify**: [japan-offmall-market-scraper](https://apify.com/atushi1841/japan-offmall-market-scraper)
**Smithery**: `npx -y smithery cli install @atushi1841/japan-offmall-market-scraper`

---

### 3. Mandarake Auction Scraper — まんだらけオークション
| 項目 | 値 |
|------|-----|
| 合計実行 | 242回 |
| カテゴリ | ホビー/アニメ |
| 用途 | まんだらけオークションの落札価格・出品履歴 |

**Apify**: [mandarake-auction-scraper](https://apify.com/atushi1841/mandarake-auction-scraper)
**Smithery**: `npx -y smithery cli install @atushi1841/mandarake-auction-scraper`

---

### 4. Tackleberry Japan Fishing Tackle Scraper — タックルベリー
| 項目 | 値 |
|------|-----|
| 合計実行 | 215回 |
| カテゴリ | 釣具 |
| 用途 | 釣具店の価格・在庫情報取得 |

**Apify**: [tackleberry-japan-fishing-tackle-scraper](https://apify.com/atushi1841/tackleberry-japan-fishing-tackle-scraper)
**Smithery**: `npx -y smithery cli install @atushi1841/tackleberry-japan-fishing-tackle-scraper`

---

### 5. Japan Used Camera Market Scraper — 中古カメラ
| 項目 | 値 |
|------|-----|
| 合計実行 | 107回 |
| カテゴリ | カメラ |
| 用途 | キタムラ・カメラ市場の中古価格調査 |

**Apify**: [japan-used-camera-market-scraper](https://apify.com/atushi1841/japan-used-camera-market-scraper)
**Smithery**: `npx -y smithery cli install @atushi1841/japan-used-camera-market-scraper`

---

## 📚 Full Catalog（全59本）

| # | Actor名 | 実行回 | 用途 |
|---|---------|--------|------|
| 1 | japan-market-mcp | 603 | 横断価格比較 |
| 2 | japan-offmall-market-scraper | 339 | ハードオフ価格 |
| 3 | mandarake-auction-scraper | 242 | まんだらけオークション |
| 4 | tackleberry-japan-fishing-tackle-scraper | 215 | 釣具価格 |
| 5 | japan-used-camera-market-scraper | 107 | 中古カメラ |
| 6 | japan-anime-figure-price-data | 106 | アニメフィギュア |
| 7 | japan-kakaku-price-search | 104 | 価格.com |
| 8 | japan-watch-market-scraper | 92 | 腕時計 |
| 9 | japan-luxury-brand-market-scraper | 89 | 高級ブランド |
| 10 | japan-used-instrument-market-scraper | 88 | 楽器 |
| 11 | mercari-japan-search-scraper | 88 | メルカリ |
| 12 | komehyo-japan-brand-scraper | 82 | コメ.hy |
| 13 | kitamura-japan-used-camera-scraper | 77 | キタムラ |
| 14 | iosys-japan-used-smartphone-scraper | 73 | スマホ中古 |
| 15 | jackroad-used-watch-scraper | 72 | ジャックロード |
| 16 | surugaya-japan-hobby-prices | 70 | 駿河屋 |
| 17 | japan-rent-market-scraper | 65 | 賃貸 |
| 18 | japan-property-market-scraper | 65 | 不動産 |
| 19 | yahoo-auctions-japan-scraper | 49 | Yahooオークション |
| 20 | dlsite-scraper | 32 | DLsite |
| ... | （全件は`examples/`を参照） | | |

> **全59本の実行例**は[`examples/`](./examples) ディレクトリをご確認ください。

---

## 🛠️ Examples（使用例）

### mercari-scraper（メルカリ）
```bash
python3 run_actor.py --name mercari-japan-search-scraper --query "iPhone 15" --max-items 50
```
**出力**: 商品名・価格・状態・出品者・URL

### yahoo-auctions-scraper（Yahoo!オークション）
```bash
python3 run_actor.py --name yahoo-auctions-japan-scraper --query "レアカード" --max-items 30
```
**出力**: 出品タイトル・現在価格・終了時刻・出品者

### rakuten-scraper（楽天）
```bash
python3 run_actor.py --name rakuten-japan-mcp --query "フィギュア" --max-items 100
```
**出力**: 商品名・価格・レビュー数・楽天ポイント

---

## 🔗 Links

- **Apify Store**: [atushi1841](https://apify.com/atushi1841)
- **Smithery**: [install guide](https://smithery.ai/@atushi1841/kensho-actor-showcase)
- **GitHub**: [github.com/atushi1841/kensho-actor-showcase](https://github.com/atushi1841/kensho-actor-showcase)
- **X (Twitter)**: [@atushi1841](https://x.com/atushi1841)

---

## 📝 License

MIT License — 商用利用・修改・配布可能です。

---

## 🤝 Contributing

1. Fork the repo
2. Create feature branch (`git checkout -b feature/xxx`)
3. Commit changes (`git commit -am 'Add xxx'`)
4. Push to branch (`git push origin feature/xxx`)
5. Create new Pull Request

---

## ⭐ Star this repo

If this helps you, please star ⭐ this repository — it motivates us to add more Japanese market scrapers!

---

## Contact

Questions? Reach out on [X/Twitter](https://x.com/atushi1841) or open an issue on GitHub.