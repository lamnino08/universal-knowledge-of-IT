# Auth Gate & Progressive Disclosure Architecture for Private vs Discovery Pages

**Category:** architecture
**Type:** Continuous Self-Learning Pattern
**Recorded At:** 2026-09-24

## 🔍 Problem / Context
Deciding between blocking whole pages with Auth Gate vs keeping pages public with contextual modal prompts, while avoiding false affordances on settings pages.

## 💡 Solution & Implementation
Apply Full-Page Auth Gate (SettingsAuthPrompt) for private identity pages (/settings) and Progressive Disclosure with Contextual Modal Gate (useAuthGateModal) for community discovery pages (/social/members). Follow Form Follows Function to keep only functional sections (Theme, Locale, Profile).

