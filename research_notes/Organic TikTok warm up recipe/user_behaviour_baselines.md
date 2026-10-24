# Real-user TikTok behaviour baselines: time spent, sessions, scrolling, engagement, search, surfaces and timing

> **Method and evidence notes (read first).** In this session the environment's network policy blocked every direct page fetch (WebFetch and curl). Each host tried returned HTTP 403 on CONNECT, including arxiv.org, homes.cs.washington.edu, pewresearch.org, ofcom.org.uk, datareportal.com, socialinsider.io and wrapped.vantezzen.io. **Every figure below therefore comes from web-search result extracts of the cited pages (searches run 24 Oct 2026), not from reading the full documents.** **[verify]** marks a figure that appeared only in a secondary summary, or that conflicted between extracts; check it against the original before relying on it.
>
> Evidence-type tags:
> - **[LOG]**: primary behavioural measurement (data donation, passive-meter panel, device or app-panel logs)
> - **[TT]**: TikTok-provided or TikTok-internal
> - **[SURVEY]**: self-report
> - **[VENDOR]**: analytics or marketing-vendor benchmark
> - **[AGG]**: secondary aggregator or blog (low confidence)

## 1. Daily time spent on TikTok (global, US, UK), by age group, and new vs established users

### Takeaway
How time is measured changes the answer a great deal. Data-donation medians and UK passive metering both put the typical adult user at **~27–28 min/day**. App-panel *means* are much higher: **~70–97 min/day** globally (Android) and **~88 min/day** in the US, pulled up by heavy users. UK 18–24s spend **~55–64 min/day**, and teens and children **~1.5–2+ h/day**. New or light users start at **~30 min/day or less**. In the cohorts measured, that roughly doubles within 1–3 months and then plateaus.

### Cited Findings

