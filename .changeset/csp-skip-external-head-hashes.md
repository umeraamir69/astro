---
'astro': patch
---

Fixes `security.csp` adding the hash of an empty string to `script-src` and `style-src` for external stylesheets and scripts. That extra hash could cause browsers to ignore `'unsafe-inline'`.
