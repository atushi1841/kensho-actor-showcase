# Rakuten Ichiba Scraper Example

## Overview
Collect product data from Rakuten Ichiba — Japan's largest online marketplace.

## Setup
```bash
echo "APIFY_TOKEN=your_token" >> .env
```

## Run
```bash
python3 run_actor.py --name rakuten-japan-mcp --query "フィギュア" --max-items 100
```

## Output Schema
- product_name: str
- price: int
- rating: float
- review_count: int
- rakuten_points: int
- url: str

## Notes
- Requires API key for full access
- Rate limit: 10 req/sec with key
- Best for: market comparison, price intelligence

## Apify Link
https://apify.com/atushi1841/rakuten-japan-mcp

## Smithery Install
```bash
npx -y smithery cli install @atushi1841/rakuten-japan-mcp
```