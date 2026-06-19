# API Documentation - Mamiwata News

## Base URL
```
Production: https://api.mamiwata-news.com/api/v1
Development: http://localhost:5000/api/v1
```

## Authentication

Tous les endpoints protégés requièrent un JWT token:

```bash
Authorization: Bearer <token>
```

## Endpoints Principaux

### Articles

#### GET /articles
Lister les articles
```bash
curl http://localhost:5000/api/v1/articles?page=1&limit=10&category=politique
```

#### GET /articles/:id
Récupérer un article
```bash
curl http://localhost:5000/api/v1/articles/123
```

#### POST /articles (Admin)
Créer un article
```bash
curl -X POST http://localhost:5000/api/v1/articles \
  -H "Authorization: Bearer <token>" \
  -H "Content-Type: application/json" \
  -d '{"title": "Article", "content": "...", "category": "politique"}'
```

## Pagination

Tous les endpoints de liste supportent:
- `page` (default: 1)
- `limit` (default: 10, max: 100)
- `sort` (field:direction)

## Rate Limiting

- 100 requests par 15 minutes par IP
- Headers:
  - `X-RateLimit-Limit: 100`
  - `X-RateLimit-Remaining: 99`
  - `X-RateLimit-Reset: 1234567890`