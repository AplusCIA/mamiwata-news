# Architecture - Mamiwata News

## Vue d'ensemble

Mamiwata News utilise une architecture **monorepo scalable** avec séparation Frontend/Backend.

## Design Patterns

### 1. MVC Pattern
- **Models**: MongoDB schemas + TypeScript interfaces
- **Views**: React components
- **Controllers**: Route handlers in Express

### 2. Service Layer Pattern
- Business logic séparé des routes
- Réutilisabilité du code
- Testabilité améliorée

### 3. Repository Pattern (Mongoose)
- Abstraction de la BD
- Requêtes centralisées
- Migration facile

## Flux de Données

```
Utilisateur
    ↓
[Frontend]
    ↓ (HTTP Request + JWT)
[API Route]
    ↓
[Middleware] (Auth, Validation)
    ↓
[Controller]
    ↓
[Service] (Business Logic)
    ↓
[MongoDB] ← Cache (Redis)
    ↓
[Response]
    ↓
[Frontend State] (Redux)
    ↓
[UI Update]
```

## Scalabilité

### Horizontal Scaling
- Multiple instances derrière load balancer
- Session store in Redis
- Database replica set

### Vertical Scaling
- Optimize queries (indexing)
- Caching strategies
- Code splitting & lazy loading