# Hackathon Weekend Planner
## NASA Space Apps Challenge-এর দুই দিনের কাজের সময়সূচি, milestone ও backup plan

> **এটি team-এর planning template—NASA-র official event schedule নয়।** আপনার Local Event বা Universal Event-এর start/end time, challenge-work window, submission deadline, timezone, breaks এবং current-year rules আগে যাচাই করুন। নিচের সময়গুলো নমুনা; event-এর official সময়ের সঙ্গে মিলিয়ে নিন। Event ৪৮ ঘণ্টার কম/বেশি হলে phase-গুলো অনুপাতে বদলান।
>
> **স্বাস্থ্য ও নিরাপত্তা:** রাত জেগে কাজ করা বাধ্যতামূলক নয়। খাবার, পানি, ঘুম, screen break ও accessibility need পরিকল্পনার অংশ। কোনো সদস্য অসুস্থ/ক্লান্ত হলে কাজ কমান, দায়িত্ব বদলান বা বিরতি নিন।

## ১. কীভাবে planner ব্যবহার করবেন

1. Official event start-কে **T0** এবং submission deadline-কে **D** হিসেবে লিখুন।
2. নিচের নমুনা slot-গুলো আপনার timezone ও event schedule-এ বসান।
3. প্রতিটি milestone-এর owner, backup এবং “complete” বলতে কী বোঝায়—লিখে রাখুন।
4. Deadline-এর আগে অন্তত একটি submission buffer রাখুন; upload/website সমস্যা হলে তার fallback ঠিক করুন।
5. কোনো task official rules-এর সঙ্গে সংঘর্ষে পড়লে নিয়ম মানুন—planner নয়।

### Team-এর event facts

```text
বছর:
Official event URL:
Event: Local / Universal / অন্য:
Timezone:
Official start (T0):
Official end:
Submission deadline (D):
Challenge:
Submission owner:
Independent checker:
Local Lead / official support:
Team communication channel:
Shared task board / files:
```

## ২. কাজের নিয়ম ও workload guardrail

- **একটি Must-have outcome:** event শেষ হওয়ার আগে কী demonstrably কাজ করবে তা এক বাক্যে লিখুন।
- **Scope freeze:** Day 2-এর নির্ধারিত সময়ের পর নতুন বড় feature নয়; bug fix, test, demo ও submission-এ মনোযোগ দিন।
- **একজন task owner, একজন backup:** প্রত্যেক critical task-এর দায়িত্ব স্পষ্ট রাখুন।
- **Integration শুরু থেকেই:** সব component শেষে জোড়া লাগানোর বদলে ছোট working version দ্রুত একত্র করুন।
- **যথেষ্ট বিরতি:** প্রায় ৬০–৯০ মিনিট মনোযোগী কাজের পর ৫–১৫ মিনিট screen/শরীরের বিরতি নিন; খাবারের জন্য আলাদা সময় রাখুন।
- **ঘুমের পরিকল্পনা:** event-এর official window এবং team-এর প্রয়োজন অনুযায়ী shift ভাগ করুন। কাউকে টানা কাজ করতে বাধ্য করবেন না।
- **Official source আগে:** pre-event challenge work, eligibility, AI/SI use, submission ও licensing-এর current rules মেনে চলুন।

## ৩. দুই দিনের নমুনা schedule

নিচের সময়গুলো একটি উদাহরণ মাত্র। `T0` থেকে নিজের timezone-এ বসান; event-এর প্রকৃত সময়ের বাইরে কোনো challenge work নির্ধারণ করবেন না।

### Day 1 — বোঝা, বেছে নেওয়া, ছোট working version

