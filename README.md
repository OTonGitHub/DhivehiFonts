CDN
---

Regions: Asia, Europe
Average Latency: 24ms

- url: `dhifonts.b-cdn.net`
- usage: `dhifonts.b-cdn.net/<font_name>`
- example: `dhifonts.b-cdn.net/mvtyper.ttf`

#### Code Example?
- HTML
  ```
  @font-face {
      font-family: 'MV Tpyer';
      src: url('https://dhifonts.b-cdn.net/mvtyper.ttf') format('truetype');
      font-weight: normal;
      font-style: normal;
  }
  ```

- React
  ```
  <div style={{ fontFamily: "'MVT Pyer', sans-serif" }}>
      <h1>... </h1>
  </div>
  ```

#### FAQ
Credits?
- See commit message details of the font file, some of these fonts uses a copyleft license, they will be included here at a later date.

Other Types?
- All the fonts included have already been tested for web or are widely in use, if enough fonts need support for other types such as `woff2` or `otf`, 
will change the folder structure and make it available easily. For now, no plans to do so, stick to `ttf`.
