# Fix 404 Logging as 500 in Observability and Seed BGG Label Taxonomy

**Category:** troubleshooting
**Type:** Continuous Self-Learning Pattern
**Recorded At:** 2026-10-14

## 🔍 Problem / Context
Observability logged 404 NotFoundError as HTTP 500 BaseAppError, and BGG labels from category_groups.json/mechanic_groups.json were missing in production database.

## 💡 Solution & Implementation
1. Set `this.name = this.constructor.name` in BaseAppError so subclasses retain their proper name (NotFoundError, etc.). 2. Add `statusCode` to errorMetadata in OnError.ts. 3. Ensure apiLogger preserves existing 4xx/5xx status codes on c.res.status instead of defaulting to 500. 4. Created database/seed-bgg-labels.ts to populate all 28 groups and 285 BGG labels into MySQL.

## ⚠️ Anti-Patterns / Pitfalls
Do not assume an error logged as 500 is truly an internal server error without checking whether apiLogger.ts or OnError.ts stripped or defaulted the status code. Never use fallback `errorCaptured.statusCode || 500` blindly when c.res.status is already a valid 4xx client response.

## 📂 Related Files
- `workspace/back-end/src/errors/base/baseAppError.ts`
- `workspace/back-end/src/libs/hono/OnError.ts`
- `workspace/back-end/src/middlewares/apiLogger.ts`
- `workspace/back-end/database/seed-bgg-labels.ts`

