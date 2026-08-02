
# TODO — Khabre India News Mobile/UX Fixes

## Steps
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

