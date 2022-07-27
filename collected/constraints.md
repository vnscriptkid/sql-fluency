# Constraints

- Add a unique index
```sql
CREATE UNIQUE INDEX "wishlists_userId_articleId_usSize_listingId_unique_idx" 
    ON "wishlists" ("userId", "articleId", "usSize", COALESCE("listingId", '11111111-1111-1111-1111-111111111111'))
```

- Add a unique constraint
```sql
ALTER TABLE "wishlishts"
ADD CONSTRAINT "wishlists_userId_articleId_usSize_listingId"
```

- Unique index vs Unique constraint
  - Unique constraint uses unique index behind the scene
  - Creating unique constraint will create unique index
  - Creating unique index won't create unique constraint

