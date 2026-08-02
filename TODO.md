# Mobile Responsive Fixes — Khabre India News

## Steps

- [x] 1. Analyze all HTML files (index, article, about, contact, privacy, terms, cookies, donotshare)
- [x] 2. index.html — Fix text overflow: headlines/summary/date-time kabhi na kate (remove line-clamp + ellipsis)
- [x] 3. index.html — Mobile card layout: title upar, time neeche (column layout)
- [x] 4. index.html — Follow icons (Insta, FB, X, YouTube): chhote + ek hi line/screen par
- [x] 5. index.html — Latest YouTube video: rectangular 16:9 box with big play button + YouTube badge
- [x] 6. index.html — 480px / 360px small-phone polish
- [x] 7. article.html — word-break safeguards (title, body, mini-brand, mini-cards)
- [x] 8. Static pages (about, contact, privacy, terms, cookies, donotshare) — mini-brand + h1 word-break fixes
- [x] 9. Final verification of edits

## Implementation Notes
- All text (headlines, summaries, timestamps) must remain fully visible — no clamping/ellipsis on phone.
- Mobile news cards: horizontal (image left, text right) with title on top and time below it.
- Follow icons: single centered row, smaller sizes (42px → 36px → 32px).
- YouTube box: 16:9 rectangular video thumbnail, big red circular play button, red "YouTube" badge, caption below.

## Detailed Edit Plan (approved)
### A) index.html
- Text overflow: `min-width:0` on `.card-body`/`.t-row`, `overflow:visible` + `overflow-wrap:anywhere` on h3/p/meta, overflow-safe `.mini-time`.
- Mobile card layout: keep horizontal card, `.t-row` column → title top, time below; add `min-width:0`.
- Follow icons: `.side-social` → `flex-wrap:nowrap` single centered row; sizes 42px → 36px (480px) → 32px (360px).
- YouTube box: fix HTML `vf-thumb`→`vf-media`, add red YouTube badge (with icon), keep big red circular play button, add dark gradient overlay, ensure 16:9 `aspect-ratio`.
- 480px/360px polish: tighter `.side-box`/`.video-fallback` padding, no overflow.

### B) article.html
- Add `word-break:break-word; overflow-wrap:anywhere;` to `.art-card h1`, `.art-content p`, `.art-meta`, `.mini-brand` (+`min-width:0`), `.mini-card .m-body h4`.

### C) Static pages (about, contact, privacy, terms, cookies, donotshare)
- Add same h1 + mini-brand word-break safeguards.

### D) Follow-up
- Update TODO.md checkboxes as steps complete, final verification read.

