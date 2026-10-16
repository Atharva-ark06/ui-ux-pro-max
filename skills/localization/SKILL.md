---
name: localization
description: Prepare interfaces for language, locale, date, number, currency, and text-direction differences.
---
# Localization-Aware UI
1. Use translation keys instead of embedding user-facing strings in logic.
2. Avoid concatenating fragments that translators cannot reorder naturally.
3. Format dates, numbers, currencies, and units for the selected locale.
4. Allow layouts to expand for longer translations and different scripts.
5. Support right-to-left direction where required, including icons and navigation order.
6. Use locale-aware sorting and plural rules.
7. Keep text out of images when possible.
8. Test pseudo-localized expansion, missing translations, mixed scripts, and date boundaries.
