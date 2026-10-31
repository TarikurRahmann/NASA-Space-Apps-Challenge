# Challenge Selection Guide

## NASA Space Apps Challenge-এর জন্য বাংলা Challenge বাছাই গাইড

> **এটি NASA-র official scoring rubric নয়।** এই guide-এর প্রশ্ন, scorecard, weights, threshold ও উদাহরণগুলো একটি team-কে নিজের আগ্রহ, skill, সময় ও data access অনুযায়ী challenge তুলনা করতে সাহায্য করার planning tool। Challenge বাছাইয়ের আগে আপনার বছরের official challenge statement, participant rules, event schedule ও resources পড়ুন। Statement-এ থাকা আবশ্যকতা এই guide-এর চেয়ে অগ্রাধিকার পাবে।

## ১. ভালো challenge নির্বাচন কেন গুরুত্বপূর্ণ?

একটি challenge বাছাই মানে শুধু আকর্ষণীয় title পছন্দ করা নয়। Team-কে বুঝতে হবে:

- challenge আসলে কোন সমস্যা address করতে বলছে;
- কাদের জন্য সমাধানটি এবং তারা কী করতে পারবে;
- event-এর মধ্যে প্রয়োজনীয় data ও tools পাওয়া যাবে কি না;
- team-এর দক্ষতা দিয়ে ছোট, test করা যায় এমন prototype তৈরি সম্ভব কি না;
- solution-এর ফলাফল, সীমাবদ্ধতা ও source পরিষ্কারভাবে ব্যাখ্যা করা যাবে কি না।

সবচেয়ে বড় idea বা সবচেয়ে বেশি technology-র challenge-ই সেরা নয়। ভালো fit হলো এমন challenge যার মূল requirement team বোঝে, যেটি event window-তে বাস্তবসম্মতভাবে মোকাবিলা করা যায় এবং যার সমাধান পরীক্ষা করে দেখানো সম্ভব।

## ২. Challenge selection-এর সংক্ষিপ্ত প্রক্রিয়া

```text
Official challenge list ও rules খুঁজুন
        ↓
প্রাথমিকভাবে আগ্রহের ৩–৫টি challenge shortlist
        ↓
প্রতিটির full statement পড়ুন
        ↓
Hard constraints ও data feasibility যাচাই
        ↓
Team-fit ও weighted scorecard পূরণ
        ↓
Top 2 challenge-এর ছোট scope sketch
        ↓
Team consensus-এ একটি challenge নির্বাচন
        ↓
Requirement ও decision লিখে রাখুন
```

এই ধাপগুলো পরামর্শ; এগুলো NASA-র নির্ধারিত নির্বাচন-প্রক্রিয়া নয়।

## ৩. ধাপ ১ — Official তথ্য সংগ্রহ

প্রতিটি candidate challenge-এর জন্য নিচের তথ্য official source থেকে সংগ্রহ করুন:

- [ ] Challenge-এর সম্পূর্ণ নাম ও official URL।
- [ ] Full Challenge Statement, শুধু card-এর short summary নয়।
- [ ] স্পষ্টভাবে চাওয়া deliverable, feature বা output।
- [ ] challenge page-এ দেওয়া dataset, API, tool ও resource।
- [ ] Resource-এর licence, access condition বা technical limitation।
- [ ] সময়, location, user, safety বা domain-specific constraint।
- [ ] Challenge-এর এমন কোনো শব্দ/ধারণা যা team-এর ব্যাখ্যা প্রয়োজন।
- [ ] বর্তমান বছরের event start ও submission deadline।
- [ ] Project Submission Guide ও judging guide প্রকাশিত হলে সেগুলো।

Challenge statement বা resource-এর কোনো অংশ এখনও প্রকাশিত না হলে সেটি অনুমান দিয়ে পূরণ করবেন না। “যাচাই বাকি” বলে decision sheet-এ লিখুন।

## ৪. ধাপ ২ — Longlist থেকে shortlist

প্রথমে team-এর আগ্রহের ৩–৫টি challenge বেছে নিন। Longlist তৈরির সময়:

- শুধু coding challenge খুঁজবেন না; challenge অনুযায়ী data analysis, map, game, education, story, visualization, model বা design-ও উপযুক্ত হতে পারে;
- team-এর সবচেয়ে শক্তিশালী একজন সদস্যের পছন্দকেই পুরো দলের সিদ্ধান্ত বানাবেন না;
- title-এর আকর্ষণকে পূর্ণ statement-এর difficulty বা scope-এর প্রমাণ ধরবেন না;
- challenge-এর সম্ভাব্য solution আগে থেকে ধরে নিয়ে statement-কে সেই দিকে টেনে নেবেন না।

### আগ্রহের দ্রুত pulse check

প্রত্যেক সদস্য আলাদাভাবে লিখুন:

1. কোন ২টি challenge নিয়ে সবচেয়ে বেশি আগ্রহ?
2. কোন বিষয়/দক্ষতা শিখতে চান?
3. কোন ধরনের কাজ করতে স্বচ্ছন্দ—data, coding, design, research, writing, storytelling, testing?
4. কোন challenge-এ কাজ করতে অনিচ্ছুক, এবং কেন?

এরপর মিল ও মতভেদ দেখুন। এগুলো shortlist তৈরির উপকরণ, চূড়ান্ত score নয়।

## ৫. ধাপ ৩ — Full statement বিশ্লেষণ

প্রতিটি shortlist challenge-এর জন্য একটি Requirement Card পূরণ করুন।

### Requirement Card

```text
Challenge:
Official URL:

1. Challenge যে সমস্যা address করতে বলছে:
2. Intended user/audience:
3. User-এর কাজ, সিদ্ধান্ত বা শেখার লক্ষ্য:
4. স্পষ্ট must-have requirement:
5. প্রস্তাবিত/উপলভ্য data ও resources:
6. Expected output/deliverable (statement-এ যেমন বলা):
7. গুরুত্বপূর্ণ unit, date range, definition বা technical detail:
8. Known limitation বা uncertainty:
9. Challenge-এর সঙ্গে সম্পর্কহীন হয়ে যাওয়ার ঝুঁকি:
10. এখনও যাচাই করতে হবে:
```

### Requirement থেকে prototype

প্রতিটি must-have-কে যাচাইযোগ্য বাক্যে লিখুন:

| Requirement | Prototype-এ কী দেখালে বোঝা যাবে? | কীভাবে test করব? |
|---|---|---|
| | | |
| | | |
| | | |

Challenge statement যদি নির্দিষ্ট deliverable বা constraint দেয়, সেটি এই analysis-এ অক্ষরে অক্ষরে রাখুন। Team-এর নিজস্ব idea official requirement-কে প্রতিস্থাপন করে না।

## ৬. ধাপ ৪ — Hard-constraint check

Score দেওয়ার আগে প্রতিটি challenge-এ নিচের “go/no-go” প্রশ্ন করুন। কোনো গুরুত্বপূর্ণ উত্তর “না” বা “জানি না” হলে আগে সমাধান/যাচাই করুন।

| Gate | প্রশ্ন | অবস্থা |
|---|---|---|
| Requirement বোঝা | Team কি problem ও must-have নিজেদের ভাষায় ব্যাখ্যা করতে পারে? | Yes / No / Unknown |
| Challenge fit | প্রস্তাবিত solution কি challenge-এর মূল কাজের সঙ্গে সরাসরি যুক্ত? | Yes / No / Unknown |
| সময় | Event window-তে একটি ছোট, demonstrable core feature বানানো সম্ভব? | Yes / No / Unknown |
| Data access | অন্তত sample/প্রয়োজনীয় data বা বিকল্প resource পাওয়া সম্ভব? | Yes / No / Unknown |
| Rights | দরকারি data/media/code-এর licence ও ব্যবহার-অধিকার গ্রহণযোগ্য? | Yes / No / Unknown |
| Testability | output-এর অন্তত একটি গুরুত্বপূর্ণ অংশ পরীক্ষা করা যাবে? | Yes / No / Unknown |
| Safety/ethics | কোনো privacy, safety, consent বা policy concern আছে? | None / Needs review / Blocking |
| Team commitment | সদস্যরা প্রয়োজনীয় কাজ ও decision-এ অংশ নিতে রাজি? | Yes / No / Unknown |

### Go/no-go ব্যবহারের নিয়ম

- **Go:** গুরুত্বপূর্ণ requirement বোঝা, data/rights-এর গ্রহণযোগ্য পথ আছে, scope বাস্তবসম্মত।
- **Needs review:** ছোট কোনো অজানা বিষয় আছে, যা দ্রুত official source বা sample দিয়ে যাচাই করা যাবে।
- **No-go for now:** central data/permission অনুপস্থিত, must-have অসম্ভব, বা solution-এর scope challenge-এর সঙ্গে মেলে না।