| নমুনা সময় | কাজ | Milestone / output | Owner |
|---|---|---|---|
| 09:00–09:30 | Kickoff; attendance, event facts ও communication check | সবাই deadline, timezone ও support contact জানে | Coordinator |
| 09:30–10:15 | Challenge Statement পড়া; problem, audience, required output চিহ্নিত | Challenge brief: problem, user, constraints | Research + team |
| 10:15–10:25 | বিরতি | পানি/চোখ/শরীরের বিরতি | সবাই |
| 10:25–11:00 | Challenge fit, data feasibility ও key risk তুলনা | Challenge selection ও unresolved question | Team |
| 11:00–11:15 | বিরতি | Screen থেকে দূরে | সবাই |
| 11:15–12:00 | User need, core use case ও success criteria ঠিক করা | এক বাক্যের solution + 2–3 measurable criteria | Product/research |
| 12:00–12:45 | Lunch ও বিশ্রাম | কাজে ফেরার আগে বিরতি | সবাই |
| 12:45–13:15 | MVP ও scope freeze; Must/Should/Could আলাদা করা | Must-have-এর তালিকা; বাদ দেওয়া scope | Coordinator + team |
| 13:15–14:15 | Data sample/API/tool access যাচাই; citation register শুরু | Data usable কি না; source, unit, coverage note | Data owner |
| 14:15–14:25 | বিরতি | পানি/চোখের বিশ্রাম | সবাই |
| 14:25–15:30 | Architecture/flow sketch; smallest end-to-end slice তৈরি | App/model/map-এর প্রথম connected skeleton | Tech owner |
| 15:30–15:45 | Snack/stretch break | কাজের চাপ কমানো | সবাই |
| 15:45–17:00 | প্রথম core feature implement ও integrate | **Milestone 1:** অন্য team member-এর device/environment-এ চালু হয় এমন working path | Feature owner + integrator |
| 17:00–17:15 | বিরতি | Screen থেকে দূরে | সবাই |
| 17:15–18:00 | Happy-path test, blocker review, backup সিদ্ধান্ত | **Milestone 2:** core flow-এর test result ও issue list | Tester |
| 18:00–19:00 | Dinner/দীর্ঘ বিশ্রাম | খাবার ও recovery | সবাই |
| 19:00–20:00 | Core flow উন্নত; visual polish সীমিত | Demo-তে দেখানোর মতো representative flow | Team |
| 20:00–20:15 | বিরতি | হাঁটা/চোখের বিশ্রাম | সবাই |
| 20:15–20:45 | Day 1 review; আগামী দিনের priority ও shift নিশ্চিত | Day 2 task board, owners ও backup | Coordinator |
| 20:45 থেকে | কাজ বন্ধ বা সম্মত shift; বিশ্রাম/ঘুম | হস্তান্তর note থাকলে লিখে রাখা | সবাই |

### Day 2 — শেষ করা, পরীক্ষা, demo ও জমা

| নমুনা সময় | কাজ | Milestone / output | Owner |
|---|---|---|---|
| 09:00–09:20 | Check-in; blocker, availability ও deadline পুনরায় নিশ্চিত | আজকের 3টি সর্বোচ্চ অগ্রাধিকার | Coordinator |
| 09:20–10:30 | Must-have feature finish; integration | **Milestone 3:** core user journey end-to-end complete | Feature owners |
| 10:30–10:40 | বিরতি | পানি/চোখ/শরীরের বিরতি | সবাই |
| 10:40–11:30 | Data, calculation, units, labels ও error handling যাচাই | Known issue ও limitation নথিবদ্ধ | Data owner + tester |
| 11:30–11:45 | বিরতি | Screen থেকে দূরে | সবাই |
| 11:45–12:30 | অন্য device/browser-এ demo path পরীক্ষা; fallback প্রস্তুত | **Milestone 4:** live path ও backup recording/screenshots | Demo owner |
| 12:30–13:15 | Lunch ও দীর্ঘ বিশ্রাম | খাবার/recovery | সবাই |
| 13:15–14:00 | Project description, README, source citation, licence ও AI disclosure review | Documentation draft ও source register | Writer + checker |
| 14:00–14:15 | বিরতি | Screen break | সবাই |
| 14:15–15:00 | Pitch/demo rehearsal; timing ও handoff practice | **Milestone 5:** rehearsed, timed demo | Presenter + team |
| 15:00–15:15 | Snack/stretch break | বিরতি | সবাই |
| 15:15–D−90 min | Final bug fixes only; scope freeze | Release candidate; no new major feature | Team |
| D−90 থেকে D−60 min | Independent review: challenge fit, facts, links, privacy, licence | Review checklist-এ blocker নেই বা documented | Independent checker |
| D−60 থেকে D−30 min | Official project page/form পূরণ, media/link upload | সব required field পূর্ণ; save/final review | Submission owner |
| D−30 থেকে D−15 min | Final submit; confirmation/status যাচাই | **Milestone 6:** final submission confirmation | Submission owner + checker |
| D−15 থেকে D | প্রয়োজন হলে official system-এ status recheck; নতুন risky change নয় | Deadline-এর আগে submitted status | Submission owner |
| Submission-এর পরে | Confirmation evidence সংরক্ষণ, team update, বিশ্রাম | Link/confirmation record | Coordinator |

