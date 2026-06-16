# Supply Chain Search and Discovery API

> Stop wasting hours hunting for parts, suppliers, and logistics data across disconnected systems—our API gives you one endpoint to search and discover everything in your supply chain instantly.

The Supply Chain Search and Discovery API solves the fragmentation problem by aggregating data from multiple sources into a single, lightning-fast REST endpoint. It's the best solution because it unifies siloed inventories, supplier databases, and shipment records, letting you find what you need in milliseconds without complex integrations.

## What's Included

- Real-time search across all your supply chain data sources
- Multi-source aggregation (ERP, WMS, supplier portals, logistics APIs)
- Advanced filtering by SKU, location, lead time, and cost
- RESTful API with simple JSON responses and webhook support
- Automatic data normalization and deduplication

## Who Is This For

- Supply chain managers who need to locate parts across multiple warehouses instantly
- Procurement teams searching for alternative suppliers and pricing in real time
- Logistics coordinators tracking shipments and inventory across carriers
- Developers building custom supply chain dashboards or automation workflows

## How It Works

Get your API key via Gumroad, then integrate with a single line of code—send a GET or POST request to our endpoint with your search terms. The API returns structured JSON with matched items, sources, and metadata. No complex setup, no data migration; just plug and search.

## Frequently Asked Questions

**What data sources does the API search by default?**
The API searches across your connected systems—ERP, WMS, supplier portals, and logistics APIs. You can onboard custom sources via our simple configuration endpoint.

**How fast are search results returned?**
Typical response time is under 200ms for queries across up to 10 data sources, depending on your network latency.

**Is this a one-time purchase or subscription?**
The $32.49 price is a one-time purchase for a lifetime license, including 10,000 API calls per month. Higher usage tiers are available.

**Can I use this API with my existing supply chain automation tools?**
Yes, it's a standard REST API compatible with any HTTP client, so it works with Zapier, Power Automate, custom scripts, and more.

**What security measures are in place?**
All API calls require an SSL-encrypted connection and an API key. Data in transit is encrypted with TLS 1.2+.

## What You Get

- Instant digital download
- Complete REST API with full documentation
- Free updates for life — pay once, own forever
- Setup guide and usage instructions

**Instantly unify your supply chain search—click to get your lifetime access now for just $32.49.**

## Features

- Full REST API

## Quick Start

```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. Configure environment
cp .env.example .env
# Edit .env with your settings

# 3. Run locally
uvicorn main:app --reload --port 8000

# 4. View interactive docs
open http://localhost:8000/docs
```

## Docker Deployment

```bash
# Build and run
docker compose up -d

# Check health
curl http://localhost:8000/health
```

## Authentication

Get a token first:
```bash
curl -X POST "http://localhost:8000/auth/token?username=admin&password=admin123"
```

Use the token in subsequent requests:
```bash
curl -H "Authorization: Bearer YOUR_TOKEN" http://localhost:8000/items
```

## API Endpoints

| Method | Path | Description |
|--------|------|-------------|
| GET | `/health` | System health |
| POST | `/auth/token` | Get JWT token |
| GET | `/items` | List all items |
| POST | `/items` | Create item |
| GET | `/items/{id}` | Get item |
| PATCH | `/items/{id}` | Update item |
| DELETE | `/items/{id}` | Delete item |
| GET | `/stats` | API statistics |

Full interactive docs: `http://localhost:8000/docs`

## Rate Limits

| Endpoint | Limit |
|----------|-------|
| `/auth/token` | 10/minute |
| `GET /items` | 60/minute |
| `POST /items` | 30/minute |
| `DELETE /items` | 20/minute |

## Running Tests

```bash
pip install pytest httpx
pytest tests/ -v
```

## Production Notes

- Change `SECRET_KEY` in `.env` before deploying
- Replace in-memory `_db` with a real database
- Add proper user management to `auth.py`
- Configure `ALLOWED_ORIGINS` for CORS
- Use Nginx/Traefik as reverse proxy

## License

MIT


---

## Free vs Pro

| Feature | Free | Pro |
|---------|:----:|:---:|
| 100 requests/day | Yes | Yes |
| Standard endpoints | Yes | Yes |
| JSON responses | Yes | Yes |
| Unlimited requests | - | Yes |
| Premium endpoints | - | Yes |
| Batch processing | - | Yes |
| Webhook notifications | - | Yes |
| SLA guarantee | - | Yes |
| Priority support | - | Yes |

### Upgrade to Pro

Get the full version with all premium features, priority support, and lifetime updates.

**[Get Pro Version](https://buy.stripe.com/eVq6oH12D2k41debzScZg3o)**

- [Buy Now (Stripe)](https://buy.stripe.com/eVq6oH12D2k41debzScZg3o)

