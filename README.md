# ख़बरें इंडिया न्यूज़ — Khabre India News

एक static HTML news website — कोई build step, कोई server, कोई dependency नहीं।

## चलाने के तरीक़े

### 1) सीधे browser में
`index.html` पर double-click करें — तुरंत खुल जाएगी।

### 2) GitHub Pages पर publish करना
1. इस folder को GitHub पर एक नई repository में upload करें।
2. **Settings → Pages** पर जाएँ।
3. **Source** में `Deploy from a branch` चुनें और **Branch** में `main` + `/ (root)` select करें → **Save**।
4. एक-दो मिनट बाद आपकी site live होगी: `https://<your-username>.github.io/<repo-name>/`

## Files
- `index.html` — पूरी website (news data, styles, live clock, सब कुछ इसी में है)
- `logo.png` — brand logo

## News कैसे update करें
`index.html` में `newsData` array (लगभग line 550 के आस-पास) खोलें और अपनी खबर जोड़ें/बदलें:

```js
{
  id: 16,
  offset: 5,                      // कितने मिनट पहले (live "X मिनट पहले" के लिए)
  category: "भारत",                // भारत / दुनिया / राजनीति / राज्य / खेल / मनोरंजन / बिजनेस / तकनीक
  title: "यहाँ हेडलाइन लिखें",
  summary: "2-3 लाइन का सारांश",
  body: "पूरी खबर का विवरण",
  img: "https://your-image-url.jpg" // या IMG.parliament जैसा preset
}
```

## Features
- 🕒 Real-time घड़ी (हर सेकंड update)
- 📅 पूरी हिन्दी तारीख़ + दिन
- 🖼️ हर खबर के साथ topical image
- ⏱️ "X मिनट पहले" timestamps हर 15 सेकंड में refresh
- 🔄 News order हर 60 सेकंड में rotate — page हमेशा live लगता है
- 📱 पूरी तरह mobile responsive
- 🔗 Social links (WhatsApp / Instagram / YouTube / Facebook / X / Email) native app deep-link के साथ
