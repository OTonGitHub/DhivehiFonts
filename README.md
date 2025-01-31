CDN
---

Regions: Asia, Europe
Average Latency: 24ms

- url: `dhifonts.b-cdn.net`
- usage: `dhifonts.b-cdn.net/<font_family>/<font_name>`
- example: `dhifonts.b-cdn.net/mvtyper/mvtyper.ttf`

File Structure
```
dhifonts.b-cdn.net/
├── mvtyper/
│   ├── mvtyper-regular.ttf
│   ├── mvtyper-regular.woff2
│   ├── mvtyper-regular.woff
│   ├── mvtyper-bold.ttf
└── aammufk/
    ├── aammufk-regular.ttf
    ├── aammufk-bold.woff2
    ├── aammufk-italic.ttf
```

Fonts
-----
AammuFK (aka, MV Aammu Fala Kathi)
- Source: [MV Aammu FK](https://www.hassanhameed.com/thaana-fonts/mv-aammufk/)
- License: Open Font License (OFL)
- Family: **aammufk**
- MD5 checksum
  - aamufk.ttf: `172eade94a56987c5cd6f6520d95627d`

MV Typewriter
- Source
  - [Thaana Typewriter](https://www.hassanhameed.com/thaana-fonts/thaana-typewriter-font/)
  - [MV Typewriter Semibold](https://www.hassanhameed.com/thaana-fonts/mv-typewriter-semibold/)
- License: Open Font License (OFL)
- Family: **mvtyper**
- MD5 checksum
  - mvtyper.ttf: `f965994c23d3400970e5474dc7efcb50`
  - mvtyper-bold.ttf: `6772dfb2a11895d84884e68c44cef7f2`
  - mvtyper-semibold.ttf: `0af51bf037040b18d001ef65196599a9`

Code Example?
-------------
**HTML**
  ```
  @font-face {
    font-family: 'MV Typer';
    src: url('https://dhifonts.b-cdn.net/mvtyper/mvtyper.woff2') format('woff2'),
         url('https://dhifonts.b-cdn.net/mvtyper/mvtyper.woff') format('woff'),
         url('https://dhifonts.b-cdn.net/mvtyper/mvtyper.ttf') format('truetype');
    font-weight: normal;
    font-style: normal;
    font-display: swap;
  }
  ```

**HTML** - Blogger (`ttf` first & escape char)
```
@font-face {
    font-family: &#39;MV AammuFK&#39;;
    src: url(&#39;https://dhifonts.b-cdn.net/aammufk/aammufk.ttf&#39;) format(&#39;woff2&#39;),
         url(&#39;https://dhifonts.b-cdn.net/aammufk/aammufk.woff2&#39;) format(&#39;woff&#39;),
         url(&#39;https://dhifonts.b-cdn.net/aammufk/aammufk.woff&#39;) format(&#39;truetype&#39;);
    font-weight: normal;
    font-style: normal;
    font-display: swap;
}
```

FAQ
---
#### Add a Font?
Simply make a pull request or open an issue with the font you want to be added with a link to it. I primarily use another git hosting provider so I might miss a notification, so you can always shoot an email at cryonix@daraknet.cc as well. But try to stick to issues, they won't be missed, just takes time for me to see them.

#### Credits?
~~See commit message details of the font file, some of these fonts uses a copyleft license, they will be included here at a later date.~~

#### Other Types?
~~All the fonts included have already been tested for web or are widely in use, if enough fonts need support for other types such as `woff2` or `otf`, 
will change the folder structure and make it available easily. For now, no plans to do so, stick to `ttf`.~~

#### Versioning?
Only a handful of fonts actually have versioning or I have been ablt to track the version changes in an accurate manner. Hence, for now, will
just skip versioning and address each font by name and keep latest updated. It can be included in the future though. There is still a need for versioning
regardless of if author documents it or not, hence, I will include it in the future. And version changes can be seen in the commit appends.

#### Crawling?
I will setup a worker so that you can fetch versioning and font names, families etc via the URl recursively until last child is reached.

#### DDoS?
Feel free to try, at the end of the day, it come's down to the measures in place and my wallet, lul. Fail over CDN is one of the measures, but I won't
document it, it's highly unlikely for it to trigger. I will expand this to serve some of the common dhivehi friendly lotties as well.