“No-go” মানে challenge খারাপ নয়। বর্তমান team, সময় বা access-এর জন্য fit নয়—এটুকুই বোঝায়।

## ৭. ধাপ ৫ — Weighted scorecard

Hard-constraint check-এর পর candidate-গুলোকে ১–৫ স্কেলে score দিন। Score হলো team-এর বর্তমান বোঝাপড়ার ওপর ভিত্তি করে; নতুন তথ্য পেলে score update করুন।

### ৭.১ Score scale

| Score | অর্থ |
|---:|---|
| **১** | খুব দুর্বল fit; বড় অজানা বা বাধা আছে |
| **২** | দুর্বল fit; প্রয়োজনীয় সহায়তা/সময় অনেক লাগবে |
| **৩** | মাঝারি fit; বাস্তবসম্মত, কিন্তু কিছু গুরুত্বপূর্ণ ঝুঁকি আছে |
| **৪** | ভালো fit; অধিকাংশ চাহিদার বাস্তবসম্মত সমাধান আছে |
| **৫** | খুব ভালো fit; requirement, resource ও team capability শক্তভাবে মেলে |

কোনো বিষয় সম্পর্কে তথ্য না থাকলে ৩ দিয়ে ঢেকে দেবেন না; **Unknown** লিখুন এবং আগে যাচাই করুন। Evidence ছাড়া confident score দেবেন না।

### ৭.২ Criteria ও weight

| বিষয় | Weight | কী বিবেচনা করবেন? |
|---|---:|---|
| Challenge ও user-এর প্রয়োজন বোঝা | ২০% | Problem, user ও প্রত্যাশিত outcome পরিষ্কার কি? |
| Event window-তে scope বাস্তবসম্মত | ২০% | Must-have কমিয়ে usable prototype শেষ করা যাবে? |
| Data/resource access ও readiness | ১৫% | Data পাওয়া, পড়া ও project-এ ব্যবহার করা সম্ভব? |
| Team skill ও কাজের আগ্রহ | ১৫% | প্রয়োজনীয় দায়িত্ব কভার এবং কাজের ইচ্ছা আছে? |
| Testability ও evidence | ১০% | ফলাফল পরীক্ষা, তুলনা বা sanity-check করা যাবে? |
| ব্যবহারকারীর উপযোগিতা/প্রভাব | ১০% | সমাধানের user ও সম্ভাব্য উপকার স্পষ্ট? |
| Licence, safety ও policy risk সামলানো | ৫% | Rights, privacy, safety ও policy-র গ্রহণযোগ্য পথ আছে? |
| Demo ও ব্যাখ্যার সক্ষমতা | ৫% | অল্প সময়ে কাজ ও ফল বোঝানো সম্ভব? |
| **মোট** | **১০০%** | |

### ৭.৩ Score হিসাব

প্রতি criterion-এর score ১–৫। Weighted total ১০০-এর মধ্যে বের করার সূত্র:

```text
Weighted total = Σ (criterion score ÷ 5 × criterion weight)
```

উদাহরণ: “Data access” score ৪, weight ১৫ হলে অবদান = `4 ÷ 5 × 15 = 12` পয়েন্ট।

### ৭.৪ Blank scorecard

| বিষয় | Weight | Score (১–৫) | Weighted points | Evidence / কারণ |
|---|---:|---:|---:|---|
| Challenge ও user-এর প্রয়োজন বোঝা | ২০ | | | |
| Event window-তে scope বাস্তবসম্মত | ২০ | | | |
| Data/resource access ও readiness | ১৫ | | | |
| Team skill ও কাজের আগ্রহ | ১৫ | | | |
| Testability ও evidence | ১০ | | | |
| ব্যবহারকারীর উপযোগিতা/প্রভাব | ১০ | | | |
| Licence, safety ও policy risk সামলানো | ৫ | | | |
| Demo ও ব্যাখ্যার সক্ষমতা | ৫ | | | |
| **Weighted total** | **১০০** | | **/100** | |

### ৭.৫ Score-এর ব্যাখ্যা

এই band-গুলোও team-এর নিজস্ব planning aid, NASA-র standard নয়:

