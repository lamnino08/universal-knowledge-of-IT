# Fix Subdomain Localhost Auth Cookie Sharing & Redirect Loop

**Category:** troubleshooting
**Type:** Continuous Self-Learning Pattern
**Recorded At:** 2026-09-18

## 🔍 Problem / Context
When accessing movie.localhost:4000, clicking login causes an infinite reload loop back to movie.localhost:4000 instead of displaying the sign-in form or recognizing the session.

## 💡 Solution & Implementation
Set authCookieDomain to 'localhost' in local development (and '.infb.app' in production) so auth cookies (token, refresh_token, next-auth) are shared across all subdomains (*.localhost:4000). Also ensure logout deletes both domain-scoped and host-only cookies.

## ⚠️ Anti-Patterns / Pitfalls
Setting auth cookies with domain undefined in local development creates Host-only cookies on localhost that cannot be sent to subdomains like movie.localhost, causing an infinite redirect loop with isGuest route protection.

## 📂 Related Files
- `workspace/web/actions/user/user.action.ts`
- `workspace/web/lib/auth-options.ts`
- `workspace/web/constant/permission.tsx`

