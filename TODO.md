 # Task Progress

## 1) Header (index.html)
- [x] Remove Hindi "ख़बरें इंडिया न्यूज़" brand + "आवाज़ जन गण मन की" tagline, keep English "Khabre India News"
- [x] Make social icons smaller, place in corner just above blue nav line
- [x] Update top-bar Hindi brand on sub-pages (about/contact/privacy/terms/cookies/donotshare/article) to English

## 2) Date & Time
- [x] Remove blue background from `.search-time` box

## 3) News category tag
- [x] Remove the top-left category tag (भारत/तकनीक/मनोरंजन) on news cards

## 4) All playlists to have 4 news
- [x] Add news to राजनीति (1→4), खेल (3→4), मनोरंजन (3→4), राज्य (3→4), दुनिया (3→4)
- [x] Update both index.html and news-data.js

## 5) भारत playlist
- [x



























## 6) Mobile spacing
- [x] Add more left/right padding on phone so items don't stick to edges

## 7) contact.html
- [x] Remove WhatsApp number 83188 80819 line

## 8) Footer WhatsApp icons
- [x] Remove the 2 WhatsApp icons from footer

## 9) Add 4 news to EVERY playlist (sabhi categories)
- [x] राजनीति: 1 → 4 news (3 news added)
- [x] खेल: 3 → 4 news (1 news added)
- [x] मनोरंजन: 3 → 4 news (1 news added)
- [x] राज्य: 3 → 4 news (1 news added)
- [x] दुनिया: 3 → 4 news (1 news added)
- [x] भारत (5), बिजनेस (4), तकनीक (4) — already have 4+
- [x] Update news-data.js
- [x] Update index.html
- [x] Add 7 new news items (id 27-33) to both index.html and news-data.js
- [x] Add matching image presets (flag, badminton, concert, metro2, diplomacy) to IMG in both files

## 10) News layout — remove slider
- [x] Remove horizontal slider bar in news rows (`.card-row`), stack cards one below another (ek ke neeche ek) on all screens

## 11) Auto-translate disable
- [x] Add `<meta name="google" content="notranslate">` + `translate="no"` on `<html>` in all 9 HTML pages (index, article, about, privacy, terms, cookies, donotshare, contact)

## 12) Footer email buttons
- [x] Remove both email (em) buttons from footer — removed the two email entries from `SOCIALS` array in index.html


- [x] Create `category.html` — shows ALL news of a selected category, with category chips + hero + article links
- [x] Home (index.html) `render()` now shows only 2 news per category section
- [x] Category title on home is now clickable → opens `category.html?cat=...`
- [x] Added "और देखें (N)" button under each category section → opens `category.html?cat=...`
- [x] category.html loads `news-data.js` (shared data) so it always matches home data
