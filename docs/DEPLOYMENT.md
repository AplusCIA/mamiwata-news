# Deployment Guide - Mamiwata News

## Production Checklist

- [ ] Environment variables configurés
- [ ] SSL/TLS certificates
- [ ] Database backups configurés
- [ ] Monitoring & alerts activés
- [ ] CDN configuré
- [ ] Email service configuré
- [ ] Payment gateway (Stripe) testé
- [ ] Security audit passé

## Frontend Deployment (Vercel)

### Via GitHub
1. Push vers `main` branch
2. Vercel déclenche automatiquement le déploiement
3. Production URL: https://mamiwata-news.com

## Backend Deployment

### Option 1: Railway
```bash
npm install -g railway
cd backend
railway login
railway deploy
```

### Option 2: Docker Compose
```bash
docker-compose -f docker-compose.prod.yml up -d
```

## Database Backup

```bash
mongodump --uri="mongodb://admin:password@mongo:27017/mamiwata-news" \
  --out=/backups/$(date +%Y%m%d)
```

## Monitoring

```bash
# Health Check
curl https://api.mamiwata-news.com/api/v1/health
```