> `D−90 min` বা অন্য deadline-relative সময়কে আপনার event-এর প্রকৃত submission deadline থেকে হিসাব করুন। Deadline যদি এই নমুনা schedule-এর আগে হয়, পুরো Day 2-কে আগেভাগে সরিয়ে নিন; শেষ মুহূর্তে upload ধরে রাখবেন না।

## ৪. Milestone gate: এগোনোর আগে কী যাচাই করবেন

| Gate | যাচাই | না হলে কী করবেন |
|---|---|---|
| **M0 — Rules ready** | Event, deadline, challenge, team eligibility ও submission path জানা | Official FAQ/Terms/Local Lead-এ প্রশ্ন পাঠান; অনিশ্চিত নিয়ম ধরে কাজ করবেন না |
| **M1 — Data feasible** | অন্তত একটি বাস্তব/অনুমোদিত data path কাজ করে, অথবা fallback data স্পষ্টভাবে label করা | Scope কমান; validated sample বা অন্য উপযুক্ত source পরীক্ষা করুন |
| **M2 — Core flow** | User input থেকে meaningful output পর্যন্ত একটি path চলে | Feature কমিয়ে সবচেয়ে ছোট demonstrable path রাখুন |
| **M3 — Integrated prototype** | Team-এর component একসঙ্গে চলে; critical dependency বোঝা | Integrator-কে এক জায়গায় focus দিন; parallel feature freeze করুন |
| **M4 — Evidence checked** | প্রধান result/claim source, unit ও limitation-সহ review হয়েছে | Claim সীমিত করুন বা যাচাই না হওয়া result বাদ দিন |
| **M5 — Demo ready** | Main demo এবং offline/recorded fallback আছে | Screenshot/video/fixture দিয়ে fallback বানান; live dependency ব্যাখ্যা করুন |
| **M6 — Submitted** | Official page-এ final status/confirmation দেখা গেছে | Owner ও checker একসঙ্গে official system পুনরায় দেখুন; support contact প্রস্তুত রাখুন |

## ৫. ছোট-team task board template

| Priority | Task | Owner | Backup | Done হলে কী দেখা যাবে | Estimate | Status |
|---|---|---|---|---|---|---|
| Must | [Core data/input path] | [নাম] | [নাম] | [যাচাইযোগ্য ফল] | [S/M/L] | [To do] |
| Must | [Main user flow] | [নাম] | [নাম] | [Demo-তে কাজ করে] | [S/M/L] | [To do] |
| Must | [Project submission page] | [নাম] | [নাম] | [Official confirmation] | [S/M/L] | [To do] |
| Should | [Visual polish/accessibility] | [নাম] | [নাম] | [নির্দিষ্ট criterion] | [S/M/L] | [To do] |
| Could | [ঐচ্ছিক feature] | [নাম] | [নাম] | [নির্দিষ্ট criterion] | [S/M/L] | [Not started] |

Task status: `To do / In progress / Blocked / Done`। Blocked হলে blocker, কে সাহায্য করবেন এবং পরবর্তী review time লিখুন।

## ৬. Backup plan: সমস্যা হলে কীভাবে বদলাবেন

