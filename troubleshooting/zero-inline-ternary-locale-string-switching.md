# Zero Inline Ternary Locale String Switching

**Category:** troubleshooting
**Type:** Continuous Self-Learning Pattern
**Recorded At:** 2026-10-08

## 🔍 Problem / Context
AI agents extracting locale from useLocale() and writing inline ternary checks `locale === 'vi' ? 'Tiếng Việt' : 'English'` instead of registering translation keys in @shared/lib/i18n.

## 💡 Solution & Implementation
Always register types in `packages/shared/lib/i18n/.../types.ts`, add bilingual translations to `vi.ts` and `en.ts`, and call `const { t } = useLocale(); t('domain.key')`. Never use `locale` for conditional text rendering.