| Weighted total | প্রাথমিক ব্যাখ্যা |
|---:|---|
| ৮০–১০০ | শক্তিশালী candidate; hard gate ও risk review শেষ হলে এগোনো যায় |
| ৬৫–৭৯ | সম্ভাবনাময়; দুর্বল criterion-এর জন্য scope/fallback ঠিক করুন |
| ৫০–৬৪ | সতর্ক থাকুন; বড় ঝুঁকি কমানো যায় কি না যাচাই করুন |
| ৫০-এর নিচে | বর্তমান team/time/resource-এ দুর্বল fit হতে পারে |

**শুধু মোট score দেখে সিদ্ধান্ত নেবেন না।** কোনো hard gate ব্যর্থ হলে high score দিয়েও তা পাশ করানো যাবে না। Safety, policy বা rights-এর blocking issue থাকলে আগে official guidance/অনুমতি যাচাই করুন।

## ৮. ধাপ ৬ — Team-fit বিশ্লেষণ

### ৮.১ Skill inventory

প্রতিটি সদস্য নিজের skill ও আগ্রহ চিহ্নিত করুন। কাউকে শুধুমাত্র “programmer” বা “non-technical” হিসেবে দেখবেন না।

| Skill/task | সদস্য(রা) | অভিজ্ঞতা | করতে আগ্রহী? | Backup আছে? |
|---|---|---|---|---|
| Challenge/domain research | | | | |
| Data discovery/analysis | | | | |
| Mapping/visualization | | | | |
| Programming/prototyping | | | | |
| UX/accessibility/design | | | | |
| Writing/storytelling | | | | |
| Testing/fact-checking | | | | |
| Demo/presentation | | | | |
| Submission/source documentation | | | | |

Skill gap থাকলেই challenge বাদ নয়। প্রশ্ন হলো, gap-টি event-এর মধ্যে শেখা বা কাজ ভাগ করে পূরণ করা সম্ভব কি না।

### ৮.২ Responsibility coverage check

প্রতিটি নির্বাচিত challenge-এর Must-have-কে প্রয়োজনীয় কাজের সঙ্গে মিলান:

| Must-have কাজ | প্রয়োজনীয় দক্ষতা | Owner | Backup | শেখার/সহায়তার plan |
|---|---|---|---|---|
| | | | | |
| | | | | |
| | | | | |

যদি critical task-এর owner বা fallback না থাকে, score করার সময় তা team-fit বা scope ঝুঁকিতে দেখান।

## ৯. ধাপ ৭ — Data ও technical feasibility

Challenge-এ data আছে মানেই তা সহজে ব্যবহারযোগ্য নয়। Prototype শুরু করার আগে সবচেয়ে ঝুঁকিপূর্ণ data assumption-টি যাচাই করুন।

### Data check

- Data source official/বিশ্বস্ত কি?
- Sample record/file বাস্তবে পাওয়া যাচ্ছে?
- Format খুলতে বা parse করতে পারবেন?
- Spatial coordinate, projection, unit, date/time range বোঝা যাচ্ছে?
- Missing data, uncertainty, resolution বা update frequency project-কে প্রভাবিত করবে?
- User-এর প্রশ্নের জন্য data যথেষ্ট relevant?
- Citation, licence বা attribution কী?
- API/key/network/rate limit-এর ওপর নির্ভরতা আছে?
- External service বন্ধ থাকলে demo-র fallback আছে?

### Technical spike

Technical spike হলো একটি ছোট feasibility test—পুরো feature নয়। যেমন:

- sample dataset download ও parse করে দেখা;
- API থেকে একটি request করা;
- sample coordinates দিয়ে map-এ একটি marker দেখানো;
- image/audio/file format browser বা tool-এ খোলে কি না দেখা;
- একটি chart বা calculation test input-এ সঠিক কি না যাচাই।

এই test-এর উদ্দেশ্য data কাজ করবে—এমন নিশ্চয়তা তৈরি করা নয়; বড় ঝুঁকি দ্রুত প্রকাশ করা।

### Data unavailable হলে সিদ্ধান্ত

