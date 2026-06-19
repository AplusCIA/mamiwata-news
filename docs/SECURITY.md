# Security Guidelines - Mamiwata News

## Authentication
- ✅ JWT with RS256
- ✅ Password hashing (bcrypt 12 rounds)
- ✅ OAuth2 providers
- ✅ 2FA support
- ✅ Session timeout

## Data Protection
- ✅ HTTPS/TLS 1.3 only
- ✅ HSTS header (1 year)
- ✅ Secure cookies
- ✅ Input validation
- ✅ No sensitive data in logs

## API Security
- ✅ Rate limiting
- ✅ CORS configured
- ✅ CSRF protection
- ✅ Input sanitization
- ✅ XSS prevention

## Environment Variables

**NEVER commit `.env` files!**

```bash
echo ".env" >> .gitignore
cp .env.example .env.local
```

## Security Audits

- Weekly: `npm audit`
- Monthly: Dependency updates
- Quarterly: Penetration testing