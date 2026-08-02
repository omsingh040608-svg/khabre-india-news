# TODO — Khabre India News Mobile/UX Fixes

## Steps (Completed earlier)
- [x] 1. File analysis (index.html) completed
- [x] 2. Plan approved by user
- [x] 3. Resolve all merge-conflict markers (red lines) — keep mobile-polished HEAD version
- [x] 4. Remove "LIVE" badge & "अंतिम अपडेट: अभी-अभी" from header strip; keep date/time centred
- [x] 5. Homepage: small compact images on mobile (light thumbnails); big image inside article modal
- [x] 6. ट्रेंडिंग ख़बरें — only 5 news
- [x] 7. Footer: move "संपर्क करें" below "हमारे बारे में" accordion; remove old contact column
- [x] 8. About heading Hindi-only (remove "(About Khabre India)")
- [x] 9. Verify final result
- [x] 10. All changes verified (no conflict markers, trending=5, small thumbnails, big modal image, contact below about)
- [x] 11. "हमारी टीम" (हमारे बारे में accordion): Editor अनुपम परिहार card with photo (anupam-parihar.jpg) + bio + gold avatar fallback

## Latest — Article page replaces modal
- [x] 12. Homepage news cards now navigate to `article.html?id=N` (full-size image on a dedicated page) instead of opening a modal
- [x] 13. Trending links navigate to the article page too
- [x] 14. Modal overlay markup/styles/functions removed from index.html (no leftover `newsModal` / `closeNews` references)
- [x] 15. `news-data.js` (shared data) expanded with full multi-paragraph article bodies
- [x] 16. `article.html` reads `?id=` → hero image, category tag, title, relative/absolute timestamps, full body, WhatsApp/share links, and "और ख़बरें" related grid

## New Batch — Article page redesign + more news + bug fixes
- [x] 17. news-data.js: add 5 new articles (id 16–20) across खेल/तकनीक/दुनिया/राज्य/मनोरंजन + new IMG keys
- [x] 18. index.html: mirror new IMG keys + 5 new articles in its inline newsData (shared source stays in sync) — also fixed `1 render("all","");` JS syntax error
- [x] 19. article.html: add reading-progress bar (red top bar filling on scroll)
- [x] 20. article.html: fix share — native `navigator.share()` with WhatsApp/copy-link fallback; "अन्य ऐप्स" no longer just WhatsApp
- [x] 21. article.html: add estimated reading time ("X मिनट पढ़ें") in meta
- [x] 22. article.html: add category filter chips above "और ख़बरें" (same-category related news)
- [x] 23. article.html: typography polish (drop cap first paragraph, refined heading/spacing)
- [x] 24. article.html: add back-to-top floating button
- [x] 25. article.html: proper "खबर नहीं मिली" not-found state for invalid ?id= (no silent fallback)
- [x] 26. article.html: unify hero image sizing (single max-height constraint, no layout gap on mobile)
- [x] 27. index.html: verify/fix search ↔ category filter interaction (search resets category & vice-versa)
- [x] 28. Verify: homepage renders, article?id=1 works, all new articles (16–20) load, no console errors