1. Official resource-এ mirror, alternate format বা sample আছে কি না দেখুন।
2. Challenge statement অনুমতি দিলে সমতুল্য public dataset বিবেচনা করুন।
3. Project-এর core প্রশ্ন ছোট করুন।
4. Synthetic/mock data ব্যবহার করলে তা স্পষ্ট label করুন।
5. Actual observation বা validated result বলে mock result উপস্থাপন করবেন না।
6. কোনো বিকল্প challenge-এ যাওয়া ভালো কি না পুনরায় score করুন।

## ১০. ধাপ ৮ — Scope ও minimum viable prototype তুলনা

প্রতিটি top candidate-এর জন্য event window-তে বানানো যাবে এমন একটি MVP লিখুন।

### MVP test

এই তিনটি বাক্য পূরণ করতে না পারলে scope এখনো অস্পষ্ট:

```text
আমাদের user হলো:
Prototype-এ user এই কাজটি করতে পারবে:
আমরা demo-তে এই প্রমাণ দেখাব:
```

### Must / Should / Could তালিকা

| স্তর | অর্থ | এই challenge-এ উদাহরণ |
|---|---|---|
| **Must** | Core problem সমাধান ও statement-এর requirement পূরণে দরকার | |
| **Should** | সময় থাকলে usability/স্পষ্টতা বাড়ায় | |
| **Could** | অতিরিক্ত polish বা ভবিষ্যৎ feature | |

একটি candidate-এর Must-have শেষ করতে না পারলে সেটির score-এ scope feasibility কমান। Should/Could-এর দীর্ঘ তালিকা দিয়ে Must অসম্পূর্ণ রাখবেন না।

### Scope-risk question

- Prototype-এর core কাজ কি এক বাক্যে বলা যায়?
- একটি প্রধান user journey কি demo করা যায়?
- Core feature-এর জন্য data ও API আগে পরীক্ষা করা হয়েছে?
- Event-এর মাঝামাঝি সময়ের মধ্যে end-to-end demo সম্ভব?
- কোনো feature বাদ দিলে challenge-এ সাড়া দেওয়ার ক্ষমতা হারাবে না?

## ১১. ধাপ ৯ — Risk ও unknown তুলনা

প্রতিটি candidate-এর জন্য সর্বোচ্চ তিনটি প্রধান risk লিখুন।

| Risk/unknown | Likelihood: Low/Med/High | Impact: Low/Med/High | কীভাবে যাচাই/কমাব? | Owner | Challenge নির্বাচন আটকে দেয়? |
|---|---|---|---|---|---|
| | | | | | Yes / No |
| | | | | | Yes / No |
| | | | | | Yes / No |

### Risk-এর উদাহরণ

- Full statement-এ required output এখনও team-এর কাছে অস্পষ্ট;
- প্রয়োজনীয় dataset বড় বা জটিল;
- External API event-এর সময় অপ্রাপ্য হতে পারে;
- Team-এর কেউ projection, unit বা domain term বোঝে না;
- Project-এর user বা use case team ধরে নিয়েছে, কিন্তু statement সমর্থন করে না;
- third-party image/code/data-এর licence যাচাই হয়নি;
- solution-এর দাবি বাস্তব data দিয়ে পরীক্ষা করা যাবে না;
- অতিরিক্ত feature-এর কারণে demo বা submission অসম্পূর্ণ হওয়ার ঝুঁকি।

Risk বেশি হলেই challenge বাদ দিতে হবে না। দ্রুত test, smaller scope বা credible fallback থাকলে ঝুঁকি গ্রহণযোগ্য হতে পারে।

## ১২. ধাপ ১০ — দুইটি finalist-এর ছোট feasibility sketch

যদি scorecard-এ দুইটি challenge কাছাকাছি হয়, সঙ্গে সঙ্গে vote না দিয়ে প্রত্যেকটির জন্য সমান সময়ের ছোট sketch তৈরি করুন। এটি solution আগে থেকে তৈরি করা নয়; challenge নিয়ে pre-event work নিষিদ্ধ কি না আগে যাচাই করুন। যদি নিষেধ থাকে, hackathon শুরু হওয়ার পরে এই exercise করুন।

প্রতিটি finalist-এর জন্য লিখুন:

1. Problem statement — এক বাক্য;
2. Target user — এক বাক্য;
3. MVP — সর্বোচ্চ তিনটি core capability;
4. Data — primary source ও sample access status;
5. First demo — user কী করবে, কী output দেখবে;
6. One test — core result কীভাবে যাচাই করবেন;
7. Main risk ও fallback;
8. Team owners;
9. Challenge statement-এর কোন requirement পূরণ হবে;
10. কোন requirement এখনো প্রশ্নবিদ্ধ।

