# Mercari Japan Scraper Example

## Overview
Scrape Mercari Japan for product listings, prices, and seller information.

## Setup
```bash
echo "APIFY_TOKEN=your_token" >> .env
pip install -r requirements.txt
```

## Run
```bash
python3 run_actor.py --name mercari-japan-search-scraper --query "iPhone 15" --max-items 50
```

## Output Schema
- product_name: str
- price: int
- condition: str
- seller_id: str
- url: str
- scraped_at: datetime

## Notes
- Mercari requires login for some endpoints
- Rate limit: ~1 request/second
- Best for: price monitoring, availability tracking

## Apify Link
https://apify.com/atushi1841/mercari-japan-search-scraper

## Smithery Install
```bash
npx -y smithery cli install @atushi1841/mercari-japan-search-scraper
```