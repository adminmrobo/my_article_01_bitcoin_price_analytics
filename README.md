**[한국어](#ko) · [English](#en) · [中文](#zh) · [日本語](#ja) · [Oʻzbekcha](#uz) · [Русский](#ru) · [Tiếng Việt](#vi)**

---

<a id="ko"></a>

# 암호화폐 자산의 정보 효율성에 대한 연구 — 해설 대시보드

코인 값이 며칠 전에 움직인 방향이 오늘 코스피의 움직임을 미리 알려 줄 수 있을까? 안상선(2021)의 논문 「암호화폐 자산의 정보 효율성에 대한 연구 — 주식시장에서의 선행지표로서의 정보 효율성을 중심으로」(『미래사회』 12권 4호, 51–73쪽)를 박사·하루(조수)·초파리 연구원·Money-Robo 네 캐릭터가 진행하는 인터랙티브 해설 페이지로 만들었습니다. 장부를 맞대고(같은 날 상관), 밀고(시차 상관), 나누고(코로나19 전후), 합쳐 보면서(섞은 지표 K1) 논문의 네 가지 연구 질문을 직접 따라갈 수 있습니다.

- **바로 보기:** https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.html
- **원문 논문 (KCI):** https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART002795323
- **저자:** 글 · 안상선 ((주)M-Robo 대표)

## 언어

페이지는 7개 언어로 볼 수 있습니다: 한국어 · English · 中文 · 日本語 · Oʻzbekcha · Русский · Tiếng Việt

- **고르는 방법:** 맨 위 메뉴의 🌐 선택 상자, 또는 화면 오른쪽 아래의 🌐 배너를 누릅니다. 고른 언어는 브라우저에 기억되어, 다음에 한국어 주소로 들어와도 그 언어로 열립니다.
- **자동 전환:** 한국어 페이지로 처음 들어오면 브라우저 언어가 지원 언어일 때 그 언어 파일로 옮겨 갑니다. 지원하지 않는 언어는 한국어 그대로입니다. 번역판 주소로 들어오면 자동으로 바뀌지 않습니다(공유한 링크는 그 언어로 열립니다).
- **주소로 고르기:** 주소 뒤에 `?lang=en`처럼 붙이면 그 언어로 열고 기억합니다. `#r2` 같은 섹션 위치는 언어를 바꿔도 유지됩니다.
- **번역하지 않은 것:** 참고문헌 목록의 한국어 원제·저자명(서지 정보 원문, 번역 제목을 괄호로 덧붙임), 캐릭터 그림 속 모양, 수식·변수 이름(BTC, KOSPI, K1 …)과 숫자.

| 언어 | 파일 이름 | 바로 보기 |
|---|---|---|
| 한국어 | `crypto_info_efficiency.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.html |
| English | `crypto_info_efficiency.en.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.en.html |
| 中文 | `crypto_info_efficiency.zh.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.zh.html |
| 日本語 | `crypto_info_efficiency.ja.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ja.html |
| Oʻzbekcha | `crypto_info_efficiency.uz.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.uz.html |
| Русский | `crypto_info_efficiency.ru.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ru.html |
| Tiếng Việt | `crypto_info_efficiency.vi.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.vi.html |

## 구성

| 순서 | 섹션 | 다루는 내용 | 난이도 |
|---|---|---|---|
| 1 | 질문 | 효율적 시장가설(약형·준강형·강형), 연구 질문 네 개, 분석 기간 | ★★ |
| 2 | 방법 | 자료 → 차분 → 같은 날 상관 → 시차 상관 → 코로나19 전후 → K1, 가성회귀 | ★★ |
| ① | 같은 날에는 | 여섯 변수 상관 지도, 연도별 상관, 상관계수 점구름 | ★★ |
| ② | 며칠 전 코인 값은 | 15·10·5·1일 전 시차 상관, 장부 밀기, 유의성(별) 계산기 | ★★★ |
| ③ | 코로나 이후 | 기간별 시차 상관과 95% 신뢰구간 | ★★★ |
| ④ | 섞은 지표 K1 | K1의 상관, 코로나 이후 시차 상관 | ★★★ |
| ⚗ | 모형 실험실 | K1 비중 조절기 — 원문 표만으로 K1 상관을 다시 계산 | ★★★★ |
| — | 대결 · 다시 읽기 · 한 장으로 | 비트코인 하나 vs K1, 장부 비유 카드, 읽을 때 주의할 점 | ★★ |
| — | 지식 색인 · 꾸러미 | 개념 검색과 미니 그래프, 온톨로지·서지 꾸러미(JSON-LD·Turtle·CSV·BibTeX·RIS) ZIP | ★★ |

## 핵심 숫자 (모두 원문 표 그대로)

| 내용 | 값 | 출처 |
|---|---|---|
| 분석 기간 | 2015.08.07 ~ 2020.08.31, 1,241일 (코로나19 이전 1,096일 / 이후 145일) | 표 3-3-2 |
| 같은 날 코스피와의 상관 | 비트코인 −0.015, 이더리움 0.036 (유의하지 않음) | 표 3-4-1 |
| 비트코인 시차 상관 (전체) | 5일 전 0.064***, 1일 전 0.067*** | 표 3-4-3 |
| 코로나19 이후 비트코인 | 5일 전 0.234***, 1일 전 0.181** | 표 3-4-5 |
| 섞은 지표 K1 | 코스피와 −0.195*** | 표 3-4-7 |

## 들어 있는 것과 주요 실습

| 실습 | 손으로 바꾸는 것 | 보이는 것 |
|---|---|---|
| 우연히 같이 오르는 두 장부 | 원값 / 하루 변화, 시드 | 무작위 걸음 200쌍의 원값·차분 상관 비교 (가성회귀) |
| 상관 점구름 | 상관계수 r | 1,240개 점구름과 기울기 |
| 장부 밀기 | 시차 k (0~15일) | 장난감 장부에서 k일 밀었을 때의 상관 |
| 별(*) 계산기 | r, 표본 수 N | t, 양측 p, 재계산 별, r², 95% 신뢰구간과 원문 표기 비교 |
| 기간별 신뢰구간 | 코인, 신뢰구간 켜기 | 코로나19 이전·이후·전체 시차 상관 |
| K1 비중 조절기 | 다섯 변수 비중, 원 단위 / 표준화 | K1–코스피 상관과 변수별 몫 (논문 비중에서 −0.195 재현) |
| 대결 | 먼저 맞혀 보기, 결과 보기 | 비트코인 하나 vs K1의 \|r\| |

각 섹션에는 장부 비유 짝 카드, 풀이 상자, 확인 퀴즈(모두 13문항), 용어 밑줄 말풍선이 있습니다. 이 페이지에는 Colab 코드가 없습니다(모든 계산은 원문 표의 숫자로 페이지 안에서 합니다).

## 파일

```
crypto_info_efficiency.html        한국어 원본
crypto_info_efficiency.en.html  .zh.html  .ja.html
crypto_info_efficiency.uz.html  .ru.html  .vi.html
index.html                         첫 화면 주소에서 한국어 원본으로 넘겨 주는 짧은 파일
README.md
```

- 모든 HTML은 그림·데이터·스크립트를 한 파일에 담았습니다. 빌드 없이 브라우저로 열기만 하면 됩니다. 외부에서 불러오는 것은 Google Fonts뿐입니다.
- 크기: 언어마다 약 0.5 MB.

## 먼저 읽으면 좋은 것

- 원문 논문(KCI 링크 위)
- 상관계수와 유의수준의 기초(페이지의 별 계산기와 용어 말풍선으로도 볼 수 있음)

## 데이터와 이미지 (설명용 모형인 것)

| 무엇 | 실제 계산인가 |
|---|---|
| 표·막대의 상관계수, 표본 수, 기초통계 | 원문 표 그대로 |
| 별 계산기의 p값, 기간별 신뢰구간 | 원문 r과 N으로 페이지가 다시 계산한 참고값 |
| K1 비중 조절기 | 원문 표 3-3-5(표준편차)와 표 3-4-1(상관)로 계산한 값. 원자료 아님 |
| 무작위 걸음, 점구름, 장부 칸 색 | 시드 고정 난수로 만든 설명용 모형 |
| 캐릭터 그림 | 공식 저장소 adminmrobo/fruitfly-lab-expressions (ea5da3f)의 캐릭터 팩 |
| 히어로·아웃트로 무대 | 캐릭터 팩 그림과 코드로 그린 임시 장면 |

## 용어 표기

- **장부:** 이 페이지의 고정 비유입니다. 같은 날 상관 = 장부 맞대기, 시차 상관 = 장부 밀기, 기간 나누기 = 장부 두 권, K1 = 합본 장부. 시계열을 처음 보는 독자도 "날짜별로 적힌 기록"으로 떠올릴 수 있어서 골랐습니다.
- **공포 온도계:** 변동성 지수 VKOSPI의 별명입니다.
- **섞은 지표 K1:** 논문의 임의 경제지표 K1(다섯 지표를 20%씩 평균)을 가리킵니다.
- **하루 변화(차분):** 전날 대비 증감액. 논문 본문의 "변화율"이라는 표현 대신 식과 기초통계에 맞춰 증감으로 적었습니다.

## 라이선스

라이선스는 아직 정하지 않았습니다(채워 넣을 것). 원 논문의 저작권은 저자와 학술지에 있습니다. 이 페이지는 연구 방법 설명이며 투자 권유가 아닙니다.

---

<a id="en"></a>

# A Study on Information Efficiency of Cryptocurrency Assets — Explainer Dashboard

Can the direction coin prices moved a few days ago tell us in advance how KOSPI moves today? This interactive explainer page turns the paper by Ahn Sangsun (2021), "A Study on Information Efficiency of Cryptocurrency Assets – Focusing on Information Efficiency as a Leading Indicator in the Stock Market" (*Journal of the Future of Society* 12(4), pp. 51–73), into a page hosted by four characters: the Doctor, Haru (Assistant), the Fruit Fly Researcher and Money-Robo. By lining up ledgers (same-day correlation), shifting them (lagged correlation), splitting them (before/after COVID-19) and binding them (blended index K1), you can follow the paper's four research questions yourself.

- **View it:** https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.en.html
- **Original paper (KCI):** https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART002795323
- **Author:** Written by Ahn Sangsun (CEO, M-Robo Co., Ltd.)

## Languages

The page is available in 7 languages: Korean · English · 中文 · 日本語 · Oʻzbekcha · Русский · Tiếng Việt

- **How to choose:** Use the 🌐 select box in the top menu, or tap the 🌐 banner at the bottom right of the screen. Your choice is remembered in the browser, so the page opens in that language even if you later come in through the Korean address.
- **Automatic switching:** The first time you open the Korean page, if your browser language is supported, you are moved to that language's file. Unsupported languages stay in Korean. Opening a translated page's address never switches automatically (shared links open in their language).
- **Choosing by address:** Add something like `?lang=en` to the address to open that language and remember it. Section positions such as `#r2` are kept when you switch languages.
- **Not translated:** the Korean original titles and author names in the reference list (original bibliographic data, with a translated title added in parentheses), the shapes inside the character art, formulas and variable names (BTC, KOSPI, K1 …) and numbers.

| Language | File name | View |
|---|---|---|
| 한국어 | `crypto_info_efficiency.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.html |
| English | `crypto_info_efficiency.en.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.en.html |
| 中文 | `crypto_info_efficiency.zh.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.zh.html |
| 日本語 | `crypto_info_efficiency.ja.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ja.html |
| Oʻzbekcha | `crypto_info_efficiency.uz.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.uz.html |
| Русский | `crypto_info_efficiency.ru.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ru.html |
| Tiếng Việt | `crypto_info_efficiency.vi.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.vi.html |

## Contents

| Order | Section | What it covers | Level |
|---|---|---|---|
| 1 | Question | Efficient market hypothesis (weak form, semi-strong form, strong form), four research questions, analysis period | ★★ |
| 2 | Method | Data → differencing → same-day correlation → lagged correlation → before/after COVID-19 → K1, spurious regression | ★★ |
| ① | On the same day | Correlation map of six variables, correlation by year, correlation point cloud | ★★ |
| ② | Coin prices from a few days earlier | Lagged correlation 15, 10, 5 and 1 days earlier, shifting the ledger, significance (star) calculator | ★★★ |
| ③ | After COVID-19 | Lagged correlation by period with 95% confidence intervals | ★★★ |
| ④ | Blended index K1 | K1's correlation, lagged correlation after COVID-19 | ★★★ |
| ⚗ | Model lab | K1 weight mixer — recompute the K1 correlation from the original tables alone | ★★★★ |
| — | Showdown · Reread · On one page | Bitcoin alone vs K1, ledger analogy cards, points to watch when reading | ★★ |
| — | Knowledge index · Package | Concept search and mini graph, ontology & bibliography package (JSON-LD, Turtle, CSV, BibTeX, RIS) as ZIP | ★★ |

## Key numbers (all exactly as in the original tables)

| Item | Value | Source |
|---|---|---|
| Analysis period | 2015.08.07 ~ 2020.08.31, 1,241 days (before COVID-19 1,096 days / after 145 days) | Table 3-3-2 |
| Same-day correlation with KOSPI | Bitcoin −0.015, Ethereum 0.036 (not significant) | Table 3-4-1 |
| Bitcoin lagged correlation (whole period) | 5 days earlier 0.064***, 1 day earlier 0.067*** | Table 3-4-3 |
| Bitcoin after COVID-19 | 5 days earlier 0.234***, 1 day earlier 0.181** | Table 3-4-5 |
| Blended index K1 | −0.195*** with KOSPI | Table 3-4-7 |

## What's inside and main hands-on activities

| Activity | What you change | What you see |
|---|---|---|
| Two ledgers that rise together by chance | Raw values / daily change, seed | Raw-value vs differenced correlations for 200 pairs of random walks (spurious regression) |
| Correlation point cloud | Correlation coefficient r | A cloud of 1,240 points and its slope |
| Shifting the ledger | Lag k (0–15 days) | The correlation when the toy ledger is shifted by k days |
| Star (*) calculator | r, sample size N | t, two-sided p, recalculated stars, r², 95% confidence interval, compared with the original notation |
| Confidence intervals by period | Coin, confidence intervals on/off | Lagged correlation before COVID-19, after COVID-19 and for the whole period |
| K1 weight mixer | Weights of the five variables, raw units / standardized | K1–KOSPI correlation and each variable's share (reproduces −0.195 with the paper's weights) |
| Showdown | Guess first, show result | \|r\| of Bitcoin alone vs K1 |

Each section has paired ledger-analogy cards, a walkthrough box, a check quiz (13 questions in total) and underlined terms with pop-up explanations. This page has no Colab code (all calculations are done inside the page from the numbers in the original tables).

## Files

```
crypto_info_efficiency.html        Korean original
crypto_info_efficiency.en.html  .zh.html  .ja.html
crypto_info_efficiency.uz.html  .ru.html  .vi.html
index.html                         short file that redirects the home address to the Korean original
README.md
```

- Each HTML file holds its images, data and scripts in a single file. No build step is needed; just open it in a browser. The only external resource is Google Fonts.
- Size: about 0.5 MB per language.

## Good to read first

- The original paper (KCI link above)
- Basics of correlation coefficients and significance levels (also available through the page's star calculator and term pop-ups)

## Data and images (what is an illustrative mock-up)

| What | Is it a real calculation? |
|---|---|
| Correlation coefficients, sample sizes and descriptive statistics in tables and bars | Exactly as in the original tables |
| p-values in the star calculator, confidence intervals by period | Reference values recalculated by the page from the original r and N |
| K1 weight mixer | Values computed from original Table 3-3-5 (standard deviations) and Table 3-4-1 (correlations). Not raw data |
| Random walks, point cloud, ledger cell colors | Illustrative models made with fixed-seed random numbers |
| Character art | Character pack from the official repository adminmrobo/fruitfly-lab-expressions (ea5da3f) |
| Hero and outro stages | Temporary scenes drawn with character-pack art and code |

## Terminology

- **Ledger:** the fixed analogy of this page. Same-day correlation = lining up ledgers, lagged correlation = shifting the ledger, splitting the period = two volumes, K1 = bound ledger. It was chosen so that readers new to time series can picture "records written down by date".
- **Fear thermometer:** the nickname of the volatility index VKOSPI.
- **Blended index K1:** refers to the paper's ad hoc economic indicator K1 (an average of five indicators at 20% each).
- **Daily change (differencing):** the amount of change from the previous day. Instead of the paper text's wording "rate of change", it is written as an amount of change, to match the equations and descriptive statistics.

## License

No license has been chosen yet (to be filled in). Copyright in the original paper belongs to the author and the journal. This page explains a research method. This is not investment advice.

---

<a id="zh"></a>

# 加密货币资产的信息效率研究 — 解说仪表板

几天前币价变动的方向，能否提前告诉我们今天 KOSPI 的走势？本页把 Ahn Sangsun（2021）的论文《加密货币资产的信息效率研究——以作为股市先行指标的信息效率为中心》（《未来社会》(Journal of the Future of Society) 第12卷第4期，第51–73页）做成了由博士、Haru（助手）、果蝇研究员和 Money-Robo 四个角色主持的互动解说页面。通过账本对齐（同一天的相关）、推移账本（滞后相关）、分册（新冠疫情前后）、合订（混合指标 K1），你可以亲手跟随论文的四个研究问题。

- **直接查看：** https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.zh.html
- **原文论文 (KCI)：** https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART002795323
- **作者：** 作者 · Ahn Sangsun（M-Robo 株式会社代表）

## 语言

页面提供7种语言：한국어 · English · 中文 · 日本語 · Oʻzbekcha · Русский · Tiếng Việt

- **选择方法：** 点击顶部菜单中的 🌐 选择框，或屏幕右下角的 🌐 横幅。所选语言会保存在浏览器中，下次即使通过韩语地址进入，也会以该语言打开。
- **自动切换：** 首次进入韩语页面时，如果浏览器语言属于支持的语言，就会跳转到该语言的文件。不支持的语言保持韩语。通过译本地址进入时不会自动切换（分享的链接会以该语言打开）。
- **通过地址选择：** 在地址后加上 `?lang=en` 之类的参数，即可以该语言打开并记住。切换语言时，`#r2` 这样的章节位置会保留。
- **未翻译的内容：** 参考文献列表中的韩语原题和作者名（书目信息原文，译名附在括号中）、角色插图中的造型、公式和变量名（BTC、KOSPI、K1 …）以及数字。

| 语言 | 文件名 | 直接查看 |
|---|---|---|
| 한국어 | `crypto_info_efficiency.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.html |
| English | `crypto_info_efficiency.en.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.en.html |
| 中文 | `crypto_info_efficiency.zh.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.zh.html |
| 日本語 | `crypto_info_efficiency.ja.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ja.html |
| Oʻzbekcha | `crypto_info_efficiency.uz.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.uz.html |
| Русский | `crypto_info_efficiency.ru.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ru.html |
| Tiếng Việt | `crypto_info_efficiency.vi.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.vi.html |

## 结构

| 顺序 | 章节 | 内容 | 难度 |
|---|---|---|---|
| 1 | 问题 | 有效市场假说（弱式、半强式、强式）、四个研究问题、分析期间 | ★★ |
| 2 | 方法 | 数据 → 差分 → 同一天的相关 → 滞后相关 → 新冠疫情前后 → K1、伪回归 | ★★ |
| ① | 同一天 | 六个变量的相关地图、按年份的相关、相关系数散点云 | ★★ |
| ② | 几天前的币价 | 15、10、5、1天前的滞后相关，推移账本，显著性（星号）计算器 | ★★★ |
| ③ | 新冠疫情后 | 各期间的滞后相关与95%置信区间 | ★★★ |
| ④ | 混合指标 K1 | K1 的相关、新冠疫情后的滞后相关 | ★★★ |
| ⚗ | 模型实验室 | K1 比重调节器 — 只用原文表格重新计算 K1 的相关 | ★★★★ |
| — | 对决 · 重读 · 一页总结 | 只用比特币 vs K1、账本比喻卡片、阅读注意事项 | ★★ |
| — | 知识索引 · 资料包 | 概念搜索与迷你图谱、本体与书目包（JSON-LD·Turtle·CSV·BibTeX·RIS）ZIP | ★★ |

## 核心数字（全部与原文表格一致）

| 内容 | 值 | 出处 |
|---|---|---|
| 分析期间 | 2015.08.07 ~ 2020.08.31，1,241天（新冠疫情前 1,096天 / 后 145天） | 表 3-3-2 |
| 同一天与 KOSPI 的相关 | 比特币 −0.015，以太坊 0.036（不显著） | 表 3-4-1 |
| 比特币滞后相关（全部期间） | 5天前 0.064***，1天前 0.067*** | 表 3-4-3 |
| 新冠疫情后的比特币 | 5天前 0.234***，1天前 0.181** | 表 3-4-5 |
| 混合指标 K1 | 与 KOSPI −0.195*** | 表 3-4-7 |

## 页面内容与主要练习

| 练习 | 可以动手改变的 | 能看到的 |
|---|---|---|
| 碰巧一起上涨的两本账本 | 原始值 / 每日变化、种子 | 200对随机游走的原始值与差分相关比较（伪回归） |
| 相关散点云 | 相关系数 r | 1,240个点的散点云与斜率 |
| 推移账本 | 滞后 k（0~15天） | 在玩具账本中推移 k 天时的相关 |
| 星号（*）计算器 | r、样本数 N | t、双侧 p、重新计算的星号、r²、95%置信区间，并与原文标记比较 |
| 各期间的置信区间 | 币种、显示置信区间 | 新冠疫情前、后及全部期间的滞后相关 |
| K1 比重调节器 | 五个变量的比重、原单位 / 标准化 | K1–KOSPI 相关与各变量的份额（在论文比重下复现 −0.195） |
| 对决 | 先猜一猜、查看结果 | 只用比特币 vs K1 的 \|r\| |

每个章节都有账本比喻配对卡片、解读框、小测验（共13题）和带下划线术语的释义气泡。本页没有 Colab 代码（所有计算都在页面内用原文表格中的数字完成）。

## 文件

```
crypto_info_efficiency.html        韩语原版
crypto_info_efficiency.en.html  .zh.html  .ja.html
crypto_info_efficiency.uz.html  .ru.html  .vi.html
index.html                         从首页地址跳转到韩语原版的简短文件
README.md
```

- 所有 HTML 都把图片、数据和脚本放在一个文件里。无需构建，用浏览器打开即可。唯一从外部加载的是 Google Fonts。
- 大小：每种语言约 0.5 MB。

## 建议先读

- 原文论文（见上方 KCI 链接）
- 相关系数与显著性水平的基础知识（也可以通过页面中的星号计算器和术语气泡了解）

## 数据与图片（哪些是示意模型）

| 内容 | 是否为实际计算 |
|---|---|
| 表格和柱状图中的相关系数、样本数、描述统计 | 与原文表格一致 |
| 星号计算器的 p 值、各期间的置信区间 | 本页根据原文 r 和 N 重新计算的参考值 |
| K1 比重调节器 | 用原文表 3-3-5（标准差）和表 3-4-1（相关）计算的值。非原始数据 |
| 随机游走、散点云、账本格子的颜色 | 用固定种子随机数生成的示意模型 |
| 角色插图 | 官方仓库 adminmrobo/fruitfly-lab-expressions (ea5da3f) 的角色包 |
| 开场与尾声舞台 | 用角色包插图和代码绘制的临时场景 |

## 术语说明

- **账本：** 本页固定使用的比喻。同一天的相关 = 账本对齐，滞后相关 = 推移账本，划分期间 = 两册账本，K1 = 合订账本。之所以选它，是因为初次接触时间序列的读者也能把它想象成“按日期记下的记录”。
- **恐慌温度计：** 波动率指数 VKOSPI 的昵称。
- **混合指标 K1：** 指论文中的自定义经济指标 K1（五个指标各取20%平均）。
- **每日变化（差分）：** 较前一天的增减额。论文正文用了“变化率”的说法，这里按照公式和描述统计写作增减。

## 许可证

许可证尚未确定（待填写）。原论文的著作权归作者和学术期刊所有。本页是对研究方法的说明，不构成投资建议。

---

<a id="ja"></a>

# 暗号資産の情報効率性に関する研究 — 解説ダッシュボード

コインの値が数日前に動いた方向は、今日のKOSPIの動きを前もって教えてくれるのだろうか？ アン・サンソン（2021）の論文「暗号資産の情報効率性に関する研究――株式市場における先行指標としての情報効率性を中心に」（『未来社会』(Journal of the Future of Society) 12巻4号、51–73頁）を、博士・ハル（助手）・ショウジョウバエ研究員・Money-Roboの4人のキャラクターが案内するインタラクティブ解説ページにした。帳簿を並べ（同じ日の相関）、ずらし（ラグ相関）、分け（コロナ19以前・以後）、綴じ合わせながら（混合指標K1）、論文の4つの研究課題を自分でたどることができる。

- **すぐに見る：** https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ja.html
- **原論文 (KCI)：** https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART002795323
- **著者：** 文・アン・サンソン（株式会社M-Robo代表）

## 言語

ページは7言語で閲覧できる：한국어 · English · 中文 · 日本語 · Oʻzbekcha · Русский · Tiếng Việt

- **選び方：** 最上部メニューの🌐選択ボックス、または画面右下の🌐バナーを押す。選んだ言語はブラウザに記憶され、次に韓国語版のアドレスから入ってもその言語で開く。
- **自動切り替え：** 韓国語ページに初めて入ったとき、ブラウザの言語が対応言語であれば、その言語のファイルに移動する。対応していない言語では韓国語のままである。翻訳版のアドレスから入った場合は自動では切り替わらない（共有したリンクはその言語で開く）。
- **アドレスで選ぶ：** アドレスの後ろに `?lang=en` のように付けると、その言語で開いて記憶する。`#r2` のようなセクションの位置は、言語を切り替えても保たれる。
- **翻訳していないもの：** 参考文献リストの韓国語の原題・著者名（書誌情報の原文。翻訳タイトルを括弧で付記）、キャラクターの絵の中の形、数式・変数名（BTC, KOSPI, K1 …）と数字。

| 言語 | ファイル名 | すぐに見る |
|---|---|---|
| 한국어 | `crypto_info_efficiency.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.html |
| English | `crypto_info_efficiency.en.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.en.html |
| 中文 | `crypto_info_efficiency.zh.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.zh.html |
| 日本語 | `crypto_info_efficiency.ja.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ja.html |
| Oʻzbekcha | `crypto_info_efficiency.uz.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.uz.html |
| Русский | `crypto_info_efficiency.ru.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ru.html |
| Tiếng Việt | `crypto_info_efficiency.vi.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.vi.html |

## 構成

| 順序 | セクション | 扱う内容 | 難易度 |
|---|---|---|---|
| 1 | 問い | 効率的市場仮説（ウィーク型・セミストロング型・ストロング型）、4つの研究課題、分析期間 | ★★ |
| 2 | 方法 | 資料 → 差分 → 同じ日の相関 → ラグ相関 → コロナ19以前・以後 → K1、見せかけの回帰 | ★★ |
| ① | 同じ日には | 6変数の相関マップ、年別の相関、相関係数の点の雲 | ★★ |
| ② | 数日前のコイン値は | 15・10・5・1日前のラグ相関、帳簿をずらす、有意性（星）計算機 | ★★★ |
| ③ | コロナ以後 | 期間別のラグ相関と95%信頼区間 | ★★★ |
| ④ | 混合指標K1 | K1の相関、コロナ以後のラグ相関 | ★★★ |
| ⚗ | モデル実験室 | K1比重調整器 — 原文の表だけでK1の相関を計算し直す | ★★★★ |
| — | 対決 · 読み直し · 1枚で | ビットコイン1つ vs K1、帳簿のたとえカード、読むときの注意点 | ★★ |
| — | 知識索引 · パッケージ | 概念検索とミニグラフ、オントロジー・書誌パッケージ（JSON-LD・Turtle・CSV・BibTeX・RIS）ZIP | ★★ |

## 主要な数字（すべて原文の表のまま）

| 内容 | 値 | 出典 |
|---|---|---|
| 分析期間 | 2015.08.07 ~ 2020.08.31、1,241日（コロナ19以前1,096日 / 以後145日） | 表3-3-2 |
| 同じ日のKOSPIとの相関 | ビットコイン −0.015、イーサリアム 0.036（有意でない） | 表3-4-1 |
| ビットコインのラグ相関（全期間） | 5日前 0.064***、1日前 0.067*** | 表3-4-3 |
| コロナ19以後のビットコイン | 5日前 0.234***、1日前 0.181** | 表3-4-5 |
| 混合指標K1 | KOSPIと −0.195*** | 表3-4-7 |

## 収録内容と主な実習

| 実習 | 手で変えるもの | 見えるもの |
|---|---|---|
| 偶然一緒に上がる2冊の帳簿 | 原値 / 1日の変化、シード | ランダムウォーク200組の原値・差分の相関比較（見せかけの回帰） |
| 相関の点の雲 | 相関係数 r | 1,240個の点の雲と傾き |
| 帳簿をずらす | ラグ k（0〜15日） | おもちゃの帳簿でk日ずらしたときの相関 |
| 星（*）計算機 | r、標本数 N | t、両側 p、再計算の星、r²、95%信頼区間と原文表記の比較 |
| 期間別の信頼区間 | コイン、信頼区間の表示 | コロナ19以前・以後・全期間のラグ相関 |
| K1比重調整器 | 5変数の比重、元の単位 / 標準化 | K1–KOSPI相関と変数別の寄与（論文の比重で−0.195を再現） |
| 対決 | 先に予想してみる、結果を見る | ビットコイン1つ vs K1の \|r\| |

各セクションには、帳簿のたとえの対カード、解説ボックス、確認クイズ（全13問）、用語の下線吹き出しがある。このページにはColabのコードはない（すべての計算は原文の表の数字を使ってページ内で行う）。

## ファイル

```
crypto_info_efficiency.html        韓国語の原本
crypto_info_efficiency.en.html  .zh.html  .ja.html
crypto_info_efficiency.uz.html  .ru.html  .vi.html
index.html                         トップのアドレスから韓国語の原本へ転送する短いファイル
README.md
```

- すべてのHTMLは、図・データ・スクリプトを1つのファイルに収めている。ビルドは不要で、ブラウザで開くだけでよい。外部から読み込むのはGoogle Fontsのみである。
- サイズ：言語ごとに約0.5 MB。

## 先に読んでおくとよいもの

- 原論文（上のKCIリンク）
- 相関係数と有意水準の基礎（ページの星計算機と用語の吹き出しでも確認できる）

## データと画像（説明用の模型であるもの）

| 対象 | 実際の計算か |
|---|---|
| 表・棒の相関係数、標本数、基礎統計 | 原文の表のまま |
| 星計算機のp値、期間別の信頼区間 | 原文のrとNからページが計算し直した参考値 |
| K1比重調整器 | 原文 表3-3-5（標準偏差）と表3-4-1（相関）で計算した値。原データではない |
| ランダムウォーク、点の雲、帳簿のマスの色 | シード固定の乱数で作った説明用モデル |
| キャラクターの絵 | 公式リポジトリ adminmrobo/fruitfly-lab-expressions (ea5da3f) のキャラクターパック |
| ヒーロー・アウトロの舞台 | キャラクターパックの絵とコードで描いた仮の場面 |

## 用語の表記

- **帳簿：** このページの固定したたとえである。同じ日の相関 = 帳簿を並べる、ラグ相関 = 帳簿をずらす、期間の分割 = 帳簿2冊、K1 = 合本帳簿。時系列を初めて見る読者でも「日付ごとに記された記録」として思い浮かべられるため選んだ。
- **恐怖温度計：** ボラティリティ指数VKOSPIの呼び名である。
- **混合指標K1：** 論文独自の経済指標K1（5つの指標を20%ずつ平均）を指す。
- **1日の変化（差分）：** 前日比の増減額。論文本文の「変化率」という表現ではなく、式と基礎統計に合わせて増減と記した。

## ライセンス

ライセンスはまだ決めていない（要記入）。原論文の著作権は著者と学術誌にある。このページは研究方法の説明であり、投資の勧誘ではありません。

---

<a id="uz"></a>

# Kriptovalyuta aktivlarining axborot samaradorligi tadqiqoti — izohli dashbord

Tanga narxi bir necha kun oldin qaysi tomonga harakatlangani bugungi KOSPI harakatini oldindan aytib bera oladimi? Ahn Sangsun (2021) maqolasi “Kriptovalyuta aktivlarining axborot samaradorligi tadqiqoti – fond bozorida yetakchi indikator sifatidagi axborot samaradorligi misolida” (Journal of the Future of Society, 12-jild, 4-son, 51–73-betlar) asosida Doktor, Haru (Yordamchi), Drozofila tadqiqotchisi va Money-Robo — toʻrt qahramon olib boradigan interaktiv izoh sahifasi tayyorlandi. Daftarlarni yonma-yon qoʻyib (bir kunlik korrelyatsiya), surib (kechikishli korrelyatsiya), boʻlib (COVID-19 dan oldin va keyin) va jamlab (aralash indikator K1), maqolaning toʻrtta tadqiqot savolini oʻzingiz kuzatib borishingiz mumkin.

- **Koʻrish:** https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.uz.html
- **Asl maqola (KCI):** https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART002795323
- **Muallif:** Muallif · Ahn Sangsun (M-Robo kompaniyasi rahbari)

## Tillar

Sahifani 7 tilda koʻrish mumkin: 한국어 · English · 中文 · 日本語 · Oʻzbekcha · Русский · Tiếng Việt

- **Qanday tanlash kerak:** eng yuqoridagi menyudagi 🌐 tanlash oynasini yoki ekranning oʻng pastki burchagidagi 🌐 bannerni bosing. Tanlangan til brauzerda eslab qolinadi, shuning uchun keyingi safar koreyscha manzilga kirsangiz ham sahifa oʻsha tilda ochiladi.
- **Avtomatik almashtirish:** koreyscha sahifaga birinchi marta kirganingizda, brauzer tili qoʻllab-quvvatlanadigan tillardan biri boʻlsa, oʻsha til fayliga oʻtiladi. Qoʻllab-quvvatlanmaydigan tillarda sahifa koreyscha qoladi. Tarjima versiyasi manziliga kirsangiz, til avtomatik almashmaydi (ulashilgan havola oʻsha tilda ochiladi).
- **Manzil orqali tanlash:** manzil oxiriga `?lang=en` kabi qoʻshsangiz, sahifa oʻsha tilda ochiladi va til eslab qolinadi. `#r2` kabi boʻlim joylashuvi til almashtirilganda ham saqlanadi.
- **Tarjima qilinmaganlar:** adabiyotlar roʻyxatidagi koreyscha asl nomlar va muallif ismlari (bibliografik ma’lumot asl holida, tarjima qilingan nom qavsda qoʻshilgan), qahramonlar rasmlaridagi shakllar, formulalar va oʻzgaruvchi nomlari (BTC, KOSPI, K1 …) hamda raqamlar.

| Til | Fayl nomi | Koʻrish |
|---|---|---|
| 한국어 | `crypto_info_efficiency.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.html |
| English | `crypto_info_efficiency.en.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.en.html |
| 中文 | `crypto_info_efficiency.zh.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.zh.html |
| 日本語 | `crypto_info_efficiency.ja.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ja.html |
| Oʻzbekcha | `crypto_info_efficiency.uz.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.uz.html |
| Русский | `crypto_info_efficiency.ru.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ru.html |
| Tiếng Việt | `crypto_info_efficiency.vi.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.vi.html |

## Tuzilishi

| Tartib | Boʻlim | Mazmuni | Qiyinligi |
|---|---|---|---|
| 1 | Savol | Samarali bozor gipotezasi (kuchsiz shakl, yarim kuchli shakl, kuchli shakl), toʻrtta tadqiqot savoli, tahlil davri | ★★ |
| 2 | Usul | Ma’lumotlar → ayirma → bir kunlik korrelyatsiya → kechikishli korrelyatsiya → COVID-19 dan oldin va keyin → K1, soxta regressiya | ★★ |
| ① | Bir kunda | Olti oʻzgaruvchining korrelyatsiya xaritasi, yillar boʻyicha korrelyatsiya, korrelyatsiya nuqtalar buluti | ★★ |
| ② | Bir necha kun oldingi tanga narxi | 15, 10, 5, 1 kun oldingi kechikishli korrelyatsiya, daftarni surish, ahamiyatlilik (yulduzcha) kalkulyatori | ★★★ |
| ③ | COVID-19 dan keyin | Davrlar boʻyicha kechikishli korrelyatsiya va 95% ishonch oraligʻi | ★★★ |
| ④ | Aralash indikator K1 | K1 korrelyatsiyasi, COVID-19 dan keyingi kechikishli korrelyatsiya | ★★★ |
| ⚗ | Model laboratoriyasi | K1 ulushlarini sozlagich — faqat asl jadvallar asosida K1 korrelyatsiyasini qayta hisoblash | ★★★★ |
| — | Bellashuv · Qayta oʻqish · Bir sahifada | Faqat Bitkoin vs K1, daftar oʻxshatishi kartalari, oʻqishda e’tibor beriladigan joylar | ★★ |
| — | Bilim indeksi · Toʻplam | Tushunchalarni qidirish va mini graf, ontologiya va bibliografiya toʻplami (JSON-LD · Turtle · CSV · BibTeX · RIS) ZIP | ★★ |

## Asosiy raqamlar (hammasi asl jadvallardagidek)

| Mazmuni | Qiymat | Manba |
|---|---|---|
| Tahlil davri | 2015.08.07 ~ 2020.08.31, 1,241 kun (COVID-19 dan oldin 1,096 kun / keyin 145 kun) | 3-3-2-jadval |
| Bir kunda KOSPI bilan korrelyatsiya | Bitkoin −0.015, Efirium 0.036 (ahamiyatli emas) | 3-4-1-jadval |
| Bitkoin kechikishli korrelyatsiyasi (butun davr) | 5 kun oldin 0.064***, 1 kun oldin 0.067*** | 3-4-3-jadval |
| COVID-19 dan keyin Bitkoin | 5 kun oldin 0.234***, 1 kun oldin 0.181** | 3-4-5-jadval |
| Aralash indikator K1 | KOSPI bilan −0.195*** | 3-4-7-jadval |

## Tarkibi va asosiy mashgʻulotlar

| Mashgʻulot | Siz oʻzgartiradigan narsa | Koʻrinadigan natija |
|---|---|---|
| Tasodifan birga oʻsadigan ikki daftar | Asl qiymat / kunlik oʻzgarish, seed | 200 juft tasodifiy yurishda asl qiymatlar va ayirmalar korrelyatsiyasini solishtirish (soxta regressiya) |
| Korrelyatsiya nuqtalar buluti | Korrelyatsiya koeffitsiyenti r | 1,240 nuqtali bulut va uning qiyaligi |
| Daftarni surish | Kechikish k (0~15 kun) | Oʻyinchoq daftarda k kunga surilgandagi korrelyatsiya |
| Yulduzcha (*) kalkulyatori | r, tanlanma hajmi N | t, ikki tomonlama p, qayta hisoblangan yulduzcha, r², 95% ishonch oraligʻi va asl matndagi yozuv bilan solishtirish |
| Davrlar boʻyicha ishonch oraliqlari | Tanga, ishonch oraligʻini yoqish | COVID-19 dan oldingi, keyingi va butun davr kechikishli korrelyatsiyasi |
| K1 ulushlarini sozlagich | Besh oʻzgaruvchi ulushlari, asl birlik / standartlashtirish | K1–KOSPI korrelyatsiyasi va oʻzgaruvchilar ulushi (maqoladagi ulushlarda −0.195 takrorlanadi) |
| Bellashuv | Avval taxmin qilish, natijani koʻrish | Faqat Bitkoin vs K1 ning \|r\| qiymati |

Har bir boʻlimda daftar oʻxshatishi juft kartalari, izoh qutisi, tekshiruv testi (jami 13 ta savol) va tagiga chizilgan atamalar uchun izoh pufakchalari bor. Bu sahifada Colab kodi yoʻq (barcha hisob-kitoblar asl jadvallardagi raqamlar bilan sahifaning oʻzida bajariladi).

## Fayllar

```
crypto_info_efficiency.html        koreyscha asl nusxa
crypto_info_efficiency.en.html  .zh.html  .ja.html
crypto_info_efficiency.uz.html  .ru.html  .vi.html
index.html                         bosh sahifa manzilidan koreyscha asl nusxaga yoʻnaltiruvchi qisqa fayl
README.md
```

- Har bir HTML fayl rasmlar, ma’lumotlar va skriptlarni bitta faylda saqlaydi. Yigʻish (build) shart emas — brauzerda ochish kifoya. Tashqaridan faqat Google Fonts yuklanadi.
- Hajmi: har bir til uchun taxminan 0.5 MB.

## Avval oʻqish foydali boʻlganlar

- Asl maqola (yuqoridagi KCI havolasi)
- Korrelyatsiya koeffitsiyenti va ahamiyatlilik darajasi asoslari (sahifadagi yulduzcha kalkulyatori va atamalar izoh pufakchalarida ham koʻrish mumkin)

## Ma’lumotlar va tasvirlar (tushuntirish uchun maket boʻlgan narsalar)

| Nima | Haqiqiy hisobmi |
|---|---|
| Jadval va ustunlardagi korrelyatsiya koeffitsiyentlari, tanlanma hajmi, asosiy statistika | Asl jadvallardagidek |
| Yulduzcha kalkulyatoridagi p-qiymatlar, davrlar boʻyicha ishonch oraliqlari | Sahifa asl matndagi r va N asosida qayta hisoblagan ma’lumot uchun qiymatlar |
| K1 ulushlarini sozlagich | Asl matndagi 3-3-5-jadval (standart ogʻish) va 3-4-1-jadval (korrelyatsiya) asosida hisoblangan qiymat. Xom ma’lumot emas |
| Tasodifiy yurishlar, nuqtalar buluti, daftar kataklari rangi | Belgilangan seed’li tasodifiy sonlar bilan yaratilgan tushuntirish modeli |
| Qahramonlar rasmlari | Rasmiy repozitoriy adminmrobo/fruitfly-lab-expressions (ea5da3f) dagi qahramonlar toʻplami |
| Kirish va yakun sahnalari | Qahramonlar toʻplamidagi rasmlar va kod bilan chizilgan vaqtinchalik manzara |

## Atamalar

- **Daftar:** bu sahifaning doimiy oʻxshatishi. Bir kunlik korrelyatsiya = daftarlarni yonma-yon qoʻyish, kechikishli korrelyatsiya = daftarni surish, davrlarga boʻlish = ikki jildli daftar, K1 = jamlangan daftar. Vaqt qatorlarini birinchi marta koʻrayotgan oʻquvchi ham uni “sanalar boʻyicha yozilgan yozuvlar” sifatida tasavvur qila olishi uchun tanlandi.
- **Qoʻrquv termometri:** volatillik indeksi VKOSPI ning laqabi.
- **Aralash indikator K1:** maqoladagi muallif tanlagan iqtisodiy indikator K1 (beshta indikatorning 20% dan oʻrtachasi).
- **Kunlik oʻzgarish (ayirma):** oldingi kunga nisbatan oʻsish-kamayish miqdori. Maqola matnidagi “oʻzgarish sur’ati” iborasi oʻrniga tenglama va asosiy statistikaga mos ravishda oʻsish-kamayish deb yozildi.

## Litsenziya

Litsenziya hali belgilanmagan (toʻldirilishi kerak). Asl maqolaning mualliflik huquqi muallif va jurnalga tegishli. Bu sahifa tadqiqot usulini tushuntiradi. Bu investitsiya tavsiyasi emas.

---

<a id="ru"></a>

# Исследование информационной эффективности криптовалютных активов — интерактивный разбор

Может ли направление, в котором несколько дней назад двигалась цена монеты, заранее подсказать сегодняшнее движение KOSPI? Статья Ан Сансон (2021) «Исследование информационной эффективности криптовалютных активов: информационная эффективность как опережающий индикатор фондового рынка» («Журнал будущего общества» (Journal of the Future of Society), т. 12, № 4, с. 51–73) превращена в интерактивный разбор, который ведут четыре персонажа: Доктор, Хару (ассистент), Исследователь-дрозофила и Money-Robo. Сопоставляя книги (корреляция в тот же день), сдвигая их (лаговая корреляция), разделяя (до и после COVID-19) и сшивая (смешанный индекс K1), вы сами пройдёте по четырём исследовательским вопросам статьи.

- **Открыть страницу:** https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ru.html
- **Оригинальная статья (KCI):** https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART002795323
- **Автор:** Автор · Ан Сансон (генеральный директор M-Robo Co., Ltd.)

## Языки

Страница доступна на 7 языках: 한국어 · English · 中文 · 日本語 · Oʻzbekcha · Русский · Tiếng Việt

- **Как выбрать:** нажмите на поле выбора 🌐 в верхнем меню или на баннер 🌐 в правом нижнем углу экрана. Выбранный язык запоминается в браузере, и в следующий раз страница откроется на нём, даже если вы зайдёте по корейскому адресу.
- **Автоматическое переключение:** при первом заходе на корейскую страницу, если язык браузера поддерживается, вы попадёте на файл этого языка. Если язык не поддерживается, страница остаётся корейской. При заходе по адресу перевода язык автоматически не меняется (присланная ссылка откроется на своём языке).
- **Выбор через адрес:** добавьте к адресу, например, `?lang=en` — страница откроется на этом языке и запомнит его. Позиция раздела вроде `#r2` сохраняется и при смене языка.
- **Что не переводится:** корейские оригинальные названия и имена авторов в списке литературы (библиографические данные в оригинале, перевод названия добавлен в скобках), надписи внутри рисунков персонажей, формулы и имена переменных (BTC, KOSPI, K1 …) и числа.

| Язык | Имя файла | Открыть |
|---|---|---|
| 한국어 | `crypto_info_efficiency.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.html |
| English | `crypto_info_efficiency.en.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.en.html |
| 中文 | `crypto_info_efficiency.zh.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.zh.html |
| 日本語 | `crypto_info_efficiency.ja.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ja.html |
| Oʻzbekcha | `crypto_info_efficiency.uz.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.uz.html |
| Русский | `crypto_info_efficiency.ru.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ru.html |
| Tiếng Việt | `crypto_info_efficiency.vi.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.vi.html |

## Структура

| № | Раздел | О чём | Сложность |
|---|---|---|---|
| 1 | Вопрос | Гипотеза эффективного рынка (слабая, полусильная, сильная форма), четыре исследовательских вопроса, период анализа | ★★ |
| 2 | Метод | Данные → взятие разностей → корреляция в тот же день → лаговая корреляция → до и после COVID-19 → K1, ложная регрессия | ★★ |
| ① | В тот же день | Карта корреляций шести переменных, корреляции по годам, облако точек для коэффициента корреляции | ★★ |
| ② | Цена монеты несколько дней назад | Лаговая корреляция 15, 10, 5 и 1 день назад, сдвиг книги, калькулятор звёздочек (*) | ★★★ |
| ③ | После COVID-19 | Лаговые корреляции по периодам и 95% доверительные интервалы | ★★★ |
| ④ | Смешанный индекс K1 | Корреляция K1, лаговые корреляции после COVID-19 | ★★★ |
| ⚗ | Модельная лаборатория | Регулятор весов K1 — пересчёт корреляции K1 только по таблицам оригинала | ★★★★ |
| — | Поединок · Перечитать · На одной странице | Один биткоин vs K1, карточки с аналогией книги, на что обратить внимание | ★★ |
| — | Указатель знаний · Пакет | Поиск понятий и мини-граф, ZIP-пакет онтологии и библиографии (JSON-LD·Turtle·CSV·BibTeX·RIS) | ★★ |

## Ключевые числа (все — из таблиц оригинала без изменений)

| Что | Значение | Источник |
|---|---|---|
| Период анализа | 2015.08.07 ~ 2020.08.31, 1,241 день (до COVID-19 — 1,096 дней / после — 145 дней) | табл. 3-3-2 |
| Корреляция с KOSPI в тот же день | биткоин −0.015, эфириум 0.036 (не значимы) | табл. 3-4-1 |
| Лаговая корреляция биткоина (весь период) | 5 дней назад 0.064***, 1 день назад 0.067*** | табл. 3-4-3 |
| Биткоин после COVID-19 | 5 дней назад 0.234***, 1 день назад 0.181** | табл. 3-4-5 |
| Смешанный индекс K1 | с KOSPI −0.195*** | табл. 3-4-7 |

## Что внутри и основные эксперименты

| Эксперимент | Что вы меняете | Что видно |
|---|---|---|
| Две книги, которые растут вместе случайно | исходные значения / дневное изменение, сид | Сравнение корреляций исходных значений и разностей для 200 пар случайных блужданий (ложная регрессия) |
| Облако точек корреляции | коэффициент корреляции r | Облако из 1,240 точек и его наклон |
| Сдвиг книги | лаг k (0~15 дней) | Корреляция в игрушечной книге при сдвиге на k дней |
| Калькулятор звёздочек (*) | r, размер выборки N | t, двусторонний p, звёздочки (пересчёт), r², 95% доверительный интервал и сравнение с записью оригинала |
| Доверительные интервалы по периодам | монета, показ доверительного интервала | Лаговые корреляции до, после COVID-19 и за весь период |
| Регулятор весов K1 | веса пяти переменных, исходные единицы / стандартизация | Корреляция K1–KOSPI и вклад каждой переменной (с весами статьи воспроизводится −0.195) |
| Поединок | сначала угадать, показать результат | \|r\| одного биткоина vs K1 |

В каждом разделе есть парные карточки с аналогией книги, блок разбора, проверочный тест (всего 13 вопросов) и всплывающие пояснения к подчёркнутым терминам. Кода Colab на этой странице нет (все расчёты выполняются прямо на странице по числам из таблиц оригинала).

## Файлы

```
crypto_info_efficiency.html        корейский оригинал
crypto_info_efficiency.en.html  .zh.html  .ja.html
crypto_info_efficiency.uz.html  .ru.html  .vi.html
index.html                         короткий файл: перенаправляет с начального адреса на корейский оригинал
README.md
```

- Каждый HTML-файл содержит рисунки, данные и скрипты внутри себя. Сборка не нужна — достаточно открыть его в браузере. Извне загружаются только Google Fonts.
- Размер: около 0.5 MB на каждый язык.

## Что полезно прочитать заранее

- Оригинальную статью (ссылка KCI выше)
- Основы коэффициента корреляции и уровня значимости (их можно посмотреть и в калькуляторе звёздочек и всплывающих пояснениях к терминам на странице)

## Данные и изображения (что здесь — иллюстративный макет)

| Что | Реальный ли это расчёт |
|---|---|
| Коэффициенты корреляции, размеры выборок и описательная статистика в таблицах и столбцах | Из таблиц оригинала без изменений |
| p-значения калькулятора звёздочек, доверительные интервалы по периодам | Справочные значения, пересчитанные страницей по r и N из оригинала |
| Регулятор весов K1 | Значения, рассчитанные по табл. 3-3-5 (стандартные отклонения) и табл. 3-4-1 (корреляции) оригинала. Не первичные данные |
| Случайные блуждания, облако точек, цвета ячеек книги | Иллюстративные модели на случайных числах с фиксированным сидом |
| Рисунки персонажей | Набор персонажей из официального репозитория adminmrobo/fruitfly-lab-expressions (ea5da3f) |
| Сцены вступления и финала | Временные сцены из рисунков набора персонажей и графики, нарисованной кодом |

## Термины

- **Бухгалтерская книга (книга):** постоянная аналогия этой страницы. Корреляция в тот же день = сопоставить книги, лаговая корреляция = сдвинуть книгу, разбиение периода = два тома книги, K1 = сшитая книга. Мы выбрали её, потому что даже читатель, впервые встречающий временные ряды, легко представит себе «записи по датам».
- **Термометр страха:** прозвище индекса волатильности VKOSPI.
- **Смешанный индекс K1:** произвольный экономический показатель статьи K1 (среднее пяти показателей по 20%).
- **Дневное изменение (разность):** приращение к предыдущему дню. Вместо выражения «темп изменения» из текста статьи мы пишем «приращение» — в соответствии с формулами и описательной статистикой.

## Лицензия

Лицензия пока не выбрана (нужно заполнить). Авторские права на оригинальную статью принадлежат автору и журналу. Эта страница объясняет метод исследования. Это не инвестиционная рекомендация.

---

<a id="vi"></a>

# Nghiên cứu về hiệu quả thông tin của tài sản tiền mã hóa — bảng giải thích

Hướng đi của giá coin vài ngày trước có thể báo trước chuyển động của KOSPI hôm nay không? Bài báo của Ahn Sangsun (2021) «Nghiên cứu về hiệu quả thông tin của tài sản tiền mã hóa – Tập trung vào hiệu quả thông tin như một chỉ báo dẫn dắt trên thị trường chứng khoán» (*Journal of the Future of Society*, tập 12, số 4, trang 51–73) được làm thành một trang giải thích tương tác, do bốn nhân vật Tiến sĩ · Haru (Trợ lý) · Nhà nghiên cứu Ruồi giấm · Money-Robo dẫn dắt. Bằng cách đặt sổ cạnh nhau (tương quan cùng ngày), dịch sổ (tương quan trễ), chia sổ (trước và sau COVID-19) và đóng gộp sổ (chỉ số trộn K1), bạn có thể tự mình đi theo bốn câu hỏi nghiên cứu của bài báo.

- **Xem ngay:** https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.vi.html
- **Bài báo gốc (KCI):** https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART002795323
- **Tác giả:** Tác giả · Ahn Sangsun (Giám đốc điều hành, M-Robo Co., Ltd.)

## Ngôn ngữ

Trang có thể xem bằng 7 ngôn ngữ: 한국어 · English · 中文 · 日本語 · Oʻzbekcha · Русский · Tiếng Việt

- **Cách chọn:** bấm hộp chọn 🌐 ở menu trên cùng, hoặc biểu ngữ 🌐 ở góc dưới bên phải màn hình. Ngôn ngữ bạn chọn được trình duyệt ghi nhớ, nên lần sau dù vào bằng địa chỉ tiếng Hàn, trang vẫn mở bằng ngôn ngữ đó.
- **Tự động chuyển:** lần đầu vào trang tiếng Hàn, nếu ngôn ngữ trình duyệt là một ngôn ngữ được hỗ trợ thì trang sẽ chuyển sang tệp của ngôn ngữ đó. Ngôn ngữ không được hỗ trợ thì giữ nguyên tiếng Hàn. Nếu vào bằng địa chỉ của bản dịch thì trang không tự đổi (liên kết đã chia sẻ sẽ mở đúng ngôn ngữ đó).
- **Chọn bằng địa chỉ:** thêm vào cuối địa chỉ kiểu `?lang=en` thì trang mở bằng ngôn ngữ đó và ghi nhớ. Vị trí phần như `#r2` vẫn giữ nguyên khi đổi ngôn ngữ.
- **Những gì không dịch:** tên gốc tiếng Hàn và tên tác giả trong danh mục tài liệu tham khảo (giữ nguyên thông tin thư mục gốc, kèm tên dịch trong ngoặc), hình dạng trong hình nhân vật, công thức · tên biến (BTC, KOSPI, K1 …) và các con số.

| Ngôn ngữ | Tên tệp | Xem ngay |
|---|---|---|
| 한국어 | `crypto_info_efficiency.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.html |
| English | `crypto_info_efficiency.en.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.en.html |
| 中文 | `crypto_info_efficiency.zh.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.zh.html |
| 日本語 | `crypto_info_efficiency.ja.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ja.html |
| Oʻzbekcha | `crypto_info_efficiency.uz.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.uz.html |
| Русский | `crypto_info_efficiency.ru.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.ru.html |
| Tiếng Việt | `crypto_info_efficiency.vi.html` | https://adminmrobo.github.io/my_article_01_bitcoin_price_analytics/crypto_info_efficiency.vi.html |

## Cấu trúc

| Thứ tự | Phần | Nội dung | Độ khó |
|---|---|---|---|
| 1 | Câu hỏi | Giả thuyết thị trường hiệu quả (dạng yếu · dạng bán mạnh · dạng mạnh), bốn câu hỏi nghiên cứu, giai đoạn phân tích | ★★ |
| 2 | Phương pháp | Dữ liệu → sai phân → tương quan cùng ngày → tương quan trễ → trước và sau COVID-19 → K1, hồi quy giả | ★★ |
| ① | Trong cùng ngày | Bản đồ tương quan sáu biến, tương quan theo năm, đám mây điểm của hệ số tương quan | ★★ |
| ② | Giá coin vài ngày trước | Tương quan trễ 15 · 10 · 5 · 1 ngày trước, dịch sổ, máy tính dấu sao (*) cho mức ý nghĩa | ★★★ |
| ③ | Sau COVID-19 | Tương quan trễ theo giai đoạn và khoảng tin cậy 95% | ★★★ |
| ④ | Chỉ số trộn K1 | Tương quan của K1, tương quan trễ sau COVID-19 | ★★★ |
| ⚗ | Phòng thí nghiệm mô hình | Bộ chỉnh tỷ trọng K1 — tính lại tương quan K1 chỉ từ các bảng gốc | ★★★★ |
| — | Đối đầu · Đọc lại · Gói trong một trang | Chỉ Bitcoin vs K1, thẻ so sánh sổ cái, lưu ý khi đọc | ★★ |
| — | Mục lục kiến thức · Gói tài liệu | Tìm khái niệm và đồ thị mini, gói bản thể học & thư mục (JSON-LD · Turtle · CSV · BibTeX · RIS) dạng ZIP | ★★ |

## Các con số chính (tất cả giữ nguyên như bảng gốc)

| Nội dung | Giá trị | Nguồn |
|---|---|---|
| Giai đoạn phân tích | 2015.08.07 ~ 2020.08.31, 1,241 ngày (trước COVID-19 1,096 ngày / sau 145 ngày) | Bảng 3-3-2 |
| Tương quan cùng ngày với KOSPI | Bitcoin −0.015, Ethereum 0.036 (không có ý nghĩa) | Bảng 3-4-1 |
| Tương quan trễ của Bitcoin (toàn bộ) | 5 ngày trước 0.064***, 1 ngày trước 0.067*** | Bảng 3-4-3 |
| Bitcoin sau COVID-19 | 5 ngày trước 0.234***, 1 ngày trước 0.181** | Bảng 3-4-5 |
| Chỉ số trộn K1 | Với KOSPI −0.195*** | Bảng 3-4-7 |

## Nội dung và các bài thực hành chính

| Thực hành | Bạn tự thay đổi | Bạn thấy được |
|---|---|---|
| Hai sổ cái tình cờ cùng tăng | Giá trị gốc / thay đổi trong ngày, hạt giống | So sánh tương quan giá trị gốc · sai phân của 200 cặp bước đi ngẫu nhiên (hồi quy giả) |
| Đám mây điểm tương quan | Hệ số tương quan r | Đám mây 1,240 điểm và độ dốc |
| Dịch sổ | Độ trễ k (0~15 ngày) | Tương quan khi dịch sổ đồ chơi đi k ngày |
| Máy tính dấu sao (*) | r, cỡ mẫu N | t, p hai phía, dấu sao tính lại, r², khoảng tin cậy 95% và so sánh với cách ghi trong bài gốc |
| Khoảng tin cậy theo giai đoạn | Coin, bật khoảng tin cậy | Tương quan trễ trước, sau COVID-19 và toàn bộ giai đoạn |
| Bộ chỉnh tỷ trọng K1 | Tỷ trọng năm biến, đơn vị gốc / chuẩn hóa | Tương quan K1–KOSPI và phần đóng góp của từng biến (tái lập −0.195 với tỷ trọng của bài báo) |
| Đối đầu | Đoán trước, xem kết quả | \|r\| của chỉ Bitcoin vs K1 |

Mỗi phần có thẻ so sánh sổ cái theo cặp, hộp giải thích, câu hỏi kiểm tra (tổng cộng 13 câu) và bong bóng giải thích cho từ được gạch chân. Trang này không có mã Colab (mọi phép tính đều làm ngay trong trang bằng số liệu từ bảng gốc).

## Tệp

```
crypto_info_efficiency.html        bản gốc tiếng Hàn
crypto_info_efficiency.en.html  .zh.html  .ja.html
crypto_info_efficiency.uz.html  .ru.html  .vi.html
index.html                         tệp ngắn chuyển từ địa chỉ trang đầu sang bản gốc tiếng Hàn
README.md
```

- Mỗi tệp HTML chứa sẵn hình ảnh · dữ liệu · mã trong một tệp duy nhất. Không cần build, chỉ cần mở bằng trình duyệt. Thứ duy nhất tải từ bên ngoài là Google Fonts.
- Dung lượng: khoảng 0.5 MB cho mỗi ngôn ngữ.

## Nên đọc trước

- Bài báo gốc (liên kết KCI ở trên)
- Kiến thức cơ bản về hệ số tương quan và mức ý nghĩa (cũng có thể xem qua máy tính dấu sao và bong bóng thuật ngữ trên trang)

## Dữ liệu và hình ảnh (những gì là mô hình minh họa)

| Cái gì | Có phải tính toán thật không |
|---|---|
| Hệ số tương quan, cỡ mẫu, thống kê mô tả trong bảng · biểu đồ cột | Giữ nguyên như bảng gốc |
| Giá trị p của máy tính dấu sao, khoảng tin cậy theo giai đoạn | Giá trị tham khảo do trang tính lại từ r và N trong bài gốc |
| Bộ chỉnh tỷ trọng K1 | Giá trị tính từ Bảng 3-3-5 (độ lệch chuẩn) và Bảng 3-4-1 (tương quan) của bài gốc. Không phải dữ liệu gốc |
| Bước đi ngẫu nhiên, đám mây điểm, màu ô sổ cái | Mô hình minh họa tạo bằng số ngẫu nhiên có hạt giống cố định |
| Hình nhân vật | Gói nhân vật từ kho chính thức adminmrobo/fruitfly-lab-expressions (ea5da3f) |
| Sân khấu mở đầu · kết bài | Cảnh tạm vẽ bằng hình trong gói nhân vật và mã |

## Cách dùng thuật ngữ

- **Sổ cái:** phép so sánh cố định của trang này. Tương quan cùng ngày = đặt sổ cạnh nhau, tương quan trễ = dịch sổ, chia giai đoạn = hai cuốn sổ, K1 = sổ đóng gộp. Được chọn vì cả người mới gặp chuỗi thời gian lần đầu cũng có thể hình dung đó là "ghi chép theo từng ngày".
- **Nhiệt kế nỗi sợ:** biệt danh của chỉ số biến động VKOSPI.
- **Chỉ số trộn K1:** chỉ chỉ số kinh tế tự lập K1 của bài báo (trung bình năm chỉ số, mỗi chỉ số 20%).
- **Thay đổi trong ngày (sai phân):** mức tăng giảm so với hôm trước. Thay vì cách nói "tỷ lệ thay đổi" trong thân bài, chúng tôi ghi là mức tăng giảm cho khớp với công thức và thống kê mô tả.

## Giấy phép

Giấy phép chưa được quyết định (cần điền sau). Bản quyền bài báo gốc thuộc về tác giả và tạp chí. Trang này giải thích phương pháp nghiên cứu. Đây không phải lời khuyên đầu tư.
