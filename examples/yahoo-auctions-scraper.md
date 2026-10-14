# Yahoo! Auctions Japan Scraper Example

## Overview
Scrape Yahoo! Auctions Japan for product listings, prices, and auction status.

## Setup
```bash
echo "APIFY_TOKEN=your_token" >> .env
```

## Run
```bash
python3 run_actor.py --name yahoo-auctions-japan-scraper --query "レアカード" --max-items 30
```

## Output Schema
- title: str
- current_price: int
- end_time: datetime
- seller: str
- url: str
- bid_count: int

## Notes
- Anonymous scraping supported
- Pagination: up to 100 items per query
- Use for: price history, rare item tracking

## Apify Link
https://apify.com/atushi1841/yahoo-auctions-japan-scraper

## Smithery Install
```bash
npx -y smithery cli install @atushi1841/yahoo-auctions-japan-scraper
```