একই পরিমাণ সময় ব্যবহার করুন, যাতে একটি challenge-কে বেশি বিশদে ভেবে অন্যটিকে অন্যায্যভাবে কম score না দেন।

## ১৩. Challenge-গুলোকে topic/format অনুযায়ী তুলনা

Challenge-গুলো শুধু বিষয়ক্ষেত্র দেখে নয়, full requirement পড়ে বেছে নিন। নিচের ধরনগুলো সাধারণ ক্ষেত্র বুঝতে সহায়ক; এগুলো official categorization নয়।

| সম্ভাব্য কাজের ধরন | Team-কে কী যাচাই করতে হবে? | সম্ভাব্য skill |
|---|---|---|
| Earth observation / environment | Location/date/unit/resolution, ground truth, scale ও uncertainty | Remote sensing, GIS, data analysis, visualization |
| Planetary science / mission planning | Coordinate system, mission context, data interpretation ও scientific limit | Planetary science, mapping, simulation, research |
| Health / human spaceflight | Safety, privacy, domain evidence, uncertainty ও claim-এর সীমা | Health research, data, UX, careful communication |
| Agriculture / climate adaptation | Local context, time scale, data relevance ও recommendation-এর ঝুঁকি | Earth data, GIS, agriculture, product design |
| Education / storytelling | Intended audience, scientific accuracy, accessibility ও engagement | Writing, education, art, interaction, media |
| Game / simulation | Rules/model assumptions, balancing, user feedback ও educational purpose | Game design, coding, simulation, testing |
| Sonification / creative data | Data-to-sound mapping, scale, accessibility ও interpretation | Audio, music, data visualization, storytelling |

এগুলো সম্ভাব্য skill-এর উদাহরণ। কোনো challenge-এ এসব কাজ করতে হবে—এমন প্রতিশ্রুতি বা NASA requirement নয়; পূর্ণ statement দেখুন।

## ১৪. সিদ্ধান্ত গ্রহণ ও tie-break

### Team consensus process

1. প্রত্যেকে নিজের score independently পূরণ করুন।
2. Score-গুলোর ব্যবধান দেখুন; যেখানে ২ বা তার বেশি পার্থক্য, evidence জিজ্ঞেস করুন।
3. Unknown-গুলো research/technical spike দিয়ে যাচাই করুন।
4. Hard gate-এ unresolved failure আছে কি না দেখুন।
5. Top 2-এর MVP ও fallback তুলনা করুন।
6. প্রতিটি সদস্যকে সংক্ষেপে বলতে দিন: “এই challenge কেন ভালো fit?” এবং “কী ঝুঁকি আমি মেনে নিচ্ছি?”
7. সিদ্ধান্ত এবং বাদ পড়া বিকল্পের কারণ লিখে রাখুন।

Unanimous agreement না হলে, team আগে ঠিক করুক কীভাবে সিদ্ধান্ত নেবে—যেমন consensus, ranked vote বা agreed facilitator। কোনো পদ্ধতিকে NASA-র requirement হিসেবে উপস্থাপন করবেন না।

### Tie-break order

দুটি candidate-এর score কাছাকাছি হলে এই প্রশ্নগুলো ক্রমানুসারে করুন:

1. কোনটির challenge requirement team বেশি নির্ভুলভাবে ব্যাখ্যা করতে পারে?
2. কোনটির central dataset/tool event-এর মধ্যে ব্যবহার করা যাবে—তার evidence বেশি?
3. কোনটির MVP ছোট ও পরীক্ষাযোগ্য?
4. কোনটির critical task-এর owner ও backup আছে?
5. কোনটির safety, licence বা external dependency risk কম/সহজে নিয়ন্ত্রণযোগ্য?
6. কোনটির demo-তে evidence পরিষ্কার হবে?
7. কোনটির কাজ team সত্যি করতে আগ্রহী?

কোনো criterion-এ উত্তর অজানা হলে সেটি যাচাই করুন; অনুমানকে tie-break বানাবেন না।

## ১৫. যে ভুলগুলো challenge selection-এ এড়াবেন

