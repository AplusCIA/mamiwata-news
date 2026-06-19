# Contribuer à Mamiwata News

Merci de votre intérêt pour contribuer à Mamiwata News ! Ce document fournit les lignes directrices pour contribuer.

## Code de Conduite

Soyez respectueux et professionnel. Toute discrimination ou harcèlement est inacceptable.

## Comment Contribuer

### 1. Fork & Clone
```bash
git clone https://github.com/YOUR_USERNAME/mamiwata-news.git
cd mamiwata-news
```

### 2. Créer une Branche
```bash
git checkout -b feature/amazing-feature
```

### 3. Commit avec Convention
```bash
git commit -m 'feat: add amazing feature'
```

Types de commits:
- `feat:` - Nouvelle fonctionnalité
- `fix:` - Bug fix
- `docs:` - Documentation
- `style:` - Code style (sans change de logique)
- `refactor:` - Refactoring
- `test:` - Tests
- `chore:` - Maintenance

### 4. Push & Pull Request
```bash
git push origin feature/amazing-feature
```

## Standards de Code

### Frontend
- TypeScript obligatoire
- Lint: ESLint + Prettier
- Tests: Jest + React Testing Library
- Composants fonctionnels avec hooks

### Backend
- TypeScript obligatoire
- Lint: ESLint
- Tests: Jest + Supertest
- API RESTful

## Testing

```bash
# Tests unitaires
npm run test

# Tests E2E
npm run test:e2e

# Coverage
npm run test:coverage
```

## Documentation

Toute nouvelle fonctionnalité doit inclure:
- Commentaires dans le code
- Tests
- Documentation mise à jour

## Questions ?

Ouvrez une issue ou contactez support@mamiwata-news.com