# Database Schema - Mamiwata News

## MongoDB Collections

### Users
```javascript
db.users.createIndex({ email: 1 }, { unique: true });
```

### Articles
```javascript
db.articles.createIndex({ slug: 1 }, { unique: true });
db.articles.createIndex({ category: 1, publishedAt: -1 });
db.articles.createIndex({ title: "text", content: "text" });
```

### Comments
```javascript
db.comments.createIndex({ article: 1, createdAt: -1 });
db.comments.createIndex({ author: 1 });
```

### Categories
```javascript
db.categories.createIndex({ slug: 1 }, { unique: true });
```