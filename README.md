# 🌊 Mamiwata News - La Minute Mamiwata

**Plateforme d'actualités dynamique et moderne pour la Guinée et l'Afrique de l'Ouest**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js](https://img.shields.io/badge/Node.js-20+-green)](https://nodejs.org/)
[![Next.js](https://img.shields.io/badge/Next.js-14+-blue)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5+-blue)](https://www.typescriptlang.org/)
[![Docker](https://img.shields.io/badge/Docker-Ready-2496ED)](https://www.docker.com/)

## 🎯 Mission

**Mamiwata News** est une plateforme d'actualités révolutionnaire qui apporte les meilleures pratiques technologiques à l'Afrique de l'Ouest. Inspirée par le mythe de Mami Wata (force de transformation et fluidité), notre plateforme incarne l'adaptation, la modernité et l'excellence.

## ✨ Caractéristiques Principales

### 📱 Expérience Utilisateur
- ✅ Design Responsive & Mobile-First
- ✅ Dark/Light Mode automatique
- ✅ Accessibilité WCAG 2.1 AA
- ✅ Performance optimale (Core Web Vitals 100/100)
- ✅ PWA Support
- ✅ Offline mode

### 📰 Gestion de Contenu
- ✅ Création/édition d'articles en temps réel
- ✅ Support multimédia (images, vidéos, audios)
- ✅ Live coverage & breaking news
- ✅ 12+ catégories d'actualités
- ✅ Planification de publication
- ✅ Versioning d'articles

### 🔐 Sécurité & Conformité
- ✅ JWT + OAuth2 (Google, Facebook)
- ✅ RGPD & CCPA compliance
- ✅ Chiffrement des données sensibles
- ✅ Rate limiting & DDoS protection
- ✅ Audit logs complets
- ✅ 2FA & biométrie

### 🎯 Engagement
- ✅ Commentaires modérés en temps réel
- ✅ Système de notification push
- ✅ Newsletter personnalisée
- ✅ Système de recommandations IA
- ✅ Social sharing intégré
- ✅ Save & reading history

### 📊 Analytics
- ✅ Tableau de bord temps réel
- ✅ Google Analytics 4 + Mixpanel
- ✅ Trending topics automatiques
- ✅ Engagement metrics
- ✅ Audience segmentation

### 💰 Monétisation
- ✅ Abonnements premium (Stripe)
- ✅ Publicités programmatiques
- ✅ Sponsored content
- ✅ Partenariats média

## 🛠️ Stack Technologique

### Frontend
```
Framework:    Next.js 14 + React 18
Language:     TypeScript
Styling:      Tailwind CSS + Framer Motion
State:        Redux Toolkit + Redux Persist
API:          TanStack React Query + Axios
UI:           Radix UI + Headless UI
Forms:        React Hook Form + Zod
Charts:       Recharts
SEO:          next-seo + Schema.org
Analytics:    Mixpanel + GA4
```

### Backend
```
Runtime:      Node.js 20 LTS
Framework:    Express.js 4 + TypeScript
Database:     MongoDB 7 + Mongoose
Cache:        Redis 7
Search:       Elasticsearch 8 (optional)
Auth:         Passport.js + JWT
File Storage: AWS S3 + Cloudinary
Email:        SendGrid
Payment:      Stripe
Queue:        Bull (Redis-based)
```

### DevOps
```
Containers:   Docker + Docker Compose
CI/CD:        GitHub Actions
Deploy:       Vercel / AWS / Railway
Monitoring:   Sentry + DataDog
Logging:      Winston + ELK
CDN:          Cloudflare
```

## 📁 Structure du Projet

```
mamiwata-news/
├── frontend/                    # Application Next.js (React)
├── backend/                     # API Node.js/Express
├── docker/                      # Docker configuration
├── database/                    # Database seeds & migrations
├── scripts/                     # Utility scripts
├── docs/                        # Documentation
├── docker-compose.yml           # Multi-container setup
├── package.json                 # Root monorepo config
├── .env.example                 # Environment template
└── CONTRIBUTING.md              # Contribution guide
```

## 🚀 Quick Start

### Prérequis
```bash
- Node.js 20+
- Docker & Docker Compose
- Git
```

### Installation (2 minutes)

```bash
# 1. Clone le repository
git clone https://github.com/AplusCIA/mamiwata-news.git
cd mamiwata-news

# 2. Installation avec Docker (recommandé)
docker-compose up -d

# 3. Initialisation de la base de données
npm run db:seed

# 4. Accès
http://localhost:3000       # Frontend
http://localhost:5000/api   # Backend API
http://localhost:5000/api/docs  # API Documentation
```

### Développement Local (sans Docker)

```bash
# Terminal 1 - Backend
cd backend
npm install
npm run dev

# Terminal 2 - Frontend
cd frontend
npm install
npm run dev
```

## 📚 Documentation

| Document | Description |
|----------|-------------|
| [API.md](docs/API.md) | Documentation API REST complète |
| [ARCHITECTURE.md](docs/ARCHITECTURE.md) | Architecture système |
| [DEPLOYMENT.md](docs/DEPLOYMENT.md) | Guide de déploiement production |
| [DATABASE.md](docs/DATABASE.md) | Schémas MongoDB |
| [SECURITY.md](docs/SECURITY.md) | Guide de sécurité |
| [CONTRIBUTING.md](CONTRIBUTING.md) | Guide de contribution |

## 🧪 Tests

```bash
# Tests Frontend
npm run test:frontend

# Tests Backend
npm run test:backend

# Tests E2E (Cypress)
npm run test:e2e

# Coverage complet
npm run test:coverage
```

## 🔐 Sécurité

- ✅ HTTPS/TLS 1.3
- ✅ JWT RS256 signing
- ✅ Helmet.js headers
- ✅ CORS configuré
- ✅ Rate limiting
- ✅ Input sanitization
- ✅ CSRF protection
- ✅ Bcrypt hashing (12 rounds)
- ✅ Audit logs
- ✅ Snyk security scans

## ⚡ Performance

### Cibles
- LCP < 2.5s ✅
- FID < 100ms ✅
- CLS < 0.1 ✅
- Lighthouse 95+ ✅

### Optimisations
- Image optimization (WebP)
- Code splitting
- SSR/SSG
- Redis multi-layer caching
- CDN global
- Database indexing

## 📱 Catégories d'Actualités

- 🏛️ Politique
- 💼 Économie
- 🌍 International
- ⚖️ Justice & Légal
- 👥 Société
- 🎓 Éducation
- 🏥 Santé
- ⚽ Sports
- 🎬 Culture & Divertissement
- 🌱 Environnement
- 💻 Technologie
- 🏠 Immobilier

## 🚀 Déploiement Production

```bash
# Frontend sur Vercel
vercel deploy --prod

# Backend sur Railway/AWS
railway deploy

# Ou Docker push personnalisé
docker-compose -f docker-compose.prod.yml up -d
```

Voir [DEPLOYMENT.md](docs/DEPLOYMENT.md) pour les détails complets.

## 🌐 Support Multilingue

- 🇫🇷 Français (FR) - Principal
- 🇬🇧 Anglais (EN) - Support
- 🇬🇳 N'ko (NQO) - Futur
- 🇬🇳 Soussou (SUQ) - Futur

## 🤝 Contribution

Contributions bienvenues ! Voir [CONTRIBUTING.md](CONTRIBUTING.md)

```bash
# Fork → Branch → Commit → Push → PR
git checkout -b feature/amazing-feature
git commit -m 'feat: add amazing feature'
git push origin feature/amazing-feature
```

## 📞 Support & Contact

- 📧 **Email**: support@mamiwata-news.com
- 🐦 **Twitter**: [@MamiwataNews](https://twitter.com/mamiwatanews)
- 💬 **Discord**: [Community Server](https://discord.gg/mamiwata)
- 📖 **Docs**: [docs.mamiwata-news.com](https://docs.mamiwata-news.com)
- 🌐 **Website**: [www.mamiwata-news.com](https://www.mamiwata-news.com)

## 📝 License

MIT License - Voir [LICENSE](LICENSE)

---

**Mamiwata News - Informer, Inspirer, Transformer** 🌊

*Made with ❤️ for Guinea 🇬🇳 & West Africa 🌍*