# zcorpan's GitHub activity

Summary of Simon Pieters's ([@zcorpan](https://github.com/zcorpan)) work for Mozilla on GitHub, by year. Personal projects are omitted.

## 2026 (through September)

### Sanitizer API and streaming HTML parsing

- Upstreaming the Sanitizer API into HTML:
  - WIP PR [whatwg/html#12314](https://github.com/whatwg/html/pull/12314)
  - Reviewed Noam's [whatwg/html#12395](https://github.com/whatwg/html/pull/12395)
  - [Moved open issues](https://github.com/WICG/sanitizer-api/issues/399) to whatwg/html
  - [Acknowledgments](https://github.com/whatwg/html/pull/12522)
- Inert fragment for sanitizing: [whatwg/html#12560](https://github.com/whatwg/html/issues/12560), [whatwg/html#12561](https://github.com/whatwg/html/pull/12561)
- Trusted Types integration:
  - [w3c/trusted-types#616](https://github.com/w3c/trusted-types/pull/616), tests in [wpt#63042](https://github.com/web-platform-tests/wpt/pull/63042)
  - Reviewed [w3c/trusted-types#606](https://github.com/w3c/trusted-types/pull/606) and [whatwg/html#12583](https://github.com/whatwg/html/pull/12583)
- Reviewed streaming, positional parsing, and sanitize-while-parsing:
  - [whatwg/html#12758](https://github.com/whatwg/html/pull/12758), [#12753](https://github.com/whatwg/html/pull/12753), [#12756](https://github.com/whatwg/html/pull/12756), [#12848](https://github.com/whatwg/html/pull/12848)
  - Related wpt PRs, e.g. [wpt#62492](https://github.com/web-platform-tests/wpt/pull/62492), [wpt#61748](https://github.com/web-platform-tests/wpt/pull/61748); fixed [wpt#62084](https://github.com/web-platform-tests/wpt/pull/62084)
  - Standards positions: [#1443](https://github.com/mozilla/standards-positions/issues/1443), [#1370](https://github.com/mozilla/standards-positions/issues/1370)
- Parser:
  - html5lib-tests import in [wpt#60787](https://github.com/web-platform-tests/wpt/pull/60787) and `.dat` format docs in [wpt#60827](https://github.com/web-platform-tests/wpt/pull/60827)
  - Reviewed the adoption agency clarification [whatwg/html#12599](https://github.com/whatwg/html/pull/12599)

### Media elements

- Lazy-loading `<video>`/`<audio>`:
  - Reviewed Scott Jehl's [whatwg/html#11980](https://github.com/whatwg/html/pull/11980) and his tests
  - Follow-up fixes: [whatwg/html#12970](https://github.com/whatwg/html/pull/12970), [#12972](https://github.com/whatwg/html/pull/12972)
  - Issues: [#12854](https://github.com/whatwg/html/issues/12854), [#12971](https://github.com/whatwg/html/issues/12971), [#12973](https://github.com/whatwg/html/issues/12973), [#12974](https://github.com/whatwg/html/issues/12974), [#12975](https://github.com/whatwg/html/issues/12975)
  - Tests: [wpt#62828](https://github.com/web-platform-tests/wpt/pull/62828), [#62832](https://github.com/web-platform-tests/wpt/pull/62832), [#62835](https://github.com/web-platform-tests/wpt/pull/62835), [#62859](https://github.com/web-platform-tests/wpt/pull/62859)
- Resource selection and `<source>` moves:
  - [whatwg/html#12511](https://github.com/whatwg/html/pull/12511), [wpt#60466](https://github.com/web-platform-tests/wpt/pull/60466), [wpt#62180](https://github.com/web-platform-tests/wpt/pull/62180)
  - Issues: [#12835](https://github.com/whatwg/html/issues/12835), [#12836](https://github.com/whatwg/html/issues/12836), [#12986](https://github.com/whatwg/html/issues/12986)
  - Reviewed [whatwg/html#12880](https://github.com/whatwg/html/pull/12880)
- ORB metadata on media and script requests: [whatwg/html#12914](https://github.com/whatwg/html/pull/12914)

### Navigation and history

- Rate limiting for navigation, traversal, and `pushState()`: [whatwg/html#12492](https://github.com/whatwg/html/pull/12492), [wpt#60210](https://github.com/web-platform-tests/wpt/pull/60210), [mdn/content#44477](https://github.com/mdn/content/issues/44477)
- `javascript:` URL `targetSnapshotParams`: [whatwg/html#12303](https://github.com/whatwg/html/pull/12303), [#12572](https://github.com/whatwg/html/pull/12572)
- `ancestorOrigins`: [whatwg/html#12071](https://github.com/whatwg/html/pull/12071)
- Meta refresh fragment navigations: [whatwg/html#12325](https://github.com/whatwg/html/issues/12325)
- Navigation API:
  - Tests: [wpt#59845](https://github.com/web-platform-tests/wpt/pull/59845), [wpt#62425](https://github.com/web-platform-tests/wpt/pull/62425)
  - Reviewed PRs from Mozilla's farre/theIDinside (e.g. [whatwg/html#12256](https://github.com/whatwg/html/pull/12256)) and Shannon Booth ([#12929](https://github.com/whatwg/html/pull/12929), [#12933](https://github.com/whatwg/html/pull/12933))

### Fullscreen keyboard lock

- Standards position: [mozilla/standards-positions#1385](https://github.com/mozilla/standards-positions/issues/1385)
- Reviewed [whatwg/fullscreen#232](https://github.com/whatwg/fullscreen/pull/232)
- Tests: [wpt#59451](https://github.com/web-platform-tests/wpt/pull/59451), [wpt#59726](https://github.com/web-platform-tests/wpt/pull/59726)
- Related: [w3c/pointerlock#110](https://github.com/w3c/pointerlock/issues/110), [polyfill](https://github.com/zcorpan/navigator-keyboard-lock-polyfill/pull/1)
- BCD for Firefox 152 `unadjustedMovement`: [mdn/browser-compat-data#29707](https://github.com/mdn/browser-compat-data/pull/29707)

### Other HTML fixes and reviews

- Focus events at a `Window`: [whatwg/html#12875](https://github.com/whatwg/html/pull/12875), [wpt#62344](https://github.com/web-platform-tests/wpt/pull/62344)
- CORS check in the `<link>` stylesheet MIME type quirk: [whatwg/html#12468](https://github.com/whatwg/html/pull/12468), [wpt#62516](https://github.com/web-platform-tests/wpt/pull/62516), [w3c/csswg-drafts#14480](https://github.com/w3c/csswg-drafts/issues/14480)
- Body margin attributes: [wpt#58682](https://github.com/web-platform-tests/wpt/pull/58682), [mdn/content#43534](https://github.com/mdn/content/pull/43534)
- Style load event: [wpt#57346](https://github.com/web-platform-tests/wpt/pull/57346)
- Picture-in-Picture `resize` event: [w3c/picture-in-picture#243](https://github.com/w3c/picture-in-picture/pull/243)
- WebVTT cue settings syntax: [w3c/webvtt#542](https://github.com/w3c/webvtt/pull/542)
- Issues: [whatwg/html#12101](https://github.com/whatwg/html/issues/12101), [#12178](https://github.com/whatwg/html/issues/12178), [#12571](https://github.com/whatwg/html/issues/12571), [#12847](https://github.com/whatwg/html/issues/12847), [#12982](https://github.com/whatwg/html/issues/12982)
- Many reviews, notably Anne's PRs, Joey Arhar's customizable `<select>` work, and the XSLT deprecation ([whatwg/html#12805](https://github.com/whatwg/html/pull/12805), [whatwg/dom#1499](https://github.com/whatwg/dom/pull/1499))
- XSLT polyfill fixes: [mfreed7/xslt_polyfill#37](https://github.com/mfreed7/xslt_polyfill/pull/37), [mfreed7/xslt_extension#6](https://github.com/mfreed7/xslt_extension/pull/6)

### Spec infrastructure

- On-demand MDN annotation panels:
  - [whatwg/wattsi#169](https://github.com/whatwg/wattsi/issues/169), [#170](https://github.com/whatwg/wattsi/pull/170), [#171](https://github.com/whatwg/wattsi/pull/171)
  - [whatwg/html-build#319](https://github.com/whatwg/html-build/pull/319), [whatwg/whatwg.org#506](https://github.com/whatwg/whatwg.org/pull/506), [whatwg/html#12864](https://github.com/whatwg/html/pull/12864)
  - [speced/bikeshed#3319](https://github.com/speced/bikeshed/issues/3319), [speced/mdn-spec-links#853](https://github.com/speced/mdn-spec-links/issues/853)
- Rendering and performance: [whatwg/html#12867](https://github.com/whatwg/html/pull/12867), [whatwg/wattsi#172](https://github.com/whatwg/wattsi/pull/172), [whatwg/html#12924](https://github.com/whatwg/html/pull/12924), [whatwg/whatwg.org#508](https://github.com/whatwg/whatwg.org/pull/508)
- specfmt fixes: [#31](https://github.com/domfarolino/specfmt/pull/31), [#33](https://github.com/domfarolino/specfmt/pull/33), [#34](https://github.com/domfarolino/specfmt/pull/34)
- Diff UI: [w3c/htmldiff-ui#26](https://github.com/w3c/htmldiff-ui/pull/26), [w3c/htmldiff-nav#3](https://github.com/w3c/htmldiff-nav/pull/3)
- Editor tooling: [whatwg-editor-dashboard](https://github.com/zcorpan/whatwg-editor-dashboard/pull/2), [whatwg-contrib-report](https://github.com/zcorpan/whatwg-contrib-report)

### Mozilla standards positions and explainers

- Filed [#1336](https://github.com/mozilla/standards-positions/issues/1336), [#1337](https://github.com/mozilla/standards-positions/issues/1337), [#1382](https://github.com/mozilla/standards-positions/issues/1382) (idscope, with [WICG/idrefs#4](https://github.com/WICG/idrefs/pull/4))
- Commented on about 50 position threads
- Reviewed position PRs such as [#1411](https://github.com/mozilla/standards-positions/pull/1411) and [#1431](https://github.com/mozilla/standards-positions/pull/1431)
- Drafted the eyedropper-input spec: [mozilla/explainers#67](https://github.com/mozilla/explainers/pull/67)

### Interop, MDN, and governance

- Ran the interop-accessibility meetings (e.g. [#246](https://github.com/web-platform-tests/interop-accessibility/issues/246))
- Proposed AVIF for Interop: [web-platform-tests/interop#1461](https://github.com/web-platform-tests/interop/issues/1461), [wpt#62892](https://github.com/web-platform-tests/wpt/issues/62892)
- MDN gaps: [mdn/content#42970](https://github.com/mdn/content/issues/42970), [#43730](https://github.com/mdn/content/issues/43730), [w3c/editing#530](https://github.com/w3c/editing/issues/530)
- Reviewed the h1 UA styles posts: [mdn/blog#385](https://github.com/mdn/blog/pull/385)
- AI contribution policy: [whatwg/sg#262](https://github.com/whatwg/sg/issues/262), [whatwg/meta#418](https://github.com/whatwg/meta/issues/418), reviewed [whatwg/sg#285](https://github.com/whatwg/sg/pull/285)
- AI spec-research tooling: [jnjaeschke/webspec-index#27](https://github.com/jnjaeschke/webspec-index/pull/27), [noamr/web-archeologist#4](https://github.com/noamr/web-archeologist/pull/4)

## 2025

### HTML editing

- Became the primary editor of the HTML Standard: [whatwg/sg#257](https://github.com/whatwg/sg/pull/257)
- Source reformatting proposal: [whatwg/html#11640](https://github.com/whatwg/html/pull/11640)
- Process: [whatwg/meta#345](https://github.com/whatwg/meta/issues/345) (incubating specs in WHATWG), [whatwg/meta#367](https://github.com/whatwg/meta/pull/367)
- Quirks Standard maintenance: [whatwg/quirks#79](https://github.com/whatwg/quirks/pull/79), [#80](https://github.com/whatwg/quirks/pull/80), [#81](https://github.com/whatwg/quirks/pull/81), [#90](https://github.com/whatwg/quirks/pull/90)
  - Percentage height quirk for `position: sticky`: [whatwg/quirks#88](https://github.com/whatwg/quirks/pull/88), [wpt#54266](https://github.com/web-platform-tests/wpt/pull/54266)

### Removing `<h1>` UA styles in sectioning elements

- Spec and tests: [whatwg/html#11102](https://github.com/whatwg/html/pull/11102), [wpt#51673](https://github.com/web-platform-tests/wpt/pull/51673)
- Shipped in Firefox 140: [mdn/browser-compat-data#26946](https://github.com/mdn/browser-compat-data/pull/26946), [#26881](https://github.com/mdn/browser-compat-data/issues/26881)
- MDN:
  - Blog post updates: [mdn/blog#388](https://github.com/mdn/blog/pull/388), [#389](https://github.com/mdn/blog/pull/389), [#391](https://github.com/mdn/blog/pull/391), [#402](https://github.com/mdn/blog/pull/402)
  - Docs: [mdn/content#37827](https://github.com/mdn/content/pull/37827), [#39582](https://github.com/mdn/content/pull/39582)
- CSS resets: [filipelinhares/ress#31](https://github.com/filipelinhares/ress/pull/31), [mayank99/reset.css#20](https://github.com/mayank99/reset.css/pull/20), [vladocar/CSS-Micro-Reset#7](https://github.com/vladocar/CSS-Micro-Reset/pull/7)

### Headings

- `:heading` and `:heading()`:
  - [whatwg/html#11413](https://github.com/whatwg/html/pull/11413), [#11412](https://github.com/whatwg/html/issues/11412), [wpt#53440](https://github.com/web-platform-tests/wpt/pull/53440), [mdn/mdn#708](https://github.com/mdn/mdn/issues/708)
  - Reviewed [w3c/csswg-drafts#11836](https://github.com/w3c/csswg-drafts/pull/11836), [#12404](https://github.com/w3c/csswg-drafts/pull/12404), [#12634](https://github.com/w3c/csswg-drafts/pull/12634), [whatwg/html#11589](https://github.com/whatwg/html/pull/11589)
- `headingoffset`/`headingreset`:
  - Reviewed [whatwg/html#11086](https://github.com/whatwg/html/pull/11086) and [wpt#54294](https://github.com/web-platform-tests/wpt/pull/54294)
  - Conformance: [whatwg/html#11979](https://github.com/whatwg/html/pull/11979) ([#11977](https://github.com/whatwg/html/issues/11977))
  - Standards position: [mozilla/standards-positions#1263](https://github.com/mozilla/standards-positions/issues/1263)

### Navigation and history

- `SecurityError` for `pushState()`/`replaceState()` abuse: [whatwg/html#11169](https://github.com/whatwg/html/pull/11169), [wpt#51670](https://github.com/web-platform-tests/wpt/pull/51670), [mdn/content#38833](https://github.com/mdn/content/pull/38833)
  - Follow-ups: [whatwg/html#11410](https://github.com/whatwg/html/issues/11410), [#11844](https://github.com/whatwg/html/issues/11844) (led to the 2026 rate limiter)
- `javascript:` URLs: [whatwg/html#10957](https://github.com/whatwg/html/pull/10957), [wpt#50193](https://github.com/web-platform-tests/wpt/pull/50193); reviewed [whatwg/html#11700](https://github.com/whatwg/html/pull/11700)
- No browsing context:
  - `window.open()`: [whatwg/html#11798](https://github.com/whatwg/html/pull/11798), [wpt#55475](https://github.com/web-platform-tests/wpt/pull/55475)
  - Event handlers: [whatwg/html#12014](https://github.com/whatwg/html/issues/12014), [wpt#56715](https://github.com/web-platform-tests/wpt/pull/56715)
- Navigation API:
  - [whatwg/html#12031](https://github.com/whatwg/html/pull/12031)
  - Reviewed Noam's PRs, e.g. [#11692](https://github.com/whatwg/html/pull/11692), [#11725](https://github.com/whatwg/html/pull/11725), [#11817](https://github.com/whatwg/html/pull/11817), [#11843](https://github.com/whatwg/html/pull/11843), [#11984](https://github.com/whatwg/html/pull/11984)
  - Reviewed farre's [#11952](https://github.com/whatwg/html/pull/11952) and Domenic's [#11409](https://github.com/whatwg/html/pull/11409)
- Speculation rules: reviewed [whatwg/html#11426](https://github.com/whatwg/html/pull/11426); [WICG/nav-speculation#368](https://github.com/WICG/nav-speculation/issues/368)
- `ancestorOrigins` redaction using iframe `referrerpolicy`:
  - [whatwg/html#11560](https://github.com/whatwg/html/pull/11560), [mdn/content#42231](https://github.com/mdn/content/issues/42231)
  - Tests: [wpt#56616](https://github.com/web-platform-tests/wpt/pull/56616), [#56635](https://github.com/web-platform-tests/wpt/pull/56635); reviewed [#56224](https://github.com/web-platform-tests/wpt/pull/56224)

### Rendering and quirks

- Bare `<li>` `list-style-position` quirk: [whatwg/html#10959](https://github.com/whatwg/html/pull/10959), [wpt#50348](https://github.com/web-platform-tests/wpt/pull/50348)
- `frameborder` on `<iframe>`: [whatwg/html#11103](https://github.com/whatwg/html/pull/11103), [#11098](https://github.com/whatwg/html/issues/11098), [wpt#51132](https://github.com/web-platform-tests/wpt/pull/51132)
- Removed the `rowspan=0` quirk: [whatwg/html#11551](https://github.com/whatwg/html/pull/11551), [wpt#54265](https://github.com/web-platform-tests/wpt/pull/54265)
- `topmargin`/`leftmargin` apply to both sides: [whatwg/html#11881](https://github.com/whatwg/html/pull/11881), [#11879](https://github.com/whatwg/html/issues/11879); snapshotting margin attributes on frames: [#11887](https://github.com/whatwg/html/pull/11887)
- `contenteditable=plaintext-only` UA style: [whatwg/html#11351](https://github.com/whatwg/html/pull/11351), [#11350](https://github.com/whatwg/html/issues/11350), [wpt#52930](https://github.com/web-platform-tests/wpt/pull/52930)
- Doctypes that enable XHTML entities: [whatwg/html#11823](https://github.com/whatwg/html/pull/11823), [wpt#55614](https://github.com/web-platform-tests/wpt/pull/55614)
- Customizable `<select>`:
  - Issues: [whatwg/html#11017](https://github.com/whatwg/html/issues/11017), [#11804](https://github.com/whatwg/html/issues/11804)
  - Reviewed Joey Arhar's [#11720](https://github.com/whatwg/html/pull/11720), [#11738](https://github.com/whatwg/html/pull/11738), [#11758](https://github.com/whatwg/html/pull/11758), [#11764](https://github.com/whatwg/html/pull/11764), [#11805](https://github.com/whatwg/html/pull/11805)
  - Tests: [wpt#56009](https://github.com/web-platform-tests/wpt/pull/56009)
- Buttons and dialogs: [whatwg/html#11043](https://github.com/whatwg/html/issues/11043); reviewed Luke Warlow's [#11049](https://github.com/whatwg/html/pull/11049), [#11053](https://github.com/whatwg/html/pull/11053) and Keith Cirkel's `closedby` PRs [#11015](https://github.com/whatwg/html/pull/11015), [#11326](https://github.com/whatwg/html/pull/11326)

### Other HTML and web platform work

- `<a ping>`: made UI optional in [whatwg/html#11329](https://github.com/whatwg/html/pull/11329) ([#11309](https://github.com/whatwg/html/issues/11309)); positive position in [mozilla/standards-positions#1235](https://github.com/mozilla/standards-positions/pull/1235)
- Images:
  - [whatwg/html#11266](https://github.com/whatwg/html/pull/11266), [#11815](https://github.com/whatwg/html/pull/11815), [#11777](https://github.com/whatwg/html/issues/11777)
  - Reviewed optional `<img src>` with `srcset` ([whatwg/html#11300](https://github.com/whatwg/html/pull/11300)), with [validator/validator#1821](https://github.com/validator/validator/issues/1821) and [mdn/content#39489](https://github.com/mdn/content/issues/39489)
- Parser and serialization:
  - Escaping `<` and `>` in attribute values: [wpt#51827](https://github.com/web-platform-tests/wpt/pull/51827), [mozilla/standards-positions#1209](https://github.com/mozilla/standards-positions/issues/1209)
  - mXSS: [whatwg/html#11397](https://github.com/whatwg/html/issues/11397); parser pop callback: [#11781](https://github.com/whatwg/html/issues/11781)
- Removals:
  - `X-UA-Compatible`: [whatwg/html#11356](https://github.com/whatwg/html/issues/11356)
  - SVG `<discard>`: [w3c/svgwg#973](https://github.com/w3c/svgwg/pull/973), [wpt#51800](https://github.com/web-platform-tests/wpt/pull/51800)
  - XSLT: [mozilla/standards-positions#1287](https://github.com/mozilla/standards-positions/issues/1287), [mdn/content#42190](https://github.com/mdn/content/issues/42190), polyfill fix [mfreed7/xslt_polyfill#1](https://github.com/mfreed7/xslt_polyfill/pull/1)
- Text tracks and WebVTT:
  - [whatwg/html#11665](https://github.com/whatwg/html/issues/11665); became a WebVTT wpt reviewer ([wpt#54380](https://github.com/web-platform-tests/wpt/pull/54380))
  - Reviewed [w3c/webvtt#534](https://github.com/w3c/webvtt/pull/534) and [wpt#54338](https://github.com/web-platform-tests/wpt/pull/54338)
- Incubations:
  - Declarative partial updates: [WICG/declarative-partial-updates#7](https://github.com/WICG/declarative-partial-updates/issues/7), [#38](https://github.com/WICG/declarative-partial-updates/issues/38), [#42](https://github.com/WICG/declarative-partial-updates/issues/42)
  - Upstreaming Capability Delegation: [WICG/capability-delegation#40](https://github.com/WICG/capability-delegation/issues/40)

### Mozilla standards positions

- Dashboard and tooling:
  - PRs: [#1178](https://github.com/mozilla/standards-positions/pull/1178), [#1180](https://github.com/mozilla/standards-positions/pull/1180), [#1185](https://github.com/mozilla/standards-positions/pull/1185), [#1210](https://github.com/mozilla/standards-positions/pull/1210), [#1216](https://github.com/mozilla/standards-positions/pull/1216), [#1314](https://github.com/mozilla/standards-positions/pull/1314), [#1328](https://github.com/mozilla/standards-positions/pull/1328)
  - Issues: [#1163](https://github.com/mozilla/standards-positions/issues/1163), [#1166](https://github.com/mozilla/standards-positions/issues/1166)
- Filed [#1230](https://github.com/mozilla/standards-positions/issues/1230), [#1329](https://github.com/mozilla/standards-positions/issues/1329)
- Commented on about 65 position threads
- Reviewed position PRs such as [#1162](https://github.com/mozilla/standards-positions/pull/1162), [#1190](https://github.com/mozilla/standards-positions/pull/1190), [#1297](https://github.com/mozilla/standards-positions/pull/1297), [#1308](https://github.com/mozilla/standards-positions/pull/1308)

### Interop and wpt

- Ran the interop-accessibility meetings (e.g. [#166](https://github.com/web-platform-tests/interop-accessibility/issues/166), [#213](https://github.com/web-platform-tests/interop-accessibility/issues/213)); Interop 2026 accessibility investigation: [#202](https://github.com/web-platform-tests/interop-accessibility/issues/202), [web-platform-tests/interop#1141](https://github.com/web-platform-tests/interop/issues/1141)
- Interop 2025 test maintenance:
  - Web compat `appearance` tests: [web-platform-tests/interop#927](https://github.com/web-platform-tests/interop/issues/927), [wpt#50704](https://github.com/web-platform-tests/wpt/pull/50704), [wpt-metadata#7297](https://github.com/web-platform-tests/wpt-metadata/pull/7297)
  - WebRTC SFrameTransform: [web-platform-tests/interop#964](https://github.com/web-platform-tests/interop/issues/964), [wpt#50651](https://github.com/web-platform-tests/wpt/pull/50651), [wpt-metadata#7611](https://github.com/web-platform-tests/wpt-metadata/pull/7611)
  - `scrollIntoView()`: [wpt-metadata#7424](https://github.com/web-platform-tests/wpt-metadata/pull/7424), [w3c/csswg-drafts#12260](https://github.com/w3c/csswg-drafts/issues/12260), reviewed [wpt#51241](https://github.com/web-platform-tests/wpt/pull/51241)
- Carry-over proposals: [web-platform-tests/interop-privacy#19](https://github.com/web-platform-tests/interop-privacy/issues/19)
- Docs fixes: [web-platform-tests/interop#1023](https://github.com/web-platform-tests/interop/pull/1023), [#1170](https://github.com/web-platform-tests/interop/pull/1170), [web-platform-tests/rfcs#223](https://github.com/web-platform-tests/rfcs/pull/223)

### Spec tooling

- Diff readability: [w3c/htmldiff-ui#23](https://github.com/w3c/htmldiff-ui/issues/23), [#24](https://github.com/w3c/htmldiff-ui/issues/24), [w3c/htmldiff-nav#2](https://github.com/w3c/htmldiff-nav/issues/2) (fixed in 2026)
- PR Preview: [specinfra/pr-preview#171](https://github.com/specinfra/pr-preview/issues/171), [#173](https://github.com/specinfra/pr-preview/issues/173)
- UI Events build: [w3c/uievents#408](https://github.com/w3c/uievents/pull/408), [#410](https://github.com/w3c/uievents/pull/410), [#407](https://github.com/w3c/uievents/issues/407), [#409](https://github.com/w3c/uievents/issues/409)
- Reviewed building HTML with Bikeshed: [whatwg/html-build#296](https://github.com/whatwg/html-build/pull/296)

## Caveats

- "Reviewed" includes a few older PRs that were only updated in that year.
- Commit search only covers default branches, so commits pushed to other people's PR branches are missing.
- Bugzilla and Phabricator aren't included.