| ঝুঁকি/সমস্যা | আগাম প্রস্তুতি | Trigger | Backup action | সিদ্ধান্তের owner |
|---|---|---|---|---|
| Primary data/API unavailable | ছোট sample/cache, provider documentation, source register | নির্ধারিত checkpoint-এ data পাওয়া যাচ্ছে না বা rate/access error | Offline sample/আগে download করা অনুমোদিত data দিয়ে core demo; synthetic/mock হলে স্পষ্ট label | Data owner |
| API key/service secret leak | Secret manager বা local environment; public repo-তে না রাখা | Key public log/repo/screenshot-এ দেখা যায় | Provider-এর নির্দেশনায় revoke/rotate; public artifact সরান; team-কে জানান | Security/config owner |
| Live demo বা internet ব্যর্থ | Local build, screenshot, short recording, static output | দুইবার retry-তেও demo চলে না/connection নেই | Offline fallback দেখান; কোন অংশ live নয় তা সৎভাবে বলুন | Demo owner |
| Feature সময়মতো শেষ নয় | Must/Should/Could scope ও feature cutoff | Day 2 core milestone miss | Feature বাদ/স্থগিত; working path ও limitation polish | Product owner |
| Member অনুপস্থিত/অসুস্থ | Critical task backup, handoff note, shared files | Owner নির্ধারিত সময়ে unavailable | Backup owner শুধু Must task নেন; scope কমান; rest/safety অগ্রাধিকার | Coordinator |
| Integration conflict বা code break | Frequent small integration, version control, known-good branch/build | Main path ভেঙে যায় বা merge blocker | শেষ known-good version ফিরিয়ে আনুন; নতুন feature freeze; smallest fix | Integrator |
| Deadline/timezone ভুল বোঝা | Event facts-এ timezone, calendar reminder, buffer | Team-এর সময়ের অমিল বা page update | Official source যাচাই; বর্তমান deadline ধরে submission আগে করুন | Submission owner |
| Submission portal ধীর/ত্রুটি | Text/media আগে প্রস্তুত, link permission check, early upload | Deadline কাছাকাছি অথচ confirmation নেই | Official portal refresh/try supported browser; error evidence রাখুন; official support-এ তৎক্ষণাৎ যোগাযোগ | Submission owner |
| Source/licence/AI disclosure অসম্পূর্ণ | Source register ও disclosure note শুরু থেকেই | Final review-এ unknown asset/AI use পাওয়া যায় | Asset বাদ/replace করুন অথবা terms যাচাই করে disclosure সম্পূর্ণ করুন | Checker |
| Scope creep/নতুন idea | Scope freeze time ও change rule | নতুন feature Must task সরিয়ে দিচ্ছে | Idea backlog-এ রাখুন; বর্তমান deliverable শেষ করুন | Coordinator |

### Submission fallback-এর সীমা

- Local copy বা screenshot official submission-এর বিকল্প নয়—শুধু demo fallback।
- Deadline পেরিয়ে গেলে late submission গ্রহণ হবে ধরে নেবেন না।
- Portal error হলে current official support/contact-এর নির্দেশনা নিন; confirmation ছাড়া “submitted” বলবেন না।
- Project page-এ private/permission-locked link থাকলে reviewer দেখতে নাও পারেন; access requirement পরীক্ষা করুন।

## ৭. সংক্ষিপ্ত handoff ও status format

### কাজ হস্তান্তর

```text
Task/component:
বর্তমান অবস্থা:
শেষ known-good commit/file:
চালানো/পরীক্ষা করার ধাপ:
অমীমাংসিত blocker:
পরবর্তী ছোট কাজ:
যে secret/data কখনো message-এ দেবেন না:
```

### Team status update

```text
Done:
Next:
Blocked:
Need from team:
পরবর্তী বিরতি/check-in:
```

## ৮. Weekend শেষে retrospective

Submission সম্পন্ন ও বিশ্রামের পরে ১০–১৫ মিনিটে লিখুন:

- কী ভালো কাজ করেছে?
- কোন assumption ভুল ছিল?
- কোন data/tool/dependency সবচেয়ে বেশি ঝুঁকি তৈরি করেছে?
- পরেরবার কোন কাজ আগে test করব?
- কোন source, licence, credit বা decision নথিভুক্ত করতে হবে?
- Team member-দের অবদান ও শেখা কীভাবে সংরক্ষণ করব?

## সম্পর্কিত বাংলা গাইড

- [NASA Space Apps FAQ Bangla](../01-Getting%20Started/NASA%20Space%20Apps%20FAQ%20Bangla.md)
- [NASA Space Apps Project Roadmap](./NASA%20Space%20Apps%20Project%20Roadmap.md)
- [Team Formation and Roles](./Team%20Formation%20and%20Roles.md)
- [Project Submission Checklist](../04-Build%20and%20Submit/Project%20Submission%20Checklist.md)
- [Project Pitch and Demo Guide](../04-Build%20and%20Submit/Project%20Pitch%20and%20Demo%20Guide.md)
- [Project README Template](../04-Build%20and%20Submit/Project%20README%20Template.md)
- [NASA Open Data Guide](../03-Data%20and%20Tools/NASA%20Open%20Data%20Guide.md)
- [Data Citation and Open Source Licensing](../03-Data%20and%20Tools/Data%20Citation%20and%20Open%20Source%20Licensing.md)
- [AI Tools Use and Disclosure](../03-Data%20and%20Tools/AI%20Tools%20Use%20and%20Disclosure.md)