#### Primary behavioural measurement (data donations, panels)
- **Zannettou et al., CHI 2024 (peer-reviewed)** [LOG]:
  - **Sample:** donated TikTok data (GDPR access requests) from **347 participants**: **9.2M video views of 4.9M unique videos**, spanning 26 Jul 2020 – 21 Feb 2022. One recruitment channel was Facebook Ads (21 Jan – 13 Feb 2022).
  - **Region:** 52% Africa, 32% North/Central America, 6.6% South America, 3% Europe, so the sample is **not representative of the US or UK**.
  - Sources: [Zannettou et al. (arXiv 2301.04945)](https://arxiv.org/pdf/2301.04945); [ACM DL](https://dl.acm.org/doi/10.1145/3613904.3642433)
- Zannettou et al.: **median daily time 1,622 s (≈27 min)**. The least active quarter spent **<834 s (13.9 min)/day** and the most active quarter **≥2,891 s (≈48 min)/day** — [UW PDF of CHI paper](https://homes.cs.washington.edu/~franzi/pdf/zannettou-tiktok-chi24.pdf)
- Zannettou et al.: average daily time and number of videos viewed **increase over a user's lifetime on the platform**, roughly **2× after 80 days**. User "attention" stays flat at ~45% over the same period — [arXiv abstract](https://arxiv.org/abs/2301.04945)
- **Washington Post reader data-donation project (published 7 Oct 2025)** [LOG, self-selected volunteers]:
  - Watch histories from **~1,100 people**. The Post's analyses use **800+ US users**, and FlowingData's summary of a later analysis says "nearly 900".
  - About **15M videos over six months**.
  - Sources: [WaPo methods piece](https://www.washingtonpost.com/technology/2025/10/07/tiktok-app-study-user-behavior-addiction/); [Nieman Lab summary](https://www.niemanlab.org/reading/a-giant-washington-post-investigation-shows-how-tiktok-keeps-its-users-scrolling-for-hours-a-day/)
- WaPo, users who typically spent **~30 min/day** at the start [WaPo interactive](https://www.washingtonpost.com/wellness/interactive/2025/tiktok-addiction-algorithm-scrolling-mental-health/):
  - After a month, more than three-quarters were spending **nearly twice as long**.
  - Within a few months the group averaged **~70 min/day**, and some users' time tripled or quadrupled.
  - **Occasional users saw the steepest increases over five months**, while heavier users stayed relatively stable.
- WaPo, as summarised secondhand: light users went from **32 → 71 min/day**, and power users stayed **near 4 h/day** — [Matt Navarra summary on Threads](https://www.threads.com/@mattnavarra/post/DPgYSXFCrXc/heres-how-tiktok-power-users-end-up-scrolling-4-hours-a-day-or-morea-washington-?hl=en) [verify]. A search extract of the interactive gives, for one month, **≈54 min/day** for the least-active cohort and **≈235 min/day** for power users — [WaPo interactive](https://www.washingtonpost.com/wellness/interactive/2025/tiktok-addiction-algorithm-scrolling-mental-health/) [verify]
- **Agarwal & Ananthakrishnan, *Management Science*** (article in advance) [LOG]:
  - **Design:** touch-level smartphone data from **~7,000 TikTok adopters** in a US opt-in **Android** panel, analysed with a difference-in-differences design.
  - **Heavy adopters** saw screen time rise by **~221 min/week**. Press coverage defines them as using TikTok **>30 min/day**, about **the top 10% of adopters**. Low-intensity adopters showed **no effect**.
  - TikTok partly replaces other social and gaming apps but expands total digital attention.
  - Sources: [INFORMS](https://pubsonline.informs.org/doi/10.1287/mnsc.2024.08260); [UW Foster School news](https://foster.uw.edu/news/research-uttara-ananthakrishnan-tiktok-addiction/)

#### UK: Ofcom Online Nation (Ipsos iris passive-measurement panel) [LOG]
- **May 2025** — [Ofcom Online Nation 2025 (pub. 10 Dec 2025)](https://www.ofcom.org.uk/siteassets/resources/documents/research-and-data/online-research/online-nation/2025/online-nations-report-2025.pdf?v=409837):
  - TikTok reached **56% of UK online adults**.
  - Daily audience rose **+37% year on year to 10.4M**.
  - The **average adult TikTok user spent 28 min/day**, and **18–34 users 49 min/day**.
  - Reach was **81% of 18–24s** and **69% of 25–34s**.
- **May 2024** — [Ofcom Online Nation 2024](https://www.ofcom.org.uk/siteassets/resources/documents/research-and-data/online-research/online-nation/2024/online-nation-2024-report.pdf?v=386238):
  - **74% of online 18–24s** visited TikTok, averaging **64 min/day**.
  - **Women 18–24: 1 h 17 min/day; men 18–24: 48 min/day.**
  - Averaged across **all online adults**, including non-users: **13 min/day**.
  - The 18–24 visitor headcount is inconsistent inside the report (2.0M vs 3.9M).
- **May 2023:** 3.8M UK 18–24 TikTok visitors averaged **55 min/day** — [Ofcom Online Nation 2023](https://www.ofcom.org.uk/siteassets/resources/documents/research-and-data/online-research/online-nation/2023/online-nation-2023-report.pdf)
- **Conflict:** a secondary site attributes **62 min/day per UK user** to Ofcom 2025, more than double Ofcom's own 28 min — [ProfileTree](https://profiletree.com/tiktok-statistics-uk) [AGG — treat as unreliable]
- **Context:** UK adults spend 4 h 30 min/day online, excluding work (Online Nation 2025) — [ISPreview](https://www.ispreview.co.uk/index.php/2025/12/ofcom-finds-uk-adults-now-spend-over-4-5-hours-online-each-day.html)
- **UK children** [LOG]:
  - Ofcom's Children's Passive Online Measurement (27 Jun 2025): **8–14s spent 2 h 59 min/day online** across smartphone, tablet and computer — [Ofcom CPOM 2025](https://www.ofcom.org.uk/siteassets/resources/documents/online-safety/research-statistics-and-data/protecting-children/ofcom-childrens-passive-online-measurement.pdf?v=408844)
  - A later Ofcom report: **TikTok = 7% (≈16 min/day) of 8–14s' online time**, and TikTok time **rises with age**. **15–17s ≈ 50 min/day** (Ipsos iris). The search extract says fieldwork ran Oct 2025 – Mar 2026 — [Ofcom Children's Online Experiences report](https://www.ofcom.org.uk/siteassets/resources/documents/online-safety/research-statistics-and-data/protecting-children/childrens-online-experiences-research-report.pdf?v=418198) [verify]

#### US
- **Pew (adults, 2025)** [SURVEY]:
  - **37%** of US adults use TikTok (21% in 2021), and **24% are daily users**.
  - **About half of 18–29s** use it at least daily, against **5% of 65+**.
  - Sources: [Pew, "8 facts about Americans and TikTok" (2 Mar 2026)](https://www.pewresearch.org/short-reads/2026/03/02/8-facts-about-americans-and-tiktok/); [Pew Social Media Use report (20 Nov 2025)](https://www.pewresearch.org/wp-content/uploads/sites/20/2025/11/PI_2025.11.20_Social-Media-Use_REPORT.pdf)
  - Pew's 2026 social-media fact sheet shows **33%**, which may be a different measure — [Pew fact sheet](https://www.pewresearch.org/internet/fact-sheet/social-media/) [verify]
- **Pew (teens)** [SURVEY]: **1,458 US teens aged 13–17**, surveyed 25 Sep – 9 Oct 2025 via Ipsos. **68%** use TikTok, and **21%** use it "almost constantly", up from 16% in 2022 — [Pew, Teens, Social Media and AI Chatbots 2025](https://www.pewresearch.org/2025/12/09/teens-social-media-and-ai-chatbots-2025/)
- **data.ai, via DataReportal** [LOG app panel/modelled]: US users spend **almost 44 h/month** in the TikTok app and open it **~9 times/day**. The DataReportal edition is unconfirmed — [DataReportal](https://datareportal.com/reports/digital-2025-sub-section-top-social-platforms) [verify]
- **Statista:** **43 h 53 min/month** per US user in 2024 — [Statista](https://www.statista.com/statistics/256347/time-spent-on-selected-mobile-social-networks-in-the-united-states)
- **eMarketer** [modelled estimate]: US adult TikTok users spend **~52–54 min/day (2025)**, per secondary citations. eMarketer's earlier forecast was **58.4 min/day for 2024** — [eMarketer](https://www.emarketer.com/content/tiktok-screen-time-will-approach-60-minutes-day-us-adult-users); [Backlinko](https://backlinko.com/tiktok-users) [verify]
- **TikTok internal data in the Kentucky AG complaint** (Oct 2024; allegations that TikTok disputes) [TT]: in a time-limit experiment, average daily **teen** use moved only from **108.5 to ~107 min** — [KUOW/NPR](https://www.kuow.org/stories/tiktok-executives-know-about-app-s-effect-on-teens-lawsuit-documents-allege); [KUNC/NPR](https://www.kunc.org/2024-10-11/lawsuit-documents-reveal-what-tiktok-executives-know-about-apps-effect-on-teenagers). A judge let the case proceed in Feb 2026 — [WKMS](https://www.wkms.org/2026-02-23/kentucky-tiktok-lawsuit-calling-app-harmful-to-teens-can-move-forward-judge-rules)
- **Qustodio** [LOG; device logs of children whose parents use Qustodio's parental-control app, a self-selected population]:
  - 2024 annual report: children averaged **~2 h/day** on TikTok globally, **+7% vs 2023**. **UK: 134 min/day; US: 132 min/day** — [Qustodio 2024 report](https://www.qustodio.com/en/research/qustodio-releases-2024-annual-report/)
  - Australia 2025: **132 min/day** — [Scoop/Qustodio](https://m.scoop.co.nz/stories/SC2602/S00021/australian-children-spent-more-than-two-hours-a-day-on-tiktok-in-2025-prior-to-ban-qustodio-report.htm)
  - UK children who use TikTok: **2 h 23 min/day** (year unclear) — [Qustodio UK insights](https://www.qustodio.com/en/research/qustodio-releases-new-uk-insights/) [verify]

#### Global
- **data.ai, via DataReportal Digital 2025** [LOG app panel]: Android users spent **~34 h 56 min/month** in TikTok in **Nov 2024**. Between Aug and Nov 2024, average session time **dipped slightly** while **sessions per month rose ~10%** — [DataReportal](https://datareportal.com/reports/digital-2025-sub-section-top-social-platforms); [BizReport](https://www.bizreport.com/research/tiktok-statistics)
- **DataReportal Digital 2026**, as cited secondhand: **1 h 37 min/day** on the Android app — [Exploding Topics](https://explodingtopics.com/blog/time-spent-on-tiktok) [AGG, verify]
- The widely repeated **95 min/day** is attributed to FT/Sensor Tower. One source dates it to **Q4 2023**, another to 2025 — [Exploding Topics](https://explodingtopics.com/blog/time-spent-on-tiktok); [Blankspaces](https://www.blankspaces.app/blog/tiktok-screen-time-statistics) [AGG, verify]
- **TikTok's own advertiser decks** (old) [TT]:
  - Nov 2018 European deck: **UK 41 min/day** (Spain 31) — [TechCrunch, Jan 2019](https://techcrunch.com/2019/01/31/leaked-tiktok-ad-deck-suggests-it-has-17m-maus-in-europe)
  - 2019 US deck: **46 min/day** — [PhoneArena](https://www.phonearena.com/news/TikTok-seeking-advertisers-reveals-info-about-its-subscribers-and-how-they-use-the-app_id131527)
  - Jan 2021 data: **89 min/day**, region unspecified — [Music Business Worldwide](https://musicbusinessworldwide.com/tiktok-users-watch-the-app-for-an-average-of-89-minutes-per-day-and-theres-732m-of-them-worldwide/)
- **TikTok's internal habit threshold** (Kentucky complaint) [TT]: a habit forms after **~260 videos**. Because videos can be as short as 8 s, that is "**under 35 minutes**" — [KUNC/NPR](https://www.kunc.org/2024-10-11/lawsuit-documents-reveal-what-tiktok-executives-know-about-apps-effect-on-teenagers)

### Inferences
- **Medians describe an "ordinary" user better than means.** Two figures represent a typical adult far better than app-panel means of 70–97 min/day, which heavy users dominate:
  - the data-donation median of 27 min (Zannettou);
  - Ofcom's 28 min/day per adult user, which probably spreads each user's monthly minutes over all days, including days without use (methodology not verified).

  The spread is wide: the interquartile range is **~14–48 min/day** (Zannettou), and power users reach ~4 h (WaPo).
- **Unit conversions.** The data.ai Android figure of 34 h 56 min/month is ≈ **70 min/day**. The US figure of ~44 h/month is ≈ **88 min/day**, which at ~9 opens/day is ≈ **10 min per open**.
- **Age gradient (UK, per-user averages):**
  - 15–17s: ~50 min
  - 18–24s: ~55–64 min (2023–24)
  - 18–34s: ~49 min (2025)
  - all adult users: 28 min

  Women aged 18–24 use TikTok noticeably more than men (77 vs 48 min/day, 2024). In the US, daily use is concentrated among under-30s (about half of 18–29s daily vs 5% of 65+).
- **New vs established users.** Three findings show that the first weeks of use sit well below established-user levels, with growth over weeks to months:
  - WaPo's light cohort started at ~30 min/day and approached ~70 min within months.
  - Only ~10% of new adopters exceeded 30 min/day in the Android panel (press-coverage definition).
  - Zannettou's daily time and videos roughly doubled after ~80 days.

  For a realistic new adult account, **~15–30 min/day in the first days** is consistent with the evidence. 45–70 min/day looks like a habituated or younger (18–24) user, and >2 h/day looks like a heavy or teen user.

#### Synthesised "ordinary user" baseline
This table is **derived** from findings across all sections of this file. It is not a figure from any single source.

| Metric | New/light user (first days–weeks) | Typical established adult | Heavy user | Main basis |
|---|---|---|---|---|
| Daily time | ~15–30 min | ~25–50 min (median ≈27; UK mean per user 28; UK 18–34 ≈49) | 2–4 h | Zannettou; Ofcom; WaPo; Agarwal & Ananthakrishnan |
| App opens/day | ~4 | ~8–10 | ~20 | WaPo; data.ai; Similarweb (secondary) |
| Sessions/day (30-min-gap definition) | ~2–4 | ~4–5 | more | Wrapped panel (skews heavy) |
| Time per app open | ~7–10 min | ~9–10 min | ~12 min | WaPo arithmetic; Similarweb 9 min 42 s (secondary) |
| Videos/day | ~40–90 | median ≈90 (IQR ≈40–170) | 170+ | Zannettou |
| Dwell before swiping | median ≈6–13 s; mean ≈18 s | same | n/a | Wrapped; WaPo; Zannettou arithmetic |
| Views watched to the end | ~45% (most users 30–50%) | ~45% | ~45% | Zannettou |
| Early abandonment | 24% before 20% of the video's length; 40% before the halfway point | same | same | Zannettou |
| Likes per video viewed | below the established rate (liking rises 1.5–2× over ~4 months), plausibly ~4–6% [speculative] | ~9% (8.8% in the Wrapped panel) | n/a | Wrapped; Zannettou |
| Comments / shares per view | very rare; on brand content ≈0.05% (comments) and ≈0.25% (shares) of views | same | n/a | Socialinsider arithmetic |
| Accounts followed | mean ~40 on day 1 of the observed history | median 144–154 total (non-posters 63) | n/a | Zannettou; Pew |
| Share of views from followed accounts | ~10% | ~10% (stable over time) | n/a | Zannettou; WaPo (~90% from non-followed creators) |
| Search | 23% ("1 in 4") search within 30 s of opening; 57% use search | same | n/a | TikTok-attributed figures |
| Posting | ~half of US adult users have never posted | same | n/a | Pew |
| Late-night share | ~11% of watch time falls 00:00–06:00 | same | n/a | Wrapped |

### Gaps
- **No primary measurement isolates brand-new accounts in their first 1–7 days.** The closest proxies are WaPo's light-user cohort, the Android-panel adopters (Agarwal & Ananthakrishnan), and Zannettou's lifetime curves, which may not start at account creation.
- **No primary US daily-minutes breakdown by age** was found; only surveys and modelled estimates. Ofcom's 2025 report did not surface a separate 18–24 minutes figure in the extracts.
- **TikTok has not published an official time-spent figure since the 2021 advertiser deck**, as far as these searches show. No TikTok Marketing Science attention or watch-time study with per-user minutes was found.
- **The Wrapped/State of the Feed daily-time figure was not captured.**
- **Most figures above could not be checked against full texts** because of the fetch block.

## 2. App opens/sessions per day and average/median session length

### Takeaway
Typical users open TikTok about **4–10 times a day**. Light and new users start at **~4 opens/day**, rising to ~8 over months. Heavy users open it **~20 times/day**.
- **Panel definition** (each foreground open is a session): sessions average **~10–11 min**.
- **Data-donation definition** (a new session after a 30-minute gap): **~4–5 sessions per active day**, with a median of **~19–26 min** each.

### Cited Findings
- **WaPo data donations** [LOG]: light users went from opening the app **~4 times/day to ~8 times/day over five months**, while heavy users stayed consistent at **~20 opens/day** — [WaPo interactive](https://www.washingtonpost.com/wellness/interactive/2025/tiktok-addiction-algorithm-scrolling-mental-health/) (via search extract) [verify]. A secondary summary says power users had "**up to 20 sessions per day**" — [Threads summary](https://www.threads.com/@mattnavarra/post/DPgYSXFCrXc/heres-how-tiktok-power-users-end-up-scrolling-4-hours-a-day-or-morea-washington-?hl=en) [verify]
- **Wrapped for TikTok "State of the Feed"** [LOG; non-peer-reviewed; self-selected panel] — [State of the Feed](https://wrapped.vantezzen.io/state-of-the-feed):
  - **Sample:** **16,981 data donations covering 464M video views**, in two waves: Dec 2024 and Mar–Jul 2026.
  - **Skew:** towards Brazil, the US and Singapore, and towards people curious about their own screen time. The authors say it "is not a representative sample of TikTok".
  - **Session definition:** a session ends after **30 minutes without a new video**.
  - **Sessions per active day** rose from **3.9 to 4.7 (+21%)** between panels.
  - **Median session length** rose from **19 to 26 min**.
  - One extract describes the median session as **~20 min covering ~30 videos** [verify].
- **data.ai, via DataReportal** [LOG app panel]:
  - **US users open TikTok ~9 times/day** (≈44 h/month).
  - Globally, **Aug → Nov 2024**: sessions per month **+~10%**, while average session time **declined slightly**.
  - Source: [DataReportal](https://datareportal.com/reports/digital-2025-sub-section-top-social-platforms)
- **Similarweb (Aug 2025, Android panel), as cited secondhand** [AGG]: **~10 opens/day**, **9 min 42 s per session**, ≈1 h 37 min/day — [SQ Magazine](https://sqmagazine.co.uk/time-spent-on-tiktok-statistics/) [verify]
- **"19 opens/day, 10 min 51 s per session, ~92 videos/day"** is widely repeated, often credited to Sensor Tower, but could not be traced to a primary source — [TTS Vibes, sessions](https://insights.ttsvibes.com/tiktok-sessions-per-day-per-user/); [TTS Vibes, session duration](https://insights.ttsvibes.com/tiktok-average-session-duration/) [AGG]. The **19 opens/day** figure matches TikTok's own **Jan 2021 advertiser deck**: "opens the app no less than 19 times in an average day", 89 min/day — [Music Business Worldwide](https://musicbusinessworldwide.com/tiktok-users-watch-the-app-for-an-average-of-89-minutes-per-day-and-theres-732m-of-them-worldwide/) [TT, old]
- **Earlier TikTok decks** [TT, old]:
  - Nov 2018 Europe: **UK, France and Germany 8 opens/day; Italy and Spain 6** — [TechCrunch](https://techcrunch.com/2019/01/31/leaked-tiktok-ad-deck-suggests-it-has-17m-maus-in-europe)
  - 2019 US: **8 opens/day, 46 min/day** — [PhoneArena](https://www.phonearena.com/news/TikTok-seeking-advertisers-reveals-info-about-its-subscribers-and-how-they-use-the-app_id131527)

### Inferences
- **"Session" means different things in different sources.**
  - App panels (data.ai, Similarweb) count each foreground open, giving **~9–11 opens/day of ~10 min**.
  - Donation analyses merge views separated by less than 30 min (Wrapped), or treat gaps over 105 s as breaks (Zannettou), giving **fewer, longer sessions (~4–5/day, ~20–26 min)**.

  A behavioural recipe should model **opens** (short bursts) nested inside a few **usage episodes** per day.
- **Minutes per open, from the WaPo figures:**
  - light users: ~32 min ÷ 4 opens ≈ **8 min**, rising to ~71 min ÷ 8 ≈ **9 min**;
  - heavy users: ~235 min ÷ 20 ≈ **12 min**.

  Minutes per open are fairly stable. Growth in total time comes mostly from **more opens per day**, which matches DataReportal's note that sessions rose while session length dipped.
- **A median established user does 3–4 sessions/day.** At Zannettou's median ~90 videos/day and Wrapped's ~30 videos per ~20-min session, that is ~3 sessions. Wrapped's 3.9–4.7 sessions/day panel is skewed towards heavier users.

### Gaps
- No peer-reviewed distribution of opens per day (median and IQR) was found. Zannettou's session metrics, if any, were not captured.
- No UK figure for opens per day was found, and no current TikTok-official figure.
- Sensor Tower's own TikTok session data could not be located; only secondary attributions.

## 3. Videos viewed per session/day; watch/dwell time per video; dwell distribution; early skips; completion; rewatch/loop

### Takeaway
The best primary data (Zannettou, CHI 2024) gives:
- a median of **~90 videos/day** (IQR ~41–170);
- **45% of views watched to the end** and **55% swiped early**;
- **24% abandoned before 20%** of the video's length and **40% before the halfway point**.

Median time on a video before swiping is **~6–13 s** (Wrapped: 6–10 s; WaPo: ~11–13 s). The mean is ≈18 s, because dwell times are right-skewed. **No credible public figure** exists for organic rewatch/loop rates, or for the exact share of organic videos skipped within 1–3 s. Paid-ad benchmarks suggest only **25–40%** of ad impressions survive past 2–3 s.

### Cited Findings
- **Zannettou et al. (CHI 2024)** [LOG] — [UW PDF](https://homes.cs.washington.edu/~franzi/pdf/zannettou-tiktok-chi24.pdf); [arXiv](https://arxiv.org/pdf/2301.04945):
  - **Videos per day:** median **≈89.9** (Q1 40.7, Q3 170.3, σ 128.9).
  - **Method:** viewing time per video was **inferred from timestamps of consecutive views**. A **105-second** threshold separated real views from breaks.
- **Zannettou et al., attention metric** — [arXiv HTML](https://arxiv.org/html/2301.04945); [arXiv abstract](https://arxiv.org/abs/2301.04945):
  - **Definition:** "attention" = inferred viewing time ÷ video duration × 100, where 100% means watched to the end.
  - **45% of video views were watched until the end**, and **55% were swiped before completion**.
  - **24% of views were "skipped quickly"**, before 20% of the video's duration, and **40% were skipped before 50%**.
  - **Most participants watched 30–50% of all their videos to the end.**
  - Attention stays **stable at ~45%** even as daily usage rises over the user's lifetime.
- **Wrapped "State of the Feed"** [LOG, self-selected]: headline "**9-second median swipe**". The panel medians are **10 s (Dec 2024 panel)** and **6 s (2026 panel)**, so the 9 s headline does not match either panel — [State of the Feed](https://wrapped.vantezzen.io/state-of-the-feed) [verify]
- **WaPo:**
  - Swipe times of roughly **11–13 s** — [WaPo interactive](https://www.washingtonpost.com/wellness/interactive/2025/tiktok-addiction-algorithm-scrolling-mental-health/) (search extract) [verify].
  - A secondary summary claims "**swipe times dropped by 1.3 to 2.2 secs**" — [Threads summary](https://www.threads.com/@mattnavarra/post/DPgYSXFCrXc/heres-how-tiktok-power-users-end-up-scrolling-4-hours-a-day-or-morea-washington-?hl=en). This may be a conflation with a separate WaPo finding: it takes skipping **~1.3 videos (2.2 for mental-health content)** to undo the effect of watching one video in full — [WaPo algorithm analysis](https://www.washingtonpost.com/technology/interactive/2025/tiktok-algorithm-mental-health/) [conflict — verify]
- **TikTok internal (Kentucky complaint)** [TT]: **260 videos ≈ "under 35 minutes"**, given videos "as short as 8 seconds" played in rapid succession — [KUNC/NPR](https://www.kunc.org/2024-10-11/lawsuit-documents-reveal-what-tiktok-executives-know-about-apps-effect-on-teenagers)
- **Masood et al., CHI 2026 (peer-reviewed)** [LOG; data donation plus ML video-content analysis] — [ACM DL](https://dl.acm.org/doi/10.1145/3772318.3790311); [arXiv 2503.20030](https://arxiv.org/pdf/2503.20030):
  - **Sample:** **100 valid participants, 3.9M unique videos**.
  - Likes and shares cause **little change in later recommendations**. Interaction correlates more with *recently seen* videos than with upcoming ones.
  - Dropping **5%** of the recommended sequence does not affect user-experience metrics; dropping **30%** does.
- **Paid-ad benchmarks** (not organic viewing) [VENDOR]:
  - TikTok **hook rate** (2–3 s views ÷ impressions) is typically **25–40%**, with 40%+ called strong. The average thumb-stop rate across video platforms is **25–35%** — [Prooflytics](https://prooflytics.io/blog/video-advertising-analytics-benchmarks)
  - TikTok Ads reports **2-second** and **6-second** video views. "Hold rate" = 6 s views ÷ 2 s views — [Coupler.io](https://www.coupler.io/ai-agent-skills/tiktok-ads-creative-analysis)
  - An unsourced rule of thumb says 6 s views on **40%+ of impressions** perform well and **under 20%** perform poorly — [Dataslayer](https://www.dataslayer.ai/blog/tiktok-ads-reporting-metrics-dashboards-2025) [low confidence]
- **Unsupported claims:** blog figures such as "**87%/71% of viewers decide within 3 seconds**" name no primary source — [Scenith](https://scenith.in/blogs/three-second-rule) [AGG — not reliable]

### Inferences
- **The dwell-time distribution is right-skewed.**
  - Median-user time ÷ videos ≈ 1,622 s ÷ 90 ≈ **18 s per video** (mean-like).
  - Median swipe times are **6–13 s**.
  - TikTok's internal "260 videos in under 35 min" implies **~8 s/video** during compulsive stretches.
  - Wrapped's "~30 videos per ~20-min session" would imply ~40 s/video. That probably includes non-viewing time (comments, pauses, the last video before the 30-min gap), so treat it with caution.
- **Organic watch-depth distribution** (from Zannettou's cumulative shares):

  | Share of views | How much of the video was watched |
  |---|---|
  | **~24%** | under 20% |
  | **~16%** | 20–50% |
  | **~15%** | 50% to just short of the end |
  | **~45%** | to the end |

  For a typical 15–30 s video, "under 20%" means leaving within roughly **3–6 s**.
- **Ad figures are only a lower bound for organic retention.** The 25–40% of paid-ad impressions that survive past 2–3 s reflect intrusive paid content, so organic early-skip rates are probably lower. That fits Zannettou's 24% of organic views abandoned before 20% of the video.
- **Videos per session:** ~90 videos/day over ~3–4 sessions gives **~25–30 videos per session** for a median user.

### Gaps
- **Rewatch/loop rates:** no credible public figure was found. TikTok does not publish them, and the extracts do not say whether Zannettou's attention metric captures views above 100% (loops).
- **Organic share skipped within the first 1–3 s:** not found. One search extract mentioned an "AdSights" ad benchmark (median 2-second view rate ~27%), but no page could be located for it, so it is **not cited**.
- **Distribution of watch time by video length:** not found.
- **Source methods:** the full methods of the Wrapped and WaPo dwell metrics could not be checked.

## 4. Engagement rates per view (viewer-side data donations vs creator-side benchmarks)

### Takeaway
**Viewer side:** ordinary users like **roughly 1 in 11 videos they watch**. The large Wrapped panel found 8.8% liked and 91% watched without a like. Liking rises with tenure, by **1.5–2× over ~4 months** (Zannettou), and is higher for creators the user follows. About **half of US adult users never post**. The median user follows **~144–154 accounts** and has **36 followers**.

**Creator side:** brand-account benchmarks put total engagements at **~3.4–4.9% of views** (or ~1.7–3.4% of followers), overwhelmingly likes. Comments run about **1–1.5% of likes** and shares about **7% of likes**. No major benchmark publishes save rates.

### Cited Findings

#### Viewer side (what ordinary users do)
- **Wrapped "State of the Feed"** [LOG, self-selected; 16,981 donations] — [State of the Feed](https://wrapped.vantezzen.io/state-of-the-feed):
  - Panelists **liked 88 in 1,000 videos watched (8.8%)**, and "**91% of videos are watched without so much as a like**".
  - On the creator side of the same panel: **75% of all likes received went to the top 1% of panelists**, and **34% had never received a single like**.
- **Zannettou et al.** [LOG] — [arXiv](https://arxiv.org/pdf/2301.04945); [ACM DL](https://dl.acm.org/doi/10.1145/3613904.3642433):
  - **1.1M like actions**, with like data available for **328 of 347** participants. Some like logs were missing, which the authors attribute to logging problems on TikTok's side.
  - Liking **increases over time: ~2× after 120 days** for videos from followed accounts and **~1.5×** for videos from accounts not followed.
  - Users like more videos from accounts they follow than from recommended accounts they don't follow.
  - One extract mentions interactions with videos from non-followed accounts rising "**from 6% to 12%**", but the metric is unclear [verify].
- **Follow growth, Zannettou et al.** [LOG]: participants followed on average **~40 accounts on day 1** of their observed history and **~350 after 120 days** — [ACM DL](https://dl.acm.org/doi/10.1145/3613904.3642433)
- **Pew, "How U.S. Adults Use TikTok" (22 Feb 2024)** [SURVEY plus direct observation of public accounts] — [Pew](https://www.pewresearch.org/internet/2024/02/22/how-u-s-adults-use-tiktok/); [Axios](https://www.axios.com/2024/02/22/pew-research-adult-tiktok-use):
  - **Sample:** **2,745 US adult TikTok users** surveyed in Aug 2023; **869** shared their handles for observation.
  - The **median user follows 154 accounts and has 36 followers**.
  - **About half have never posted a video.** The **top 25% of users by posting volume produce 98% of public videos**.
  - **Posters vs non-posters:** posters' median is **246 follows and 103 followers**; non-posters' is **63 follows and 16 followers** [verify].
  - A secondary source says the median poster had **6 public videos and 149 likes received** — [Social Media Today](https://www.socialmediatoday.com/news/new-report-looks-tiktok-usage-behaviors-the-us/708275/) [verify].
- **Pew Data Labs (8 Oct 2024)** [LOG of public lists]: the median user **follows 144 accounts**, based on 664 users with public following lists — [Pew](https://www.pewresearch.org/data-labs/2024/10/08/who-u-s-adults-follow-on-tiktok/)

#### Creator side (per-view and per-follower benchmarks; mostly brand accounts) [VENDOR]
- **Dash Social (formerly Dash Hudson), 2026 TikTok Benchmark Report** (Jul–Dec 2025 data): **4.4% engagement rate by views** and **3.4% by followers**. By industry: **Publishing 5.3%, Wellness 2.3%** (by views) — [Dash Social](https://www.dashsocial.com/social-media-benchmarks/tiktok)
- **Rival IQ** (median interactions ÷ followers; ~150 companies per industry) — [Rival IQ blog](https://www.rivaliq.com/blog/good-engagement-rate-tiktok/); [Rival IQ 2025 report](https://www.rivaliq.com/blog/social-media-industry-benchmark-report/); [Rival IQ 2024 PDF](https://get.rivaliq.com/hubfs/eBooks/2024-Rival-IQ-Social-Media-Industry-Benchmark-Report.pdf); [Quid/Rival IQ 2026](https://www.quid.com/knowledge-hub/resource-library/blog/2026-social-media-industry-benchmark-report) [verify]:

  | Measure | Report year | Median TikTok rate |
  |---|---|---|
  | Per post, by followers | 2024 | **2.63%** |
  | Per post, by followers | 2025 | **~1.73%** |
  | Per post, by followers | 2026 | **2.01%** |
  | By views | not stated | **3.4%** |

  The 1.73% figure is corroborated by [Emplicit](https://emplicit.co/tiktok-engagement-rate-benchmarks-2025/).
- **Socialinsider** (TikTok engagement measured by views) — [Socialinsider TikTok benchmarks](https://www.socialinsider.io/social-media-benchmarks/tiktok); [Socialinsider all-platform benchmarks](https://www.socialinsider.io/social-media-benchmarks) [conflicting — verify]:
  - **Rate extracts disagree.** They variously give:
    - **4.90%** average in H1 2025 (+12%), with the 1–5K follower tier at 4.20% and 100K–1M at 3.95%;
    - **3.70%** for 2025 vs 2.50% for 2024;
    - **3.85% (2024) → 4.20% (2025)**, with the 1–5K tier at 4.40%;
    - **3.85%** for H1 2026.
  - **Per-post averages (2025):** **3,492 likes, 50 comments** (comments −24% YoY) and **248 shares**.
  - **1–5K follower tier:** **330 likes/post** in 2025 (320 in 2024), and shares/post **35 → 40**.
- **Hootsuite:** average TikTok engagement rate of **~1.5%**, with **2.5–4%** called "good" and **>4%** "exceptional". This appears to be follower-based — [Hootsuite](https://blog.hootsuite.com/average-engagement-rate/) [verify]
- **SociaVault:** **4.62%** for 2025, with tier medians of **7.84%** for nano accounts (1K–10K) and **1.84%** for mega accounts — [SociaVault](https://sociavault.com/blog/good-engagement-rate-tiktok) [VENDOR, low confidence]
- **Emplifi:** median TikTok engagement rate peaked at **35.9% in Q3 2025** and fell to **27.6% in Q4 2025**. The method differs (not a by-views rate), so it is **not comparable** — [Emplifi](https://emplifi.io/resources/social-media-benchmarks/) [verify]

### Inferences
- **Likes : comments : shares on brand content.** From Socialinsider's 2025 per-post averages:
  - comments ≈ **1.4% of likes** (50 ÷ 3,492);
  - shares ≈ **7.1% of likes** (248 ÷ 3,492).

  With total engagement at **~4% of views**, that is roughly **37 likes, 0.5 comments and 2.6 shares per 1,000 views**. Saves are unknown.
- **Why viewer-side and creator-side like rates differ.** Viewers' own like rate (**~9% of videos watched**, Wrapped) is more than double brand content's like-per-view rate (**~3.5–4%**). Three likely reasons:
  1. Users like friends' and followed creators' content more (Zannettou).
  2. Brand content under-performs.
  3. The Wrapped panel skews towards engaged users.

  An ordinary user's likes should be **clustered on content they connect with**, not spread evenly.
- **New vs established engagement.** Liking grows ~1.5–2× over the first ~4 months (Zannettou), so a new user's like rate is plausibly **below** the ~9% established rate. Follows accumulate quickly early (mean ~40 on day 1, ~350 by day 120, about **2.6 follows/day on average**). That mean is likely inflated by heavy followers, and Pew's established-adult median total is only ~144–154.
- **Posting.** About half of ordinary US adult users never post (Pew), so a consumption-only first phase is normal behaviour.

### Gaps
- **Viewer-side rates for comments, shares, saves/favourites, follows per video viewed, and creator-profile visits:** no published data-donation figure found. TikTok exports include comments and favourites, but neither Zannettou nor Wrapped figures for these were captured.
- **Socialinsider:** the conflicting extracts could not be reconciled without the page.
- **Pew's "median user has 0 likes" claim,** seen in a secondary source, could not be verified.
- **Statista's TikTok likes-to-views ratio by content type** (US & Canada, 2022) exists, but its numbers were not captured — [Statista](https://www.statista.com/statistics/1373961/likes-to-views-ratio-tiktok-content-type-us-canada)
- **Save rates:** no major benchmark publishes a save rate per view.

## 5. Search behaviour

### Takeaway
Search is mainstream but secondary to the feed. Two TikTok-attributed figures:
- **57% of users use TikTok search**;
- **~1 in 4 (23%) search within 30 seconds of opening the app**.

US surveys show **41% (2024) → 49% (2026)** of consumers have used TikTok "as a search engine", and **~64–65% of Gen Z**. Only **4%** of Gen Z prefer it over Google. **No public figure for searches per day or per session** was found.

### Cited Findings
- **TikTok-attributed** [TT]:
  - "**One in four users starts searching within 30 seconds of opening the app**", stated at the launch of TikTok's Search Ads Center (World Summit) — [Adweek](https://www.adweek.com/media/tiktok-ai-powered-tools-woo-marketers-potential-ban/)
  - TikTok's Tim Natividad (Mar 2025): one in four users goes to the search results page within the first 30 seconds — [Beet.TV](https://www.beet.tv/2025/03/to-capitalize-on-search-trends-just-turn-to-tiktok-tim-natividad.html)
  - "**57%** of users use TikTok's search functionality and **23%** search for something within 30 seconds of opening the app" — [Shopify](https://www.shopify.com/za/blog/tiktok-search); [TikTok Academy search-ads module](https://www.tiktokacademy.com/student/page/3228594-the-power-search)
- **Adobe (2024)** [SURVEY]: **41%** of Americans have used TikTok as a search engine, and **64% of Gen Z** — [Adobe Express blog](https://www.adobe.com/express/learn/blog/using-tiktok-as-a-search-engine); [WARC](https://www.warc.com/content/paywall/article/warc-curated-datapoints/64-of-us-gen-z-consumers-use-tiktok-for-search/en-gb/154359)
- **Adobe (Feb 2026; 807 US consumers)** [SURVEY, via secondary summaries] — [ALM Corp](https://almcorp.com/blog/tiktok-as-search-engine-2026-data/); [ALM Corp, Gen Z](https://almcorp.com/blog/gen-z-tiktok-google-preference-drop-2026-data/); [Tomorrow's Publisher](https://tomorrowspublisher.today/new-audiences/half-of-americans-use-tiktok-for-search-study-finds/) [verify]:
  - **Usage:** **49%** have used TikTok as a search engine (41% two years earlier).
  - **By generation:** **Gen Z ~65%, Millennials 55%, Baby Boomers 12%**.
  - **Preferred content:** video tutorials (**61%**), then product reviews (**45%**).
  - **Preference over Google:** only **4% of Gen Z** are more likely to rely on TikTok than on Google, down from **8% in 2024**. Gen Z prefer Google at **89%**.
  - Gen Z were only ~15% of respondents.
- **News-seeking (related):** about **1 in 5 US adults regularly get news on TikTok** — [Pew (25 Sep 2025)](https://www.pewresearch.org/short-reads/2025/09/25/1-in-5-americans-now-regularly-get-news-on-tiktok-up-sharply-from-2020/); [Pew (19 Oct 2026)](https://www.pewresearch.org/short-reads/2026/10/19/1-in-5-americans-regularly-get-news-on-tiktok/). An extract says **53% of TikTok users** regularly get news there [verify].

### Inferences
- **A realistic pattern is occasional search, not habitual search.** A plausible model is a search early in roughly a quarter of users' app openings or days, with most viewing time on the feed. The 23% "within 30 s" figure is ambiguous: it may be a share of users or a share of sessions.
- **Search is more common among under-35s,** and is used mostly for how-to, tutorial and product queries (Adobe).

### Gaps
- **Searches per day or per session:** no published figure. TikTok's data export contains search history, so this is measurable, but no study surfaced it.
- **UK-specific TikTok search data:** none found.
- **TikTok's original 57%/23% release:** not located on a TikTok domain; the figures come via press and training material.

## 6. Use of other surfaces: For You vs Following/Friends, Explore/Discover, LIVE, Inbox/DMs, TikTok Shop

### Takeaway
For You overwhelmingly dominates viewing. Only **~10% of views come from followed accounts** (Zannettou), and that share stays flat even as follow counts grow. WaPo found users see creators they don't follow **~90%** of the time. Hard numbers on Following/Friends tab time, Explore/Discover, Inbox/DMs and LIVE time share are essentially absent from public sources. About **30% of US TikTok users** have bought via **TikTok Shop** (YouGov, May 2025).

### Cited Findings
- **Zannettou et al.** [LOG]: a median of **~10% of all video views came from followed accounts**. The share **stayed flat over time** even as average follows rose from ~40 to ~350 — [ACM DL](https://dl.acm.org/doi/10.1145/3613904.3642433); [UW PDF](https://homes.cs.washington.edu/~franzi/pdf/zannettou-tiktok-chi24.pdf)
- **WaPo** [LOG]: most users saw videos from creators they **don't follow about 90% of the time** — [YPulse summary of WaPo](https://www.ypulse.com/newsfeed/2025/10/14/once-tiktoks-algorithm-learns-users-vibe-its-hard-for-them-to-log-off/) [verify]
- **TikTok support documentation** [TT, descriptive only]:
  - The **Following feed** shows followed creators' content, ranked per user — [TikTok Support](https://www.tiktok.com/support/faq_detail?id=7655285288050104852&category=web_account)
  - The **Friends tab** shows content from followers you follow back, accounts you follow, and suggested accounts. **Some users see "Discover" in place of the Friends tab** — [TikTok Support: Friends tab](https://support.tiktok.com/en/using-tiktok/exploring-videos/friends-tab?lang=en)
  - TikTok tested an **Explore** page replacing Friends in a few regions in 2023 (old) — [TechCrunch, Apr 2023](https://techcrunch.com/2023/04/11/tiktok-considers-ditching-its-friends-tab-for-a-new-explore-experience-focused-on-discovery)
- **LIVE** [TT-commissioned survey, date unknown]: a TikTok–Ipsos study is summarised as "**1 in 5 livestreaming users watch TikTok Lives**", and **1 in 3** users name TikTok their go-to live platform for connecting with brands — [Influencer Marketing Factory](https://theinfluencermarketingfactory.com/tiktok-live-shopping-guide/) [verify; wording ambiguous]
- **TikTok Shop:**
  - **YouGov, May 2025** [SURVEY]: 1,070 US adults, including 415 TikTok users. **30% of US TikTok users have bought from TikTok Shop**, led by ages 35–54 — [YouGov](https://yougov.com/en-us/articles/52193-are-us-tiktok-users-turning-to-tiktok-shop)
  - **PartnerCentric, Feb 2025** [SURVEY]: **over one-third of Americans under 60** have made at least one TikTok Shop purchase — [PartnerCentric](https://partnercentric.com/blog/tiktok-shop-trends-statistics/)
  - **GlobalData, cited by TikTok** [TT-cited]: **76%** of consumers who engaged with TikTok Shop bought from a livestream in the past year — [TikTok Newsroom](https://newsroom.tiktok.com/en-us/tiktok-shop-is-where-shoppers-come-to-discover)

### Inferences
- **An ordinary user spends nearly all viewing time on For You,** with ~10% of views from followed accounts. Visits to the Following/Friends tab, LIVE and Shop are episodic rather than routine.
- **Shop purchasing is a minority behaviour** (about 30% of US users ever), so a new user not engaging with Shop or LIVE in the first days is normal.

### Gaps
- **Inbox/DM use** (share of users who message, messages/day): no data found.
- **Explore/Discover tab usage share:** no data found.
- **LIVE:** no data on share of daily users or minutes watched.
- **Following/Friends feed visits per day:** no data found.
- **Overall:** TikTok publishes no per-surface time split, and no data-donation study with per-surface breakdowns was captured.

## 7. Time-of-day usage patterns (peak hours) and weekday vs weekend

### Takeaway
Measured usage leans heavily into the evening and night. In the Wrapped panel, **~11% of all watching happens between midnight and 6 am**, and **about a third of usage days (30% → 36%) end after midnight**. Among UK 8–14s, **15–24% of time on major apps falls between 9 pm and 5 am**, and **51%** of TikTok-using 8–14s used it between 11 pm and 5 am at least once in four weeks. Engagement studies of posts point to **evening peaks (~6–11 pm)**. **No measured weekday-vs-weekend usage difference was found.**

### Cited Findings
- **Wrapped "State of the Feed"** [LOG, self-selected] — [State of the Feed](https://wrapped.vantezzen.io/state-of-the-feed):
  - **11% of all watching happens between midnight and 6 am.**
  - The share of **days whose scrolling ends past midnight rose from 30% to 36%** between panels.
- **Ofcom, UK children aged 8–14** [LOG passive measurement] — [Ofcom CPOM 2025](https://www.ofcom.org.uk/siteassets/resources/documents/online-safety/research-statistics-and-data/protecting-children/ofcom-childrens-passive-online-measurement.pdf?v=408844) [verify which Ofcom report]:
  - **51%** of 8–14s who use TikTok used it **between 11 pm and 5 am** at least once in a four-week period.
  - Across YouTube, Snapchat, TikTok and WhatsApp, **15–24%** of time spent falls **between 9 pm and 5 am**, and **4–10%** falls after 11 pm, depending on the platform.
- **Agarwal & Ananthakrishnan, US Android adopter panel** [LOG] — [INFORMS](https://pubsonline.informs.org/doi/10.1287/mnsc.2024.08260); [UW Foster](https://foster.uw.edu/news/research-uttara-ananthakrishnan-tiktok-addiction/):
  - TikTok's screen-time effects are **highest during late-night hours**.
  - For heavy adopters, **bedtime shifted ~84 min/week** (≈12 min/night) and **net sleep fell ~35 min/week**.
- **Posting-engagement studies** [VENDOR; these measure engagement on posts, not time in app]: Buffer analysed **7.1M posts**. Engagement peaks **6–11 pm** on most days, and **Sunday 9 am** was the single strongest slot — [Buffer](https://buffer.com/resources/best-time-to-post-on-tiktok/)

### Inferences
- **A realistic adult daily curve** is low in the morning, with modest daytime or lunchtime use and a **clear evening peak (~6–11 pm)**, plus a meaningful late-night tail of **~10% of viewing after midnight**. A uniform day would put 25% of time in 00:00–06:00, so the night is under-represented but far from empty.
- **Late-night use grows with habit.** Wrapped's rising share of days that end after midnight, and Agarwal & Ananthakrishnan's late-night concentration among heavy adopters, suggest a new or light user's activity is more concentrated in the evening, with less after midnight.

### Gaps
- **Weekday vs weekend:** no measured usage data found in Sensor Tower, data.ai, Ofcom or academic sources. Only posting-engagement blogs, which disagree, cover it.
- **Adult hour-of-day curves:** no primary log-based curve for adults; the Ofcom passive data found covers children.
- **Wrapped and WaPo:** neither hour-of-day histogram could be read because of the fetch block.