| ভুল | কেন সমস্যা | ভালো বিকল্প |
|---|---|---|
| শুধু title বা buzzword দেখে বাছাই | আসল requirement ভিন্ন হতে পারে | Full statement পড়ুন |
| নিজের আগের project-এ challenge-কে জোর করে মানানো | Solution challenge-এর বাইরে চলে যেতে পারে | Problem statement থেকে শুরু করুন |
| “সব data NASA-র, তাই সহজ” ধরে নেওয়া | Format, access, resolution ও licence ভিন্ন হতে পারে | Sample data access test করুন |
| সবচেয়ে বেশি coding-ওয়ালা challenge বেছে নেওয়া | Non-code/creative output-ও challenge-এর উপযুক্ত হতে পারে | Required outcome-কে কেন্দ্র করুন |
| বেশি feature মানেই বেশি value মনে করা | Core solution অসম্পূর্ণ থেকে যায় | MVP ও Must/Should/Could নির্ধারণ করুন |
| Unknown-কে score ৩ দেওয়া | ঝুঁকি লুকিয়ে যায় | Unknown আলাদা করে লিখে test করুন |
| Score যোগ করে hard blocker ভুলে যাওয়া | উচ্চ মোট score গুরুতর blocker মুছে না | Hard gate আগে প্রয়োগ করুন |
| NASA judging criteria অনুমান করা | পুরস্কারের rubric আলাদা হতে পারে | Current Judging & Awards Guide পড়ুন |
| Challenge statement-এর সংক্ষিপ্তসারকে পূর্ণ brief ভাবা | requirement/resource বাদ পড়ে | Full statement ও resource পড়ুন |
| Team-এর একজনের আগ্রহকে সবার সিদ্ধান্ত করা | কাজের ownership ও motivation কমতে পারে | সবার input নিন, role map করুন |
| Hackathon শুরুর আগে solution-এ কাজ করা | Current-year rules-এর সঙ্গে বিরোধ হতে পারে | Start rule যাচাই; নিষেধ থাকলে অপেক্ষা করুন |

## ১৬. Ready-to-copy comparison table

| Item | Candidate A | Candidate B | Candidate C |
|---|---|---|---|
| Challenge title + URL | | | |
| Problem এক বাক্যে | | | |
| User | | | |
| Must-have requirement | | | |
| MVP এক বাক্যে | | | |
| Primary data/resource | | | |
| Data access tested? | | | |
| Main technical/domain skill | | | |
| Team owner + backup | | | |
| Test/evidence আছে? | | | |
| Main risk | | | |
| Fallback | | | |
| Hard gate status | | | |
| Weighted total / 100 | | | |
| Team interest summary | | | |
| Decision / unresolved question | | | |

## ১৭. Ready-to-copy final decision record

```text
# Challenge Selection Decision

বছর:
Event:
সিদ্ধান্তের তারিখ:
অংশগ্রহণকারী team member:

## নির্বাচিত challenge
- নাম:
- Official URL:
- Full statement version/date (যদি থাকে):

## কেন নির্বাচন করেছি
1.
2.
3.

## Requirement summary
- Core problem:
- Intended user:
- Must-have:
- MVP:

## Team fit
- Critical responsibility:
- Owner:
- Backup:
- Skill gap ও plan:

## Data/resources
- Primary source:
- Access test:
- Licence/citation note:

## Feasibility
- Success criteria:
1.
2.
3.

- Main risks:
- Fallback:

## Scorecard
- Weighted total:
- Hard gates:
- Unknown:

## বিবেচিত কিন্তু নির্বাচিত নয়
- Challenge:
- কারণ:

## Revisit condition
কোন নতুন তথ্য এলে decision আবার খুলব?
```

## ১৮. উদাহরণ: scorecard কীভাবে পূরণ করবেন

নিচের উদাহরণগুলো **সম্পূর্ণ কাল্পনিক ও পদ্ধতি দেখানোর জন্য**। এগুলো কোনো NASA challenge-এর official assessment, factual technical claim বা recommendation নয়।

ধরা যাক, একটি team দুইটি candidate challenge তুলনা করছে:

- **Candidate A:** একটি data-driven map/dashboard তৈরি করতে হবে;
- **Candidate B:** একটি interactive learning game বা story তৈরি করতে হবে।

