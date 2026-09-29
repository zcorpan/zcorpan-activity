# zcorpan's GitHub activity in 2026

Summary of Simon Pieters's ([@zcorpan](https://github.com/zcorpan)) work for Mozilla on GitHub in 2026 (through September). Personal projects are omitted.

## Sanitizer API and streaming HTML parsing

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

## Media elements

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

## Navigation and history

- Rate limiting for navigation, traversal, and `pushState()`: [whatwg/html#12492](https://github.com/whatwg/html/pull/12492), [wpt#60210](https://github.com/web-platform-tests/wpt/pull/60210), [mdn/content#44477](https://github.com/mdn/content/issues/44477)
- `javascript:` URL `targetSnapshotParams`: [whatwg/html#12303](https://github.com/whatwg/html/pull/12303), [#12572](https://github.com/whatwg/html/pull/12572)
- `ancestorOrigins`: [whatwg/html#12071](https://github.com/whatwg/html/pull/12071)
- Meta refresh fragment navigations: [whatwg/html#12325](https://github.com/whatwg/html/issues/12325)
- Navigation API:
  - Tests: [wpt#59845](https://github.com/web-platform-tests/wpt/pull/59845), [wpt#62425](https://github.com/web-platform-tests/wpt/pull/62425)
  - Reviewed PRs from Mozilla's farre/theIDinside (e.g. [whatwg/html#12256](https://github.com/whatwg/html/pull/12256)) and Shannon Booth ([#12929](https://github.com/whatwg/html/pull/12929), [#12933](https://github.com/whatwg/html/pull/12933))

## Fullscreen keyboard lock

- Standards position: [mozilla/standards-positions#1385](https://github.com/mozilla/standards-positions/issues/1385)
- Reviewed [whatwg/fullscreen#232](https://github.com/whatwg/fullscreen/pull/232)
- Tests: [wpt#59451](https://github.com/web-platform-tests/wpt/pull/59451), [wpt#59726](https://github.com/web-platform-tests/wpt/pull/59726)
- Related: [w3c/pointerlock#110](https://github.com/w3c/pointerlock/issues/110), [polyfill](https://github.com/zcorpan/navigator-keyboard-lock-polyfill/pull/1)
- BCD for Firefox 152 `unadjustedMovement`: [mdn/browser-compat-data#29707](https://github.com/mdn/browser-compat-data/pull/29707)

## Other HTML fixes and reviews

- Focus events at a `Window`: [whatwg/html#12875](https://github.com/whatwg/html/pull/12875), [wpt#62344](https://github.com/web-platform-tests/wpt/pull/62344)
- CORS check in the `<link>` stylesheet MIME type quirk: [whatwg/html#12468](https://github.com/whatwg/html/pull/12468), [wpt#62516](https://github.com/web-platform-tests/wpt/pull/62516), [w3c/csswg-drafts#14480](https://github.com/w3c/csswg-drafts/issues/14480)
- Body margin attributes: [wpt#58682](https://github.com/web-platform-tests/wpt/pull/58682), [mdn/content#43534](https://github.com/mdn/content/pull/43534)
- Style load event: [wpt#57346](https://github.com/web-platform-tests/wpt/pull/57346)
- Picture-in-Picture `resize` event: [w3c/picture-in-picture#243](https://github.com/w3c/picture-in-picture/pull/243)
- WebVTT cue settings syntax: [w3c/webvtt#542](https://github.com/w3c/webvtt/pull/542)
- Issues: [whatwg/html#12101](https://github.com/whatwg/html/issues/12101), [#12178](https://github.com/whatwg/html/issues/12178), [#12571](https://github.com/whatwg/html/issues/12571), [#12847](https://github.com/whatwg/html/issues/12847), [#12982](https://github.com/whatwg/html/issues/12982)
- Many reviews, notably Anne's PRs, Joey Arhar's customizable `<select>` work, and the XSLT deprecation ([whatwg/html#12805](https://github.com/whatwg/html/pull/12805), [whatwg/dom#1499](https://github.com/whatwg/dom/pull/1499))
- XSLT polyfill fixes: [mfreed7/xslt_polyfill#37](https://github.com/mfreed7/xslt_polyfill/pull/37), [mfreed7/xslt_extension#6](https://github.com/mfreed7/xslt_extension/pull/6)

## Spec infrastructure

- On-demand MDN annotation panels:
  - [whatwg/wattsi#169](https://github.com/whatwg/wattsi/issues/169), [#170](https://github.com/whatwg/wattsi/pull/170), [#171](https://github.com/whatwg/wattsi/pull/171)
  - [whatwg/html-build#319](https://github.com/whatwg/html-build/pull/319), [whatwg/whatwg.org#506](https://github.com/whatwg/whatwg.org/pull/506), [whatwg/html#12864](https://github.com/whatwg/html/pull/12864)
  - [speced/bikeshed#3319](https://github.com/speced/bikeshed/issues/3319), [speced/mdn-spec-links#853](https://github.com/speced/mdn-spec-links/issues/853)
- Rendering and performance: [whatwg/html#12867](https://github.com/whatwg/html/pull/12867), [whatwg/wattsi#172](https://github.com/whatwg/wattsi/pull/172), [whatwg/html#12924](https://github.com/whatwg/html/pull/12924), [whatwg/whatwg.org#508](https://github.com/whatwg/whatwg.org/pull/508)
- specfmt fixes: [#31](https://github.com/domfarolino/specfmt/pull/31), [#33](https://github.com/domfarolino/specfmt/pull/33), [#34](https://github.com/domfarolino/specfmt/pull/34)
- Diff UI: [w3c/htmldiff-ui#26](https://github.com/w3c/htmldiff-ui/pull/26), [w3c/htmldiff-nav#3](https://github.com/w3c/htmldiff-nav/pull/3)
- Editor tooling: [whatwg-editor-dashboard](https://github.com/zcorpan/whatwg-editor-dashboard/pull/2), [whatwg-contrib-report](https://github.com/zcorpan/whatwg-contrib-report)

## Mozilla standards positions and explainers

- Filed [#1336](https://github.com/mozilla/standards-positions/issues/1336), [#1337](https://github.com/mozilla/standards-positions/issues/1337), [#1382](https://github.com/mozilla/standards-positions/issues/1382) (idscope, with [WICG/idrefs#4](https://github.com/WICG/idrefs/pull/4))
- Commented on about 50 position threads
- Reviewed position PRs such as [#1411](https://github.com/mozilla/standards-positions/pull/1411) and [#1431](https://github.com/mozilla/standards-positions/pull/1431)
- Drafted the eyedropper-input spec: [mozilla/explainers#67](https://github.com/mozilla/explainers/pull/67)

## Interop, MDN, and governance

- Ran the interop-accessibility meetings (e.g. [#246](https://github.com/web-platform-tests/interop-accessibility/issues/246))
- Proposed AVIF for Interop: [web-platform-tests/interop#1461](https://github.com/web-platform-tests/interop/issues/1461), [wpt#62892](https://github.com/web-platform-tests/wpt/issues/62892)
- MDN gaps: [mdn/content#42970](https://github.com/mdn/content/issues/42970), [#43730](https://github.com/mdn/content/issues/43730), [w3c/editing#530](https://github.com/w3c/editing/issues/530)
- Reviewed the h1 UA styles posts: [mdn/blog#385](https://github.com/mdn/blog/pull/385)
- AI contribution policy: [whatwg/sg#262](https://github.com/whatwg/sg/issues/262), [whatwg/meta#418](https://github.com/whatwg/meta/issues/418), reviewed [whatwg/sg#285](https://github.com/whatwg/sg/pull/285)
- AI spec-research tooling: [jnjaeschke/webspec-index#27](https://github.com/jnjaeschke/webspec-index/pull/27), [noamr/web-archeologist#4](https://github.com/noamr/web-archeologist/pull/4)

## Caveats

- "Reviewed" includes a few older PRs that were only updated in 2026.
- Commit search only covers default branches, so commits pushed to other people's PR branches are missing.
- Bugzilla and Phabricator aren't included.
