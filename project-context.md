# KOR-0241 marketing site context

## Scope

- Independent public marketing and study site for released app `KOR-0241` only.
- App source is read-only: `/Users/youngjunma/Documents/various test prep apps project/services/kor/02/kor-0241`.
- Android package and iOS bundle identifier: `app.mcyj.examprep.kor0241`.
- Production target: `https://mcyj.github.io/korean-housing-manager-exam-prep-web/`.

## Verified Store state — 2026-09-19

- Google Play resolves publicly for the exact package.
- Apple lookup resolves the exact bundle to track ID `6797330142` in KR, US and GB.
- Both official Store badges are active and use the same 194 × 75 px outer frame without distorting artwork.

## Content and official facts

- Korean and English routes with 10 substantive guides per locale.
- Official qualification: 주택관리사보 (`jmCd=9744`).
- Stage 1: 회계원리, 공동주택시설개론, 민법, 40 items each. The first session is 100 minutes and the second is 50 minutes.
- Stage 2: 주택관리관계법규 and 공동주택관리실무. Each subject has 24 multiple-choice plus 16 short-answer items; 80 items total in 100 minutes.
- Stage 1 requires at least 40 in every subject and a 60 average. Stage 2 applies the same thresholds, then selects the highest scores within the planned number.
- Q-Net states no general eligibility restriction, subject to statutory disqualifications and the five-year misconduct restriction.
- The 29th Stage 1 was June 27, 2026; Stage 2 is September 19, 2026, with results beginning December 2.
- Canonical sources:
  - `https://www.q-net.or.kr/man001.do?gId=59&gSite=L&id=`
  - `https://www.q-net.or.kr/crf005.do?gId=&gSite=Q&id=crf00503s02&jmCd=9744&jmInfoDivCcd=B0`
  - `https://www.q-net.or.kr/crf002.do?gId=59&gSite=L&id=crf00201`

## Design and implementation

- Visual thesis: a warm housing-sand operations board with forest-green management markers and ochre checkpoints.
- Global Korean-safe wrapping uses `word-break: keep-all` and `overflow-wrap: break-word`.
- Dependency-free static generator; GitHub Actions builds, checks and deploys `dist/` to Pages.

## Verification log

- 2026-09-19: project initialized from the proven static-site system and retargeted to KOR-0241 content, assets and Store identities.
- 2026-09-19: local build generated 34 indexable routes and 36 HTML files; the checker passed metadata, links, both exact Store identities, `keep-all`, equal marketplace frames and stale-content rejection.
- 2026-09-19: local HTTP QA returned 200 for all 34 sitemap routes and five key assets; an unknown route returned 404.
- 2026-09-19: live Store recheck returned Google Play 200 and Apple bundle `app.mcyj.examprep.kor0241`, track ID `6797330142` in KR, US and GB.
- 2026-09-19: GitHub Pages workflow run `35365268031` completed successfully.
- 2026-09-19: production QA returned 200 for all 34 sitemap routes and five key assets; an unknown route returned 404.
- 2026-09-19: production CSS contains global `word-break: keep-all` and the shared 194 × 75 px marketplace frame; the Korean home contains both exact public Store links.