| বিষয় | Weight | A score | A points | B score | B points |
|---|---:|---:|---:|---:|---:|
| Problem বোঝা | ২০ | ৪ | ১৬ | ৪ | ১৬ |
| Scope বাস্তবসম্মত | ২০ | ৩ | ১২ | ৫ | ২০ |
| Data/resource readiness | ১৫ | ২ | ৬ | ৪ | ১২ |
| Skill ও আগ্রহ fit | ১৫ | ৪ | ১২ | ৩ | ৯ |
| Testability/evidence | ১০ | ৩ | ৬ | ৩ | ৬ |
| User value | ১০ | ৪ | ৮ | ৪ | ৮ |
| Licence/safety/policy | ৫ | ৩ | ৩ | ৪ | ৪ |
| Demo clarity | ৫ | ৪ | ৪ | ৪ | ৪ |
| **মোট** | **১০০** | | **৬৭/১০০** | | **৭৯/১০০** |

এই কাল্পনিক স্কোরে B এগিয়ে, কিন্তু A-এর Data/resource score ২ হওয়ার কারণ তদন্ত না করে সিদ্ধান্ত নেওয়া ঠিক নয়। যদি A-এর central data event-এর মধ্যে পাওয়া না যায় এবং valid fallback না থাকে, hard gate-এ সেটি আটকে যেতে পারে। আবার team যদি B-এর Must-have game requirement পূরণ করতে না পারে, B-এর উচ্চ score-ও যথেষ্ট নয়। Evidence, scope ও hard gate-ই final discussion-এর ভিত্তি।

## ১৯. Final selection checklist

### Official understanding

- [ ] Full Challenge Statement পড়েছি, শুধু summary নয়।
- [ ] Official must-have ও expected outcome লিখেছি।
- [ ] Challenge-specific resource ও published guide দেখেছি।
- [ ] বর্তমান বছরের কাজ শুরুর/eligibility/submission rules যাচাই করেছি।

### Feasibility

- [ ] User ও problem team বোঝে।
- [ ] একটি ছোট MVP event window-তে শেষ করা যাবে।
- [ ] Central data/resource-এর access test করেছি বা credible fallback আছে।
- [ ] Rights/licence/safety/privacy প্রশ্নগুলোর গ্রহণযোগ্য পথ আছে।
- [ ] Output-এর অন্তত একটি গুরুত্বপূর্ণ অংশ পরীক্ষা করা যাবে।

### Team fit

- [ ] সদস্যদের আগ্রহ ও skill inventory নিয়েছি।
- [ ] Critical task-এর owner ও backup আছে।
- [ ] Team জানে কোন skill gap শিখবে বা কীভাবে সামলাবে।
- [ ] সবাই নির্বাচিত challenge-এর scope ও ঝুঁকি বোঝে।

### Decision quality

- [ ] Score-এর পাশে evidence/কারণ লিখেছি।
- [ ] Unknown-কে লুকিয়ে score দিইনি।
- [ ] Hard blocker-কে মোট score দিয়ে পাশ করাইনি।
- [ ] অন্তত একটি বিকল্প challenge বিবেচনা করেছি।
- [ ] সিদ্ধান্ত, rationale ও revisit condition লিখে রেখেছি।

## ২০. Official references

Challenge বাছাইয়ের আগে আপনার অংশগ্রহণের বছরের official page-এ গিয়ে current link অনুসরণ করুন:

- [NASA Space Apps Challenge](https://www.spaceappschallenge.org/)
- [Participant FAQs](https://www.spaceappschallenge.org/resources/participant-faqs/)
- [NASA Space Apps Resources](https://www.spaceappschallenge.org/resources/)
- [Participant Terms and Conditions](https://www.spaceappschallenge.org/legal/)
- [Contact NASA Space Apps](https://www.spaceappschallenge.org/contact-space-apps/)

২০২৬ সালের challenge-গুলো দেখতে: [2026 Challenge Statements](https://www.spaceappschallenge.org/2026/challenges/). এটি কেবল ২০২৬-এর list; পরবর্তী বছরের challenge list হিসেবে ব্যবহার করবেন না।

## ২১. এক বাক্যে challenge selection

> **যে challenge-এর full requirement team বোঝে, যার data ও rights-এর বাস্তবসম্মত পথ আছে, যার ছোট MVP event window-তে বানানো ও পরীক্ষা করা যায়, এবং যার কাজ team আগ্রহ নিয়ে ভাগ করে নিতে পারে—সেটিই শক্তিশালী candidate।**
