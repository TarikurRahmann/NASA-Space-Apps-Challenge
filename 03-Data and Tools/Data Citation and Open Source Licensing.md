# Data Citation and Open Source Licensing

## Dataset, code, image ও library-এর credit এবং licence নথিভুক্ত করার বাংলা গাইড

> **এটি সাধারণ শিক্ষামূলক গাইড—আইনি পরামর্শ নয়, NASA-র official policy নয়, এবং কোনো নির্দিষ্ট dataset বা asset-এর licence নির্ধারণ করে না।** প্রতিটি resource-এর নিজস্ব landing page, metadata, licence, terms, attribution এবং citation নির্দেশনা পড়ুন। সন্দেহ থাকলে asset ব্যবহার করবেন না, rightsholder-এর অনুমতি নিন, বা event-এর official contact-এ জিজ্ঞেস করুন।
>
> **২০২৬ Space Apps Terms-এর যাচাইকৃত শর্ত:** ২০২৬ সালের Participant Terms অনুযায়ী solution-এ ব্যবহৃত প্রত্যেকটি source cite করতে হয়—open-source বা বিনামূল্যের source-ও; third-party material-এর public availability/licence যাচাই এবং প্রযোজ্য licence project documentation-এ শনাক্ত করতে হয়। Terms আরও বলে, posted solution অন্যদের download/use-এর জন্য available হতে পারে; original content unrestrictedভাবে উপলভ্য অথবা OSI-compliant open-source licence-এ থাকতে হবে। Team নির্দিষ্ট OSI-compliant licence না দিলে NASA original content Apache 2.0 licence-এ distribute করবে—এ কথাও ২০২৬ Terms-এ আছে। এগুলো **২০২৬ সালের Terms-এর সারাংশ**; অন্য বছরের জন্য current Terms পড়ুন।

## ১. চারটি আলাদা ধারণা

| ধারণা | কী বোঝায় | উদাহরণ |
|---|---|---|
| **Citation** | কোন source, version বা asset থেকে তথ্য/উপাদান এসেছে—তার পুনরুদ্ধারযোগ্য reference | Dataset-এর title, DOI, provider, version, URL |
| **Attribution/credit** | Creator/provider-কে কীভাবে উল্লেখ করতে হবে | “Data provided by …” বা asset page-এর নির্দিষ্ট credit line |
| **Permission/licence** | কী করতে পারবেন—copy, modify, redistribute, publish, commercial use ইত্যাদি | Software licence, image permission, dataset terms |
| **Access** | Resource দেখা বা download করা যায় কি না | Public URL, account, API key, EULA |

একটি বিষয় অন্যটির বিকল্প নয়:

- Citation দিলেই কোনো copyrighted image ব্যবহারের permission পাওয়া যায় না।
- Public URL থাকলেই resource open-source হয় না।
- বিনামূল্যে download করা গেলেই reuse/redistribution অনুমোদিত হয় না।
- Open-source licence থাকলেও source/attribution notice বাদ দেওয়া যায়—এমন নয়।
- API key বা Earthdata Login থাকলেই licence obligation মুছে যায় না।

## ২. কোন resource-এর জন্য কী রেকর্ড করবেন?

| Resource | Citation/credit-এ খুঁজুন | Permission/licence-এ খুঁজুন |
|---|---|---|
| Dataset/data product | Provider, collection, product, DOI, version, date/area | Data use, redistribution, derivative, attribution, access/EULA |
| API/service | Provider, endpoint, API/product, documentation, accessed date | Key/rate limits, response data terms, caching, redistribution |
| Code/library | Project name, version, repository URL | Software licence, NOTICE/attribution, dependency terms |
| Image/video/audio | Creator, asset title/ID, item page, required credit | Copyright/usage note, third-party rights, person/likeness consent |
| Map tile/style/service | Tile/style provider, service URL, layer name | Attribution, display/caching/print rules, key use |
| Font/icon/illustration | Creator/library, asset name, source URL | Embedding, modification, redistribution, attribution |
| Paper/report/web source | Author/agency, title, year, DOI/URL | Copyright/reuse; quotation limits; linked asset rights |
| AI-generated content | Tool/provider, use description, relevant date/version | Tool terms, input rights, generated-output terms, third-party likeness |
| Team-created content | Creator/team, version or repository | Team ownership agreement and selected licence |

## ৩. Source register আগে থেকেই রাখুন

Hackathon-এর শেষ দিনে browser history থেকে source পুনর্গঠন করবেন না। Project-এ প্রথমবার কোনো data, code, image, model, font বা service যোগ করার সময় register-এ লিখুন।

### পূরণযোগ্য register

| ID | Resource | Provider/creator | Version/DOI/URL | Licence/terms | Required credit | Project-এ ব্যবহার |
|---|---|---|---|---|---|---|
| 1 | | | | | | |
| 2 | | | | | | |
| 3 | | | | | | |
| 4 | | | | | | |
| 5 | | | | | | |

### প্রতিটি entry-র জন্য record

- Official landing page বা canonical repository;
- Dataset/asset/library-এর সুনির্দিষ্ট নাম;
- Version, release date, commit hash বা collection identifier;
- DOI থাকলে DOI;
- Access date (বিশেষ করে API, changing page বা query result);
- Licence/terms-এর exact name এবং link;
- Provider-এর required attribution/citation;
- কোন file, screen, chart, code path বা feature-এ ব্যবহার;
- পরিবর্তন/processing/translation/cropping/derivative করা হয়েছে কি না;
- licence বা permission অনিশ্চিত হলে সেই প্রশ্ন ও owner।

## ৪. Dataset ও data product cite করা

### Citation-এর অগ্রাধিকার

1. Dataset landing page-এ দেওয়া recommended citation হুবহু অনুসরণ করুন।
2. DOI থাকলে DOI, collection/product name ও version উল্লেখ করুন।
3. Tool-generated README/citation file (যেমন AppEEARS request-এর citation অংশ) পরীক্ষা করুন।
4. DOI/citation না থাকলে provider, dataset name, version, date/area, URL ও access date দিন।
5. API/service-এর ক্ষেত্রে endpoint documentation ও ব্যবহৃত product/parameter উল্লেখ করুন।
6. Team-এর derived result হলে input data-এর citation-এর সঙ্গে processing method/code-ও নথিবদ্ধ করুন।

### সাধারণ dataset citation template

```text
Provider/agency. (Release year/date). Dataset/collection/product title,
version/product ID (যদি থাকে), mission/instrument (প্রযোজ্য হলে),
ব্যবহৃত সময়কাল ও স্থান। DOI বা official landing-page URL.
Accessed: YYYY-MM-DD. Licence/attribution: provider-এর নির্দেশনা অনুযায়ী।
```

### API/service citation template

```text
Provider. API/service ও endpoint-এর নাম. API documentation URL.
ব্যবহৃত product, query/parameter বা সময়সীমা (প্রাসঙ্গিক হলে).
Accessed: YYYY-MM-DD. Licence/usage note: provider-এর নির্দেশনা অনুযায়ী।
```

### Dataset processing note

শুধু source cite করাই যথেষ্ট নাও হতে পারে—ফল পুনরায় বোঝার জন্য আপনার processing-ও লিখুন:

```text
Input collection/version:
Download/query date:
Spatial/time subset:
Variable ও unit:
Quality/missing-value handling:
Filter/aggregation/conversion:
Script/tool/version:
Output file/figure:
Known limitation:
```

### Provider-specific নির্দেশনা

NASA Earthdata-এর নির্দিষ্ট collection, DOI বা product citation format থাকলে সেটি অনুসরণ করুন। NASA AppEEARS-এর official page বলছে, request-সংশ্লিষ্ট generated README-তে “Data Product Citations” এবং “Software Citation” section থাকতে পারে; দুটোই পরীক্ষা করুন। অন্য tool-এও generated citation বা README থাকলে সেটি সংরক্ষণ করুন।

## ৫. API, query ও derived output cite করা

API থেকে পাওয়া ফল পরিবর্তনশীল হতে পারে। তাই:

- API provider, endpoint ও documentation-এর URL রাখুন;
- response-এর accessed date/time লিখুন;
- সম্ভব হলে product ID, version, date range ও query parameter নথিবদ্ধ করুন;
- rate limit বা key কোনো citation/permission নয়—terms আলাদা করে পড়ুন;
- API response-এ অন্য agency-এর data থাকলে underlying provider-কে cite করুন;
- API output cache বা redistribute করা যায় কি না provider-এর terms দেখুন;
- API data থেকে নিজস্ব chart/model তৈরি করলে input source ও method দুটোই ব্যাখ্যা করুন।

## ৬. Code ও software library-এর licence

### ৬.১ Software licence সাধারণত কী নিয়ন্ত্রণ করে?

Software licence code copy, modify, distribute, incorporate বা derived work প্রকাশের শর্ত নির্ধারণ করতে পারে। Library যোগ করার আগে:

1. Repository-র `LICENSE` file বা official licence page খুলুন;
2. সঠিক version/tag/commit-এর licence মেলান;
3. `NOTICE`, `COPYING`, attribution বা patent notice প্রয়োজন কি না পড়ুন;
4. transitive dependency-সহ project-এর dependency list দেখুন;
5. licence-এর redistribution/notice/source-code obligation বুঝুন;
6. licence project-এর অন্য component-এর সঙ্গে সামঞ্জস্যপূর্ণ কি না যাচাই করুন;
7. project-এর মধ্যে required notice/attribution রাখুন।

একই package-এর code, documentation, dataset, logo ও hosted service আলাদা terms-এ থাকতে পারে। Repository-র একটি `LICENSE` সব content cover করে—এমন ধরে নেবেন না।

### ৬.২ পরিচিত software licence—খুব সংক্ষিপ্ত ধারণা

| Licence | সাধারণ বৈশিষ্ট্য | কী যাচাই করবেন |
|---|---|---|
| **MIT** | সাধারণত permissive; copyright ও licence notice রাখার শর্ত থাকে | Notice ও disclaimer সংরক্ষণ |
| **BSD-2-Clause / BSD-3-Clause** | permissive; BSD-3-এ endorsement restriction আছে | Notice, disclaimer ও endorsement language |
| **Apache-2.0** | permissive; patent grant ও NOTICE-related provision আছে | Licence text, NOTICE, modifications ও attribution |
| **GPL family** | copyleft; distribution-এর সময় source/reciprocal conditions প্রযোজ্য হতে পারে | নির্দিষ্ট GPL version, combination ও distribution obligations |
| **AGPL family** | network interaction-এও source-related obligations থাকতে পারে | Exact version এবং network-use conditions |
| **MPL-2.0** | file-level copyleft বৈশিষ্ট্য | Modified covered file ও distribution terms |
| **No licence / “all rights reserved”** | Public code দেখা গেলেও reuse permission স্বয়ংক্রিয় নয় | Owner-এর explicit permission ছাড়া ব্যবহার এড়িয়ে চলুন |

এগুলো আইনি ব্যাখ্যা নয়; licence-এর exact text পড়ুন। “Permissive” মানে attribution/notice বাদ দেওয়ার অনুমতি নয়।

### ৬.৩ নিজের code-এ licence যোগ করা

NASA Space Apps-এর current-year Terms আগে পড়ুন। সাধারণ open-source project-এ:

- Team-এর সব contributor-এর agreement/ownership পরিষ্কার করুন;
- project-এর জন্য উপযুক্ত OSI-approved software licence নির্বাচন করুন;
- `LICENSE` file-এ full text রাখুন;
- third-party code-এর original notices/NOTICE সংরক্ষণ করুন;
- `README`-তে third-party components ও project licence ব্যাখ্যা করুন;
- code-এর licence-কে data, media, model weight বা logo-র licence বলে উপস্থাপন করবেন না।

**২০২৬ Space Apps Terms:** ২০২৬ Terms অনুযায়ী posted solutions অন্যদের download/use-এর জন্য উপলভ্য হতে পারে; original content freely available without restriction অথবা OSI-compliant open-source licence-এ থাকতে হবে। Team নির্দিষ্ট OSI-compliant licence না দিলে NASA original content Apache 2.0-এ distribute করবে—এ কথাও Terms-এ আছে। এই শর্ত বুঝে, আপনার বছরের Terms-এ পুনরায় যাচাই করে, original content-এর licence নির্ধারণ করুন।

## ৭. Dataset ও content licence software licence থেকে আলাদা

একটি software licence dataset, image বা audio-তে স্বয়ংক্রিয়ভাবে প্রযোজ্য হয় না। Content/data-এর জন্য:

- provider-এর data terms/licence সুনির্দিষ্টভাবে খুঁজুন;
- attribution, redistribution, derivative work, commercial/non-commercial use ও share-alike শর্ত দেখুন;
- database rights বা jurisdiction-specific terms থাকতে পারে—provider-এর wording পড়ুন;
- “open data” label থাকলেও collection-specific EULA/terms দেখুন;
- no licence থাকলে অনুমতি আছে বলে ধরে নেবেন না;
- sensitive, personal, confidential বা export-controlled material project-এ দেবেন না।

Creative Commons licence কোনো text/image/media-র জন্য উপযুক্ত হতে পারে, কিন্তু code-এর জন্য সাধারণত software licence বেশি মানানসই। CC0, CC BY, CC BY-SA, CC BY-NC বা CC BY-ND একে অন্যের সমতুল্য নয়; attribution, commercial use, derivative ও share-alike শর্ত আলাদা। নির্দিষ্ট asset-এর licence page পড়ুন—শুধু “Creative Commons” লেখা যথেষ্ট নয়।

## ৮. NASA image, video, audio ও logo

NASA-র Media Usage Guidelines অনুযায়ী NASA content সাধারণত U.S.-এ copyright-এর আওতায় পড়ে না এবং educational/informational কাজে ব্যবহার করা যেতে পারে—তবে এটি সব asset-এর জন্য blanket permission নয়। NASA-র guidance-এ স্পষ্ট:

- NASA insignia, logotype ও identifiers-এর ব্যবহার আলাদাভাবে সুরক্ষিত;
- NASA site-এ third-party copyright asset থাকলে NASA-র permission অন্যদের ব্যবহারের অধিকার দেয় না;
- NASA content factualভাবে ব্যবহার করুন, NASA endorsement বোঝাবেন না;
- identifiable person-এর নাম/ছবি/কণ্ঠ ব্যবহারে privacy/publicity ও permission issue হতে পারে;
- commercial/promotional use-এর জন্য অতিরিক্ত শর্ত থাকতে পারে।

### Media ব্যবহার করার আগে

- [ ] NASA Image and Video Library-র asset/item page খুলেছি।
- [ ] Credit line, creator, asset ID ও rights note নথিবদ্ধ করেছি।
- [ ] Asset-এ third-party copyright mark/credit আছে কি না পরীক্ষা করেছি।
- [ ] Asset-এ identifiable person বা minor আছে কি না দেখেছি।
- [ ] NASA logo/insignia ব্যবহার এড়িয়ে চলেছি, যদি official permission/brand guidance না থাকে।
- [ ] Cropping, editing, montage বা derivative allowed কি না যাচাই করেছি।
- [ ] Project NASA-র official endorsement বলে ভুল বোঝায় না।

যে asset-এর rights অস্পষ্ট, সেটি বদলে rights পরিষ্কার এমন asset ব্যবহার করুন।

## ৯. Image, font, icon, map tile ও design asset

Project-এর interface বা presentation-এ অল্প মনে হলেও এসব asset-ও source/rights review-এ আনুন:

- basemap ও map tile;
- icon pack, emoji, illustration ও template;
- font ও webfont;
- stock photo, sound effect, music ও video clip;
- chart/map screenshot;
- external model, embedding বা pretrained weights;
- generated image বা voice;
- design-system component ও code snippet।

প্রতিটির জন্য record করুন: provider/creator, asset identifier, URL, licence version, required attribution, পরিবর্তন করা হয়েছে কি না এবং কোন screen/media-তে ব্যবহৃত।

## ১০. Attribution কীভাবে দেখাবেন?

Provider-এর exact attribution wording থাকলে সেটি ব্যবহার করুন। তা না থাকলে এমন credit দিন যাতে resource শনাক্ত করা যায়:

```text
Data: [provider], [dataset/collection], [version/date], [DOI/URL].
Map/base layer: [provider], [service/style], [attribution URL].
Image/audio: [creator/credit], [asset title/ID], [source URL].
Software: [library/project], [version], [licence], [repository URL].
```

Credit দেখানোর জায়গা:

- project page-এর References/Data Sources অংশ;
- README বা documentation;
- chart/map-এর caption/footnote;
- video description/end credits;
- submission-এর references/resources field;
- licence অনুযায়ী `LICENSE`, `NOTICE` বা attribution file।

একটি bibliography থাকলেও asset-এর পাশে ছোট credit দরকার হতে পারে; provider-এর নির্দেশনা দেখুন।

## ১১. Third-party licence compatibility ও team ownership

Team-এর project-এ অনেক source একত্র হলে:

- dependency tree ও included assets-এর licence আলাদা তালিকায় রাখুন;
- project licence কোনো dependency-এর শর্তের সঙ্গে বিরোধ করে কি না যাচাই করুন;
- GPL/AGPL/copyleft code ব্যবহার করলে integration/distribution effect বোঝার আগে copy করবেন না;
- image/data licence-কে code repository-এর `LICENSE`-এর নিচে ভুলভাবে ফেলবেন না;
- template, AI-generated content বা teammate-এর contribution-এর rights স্পষ্ট করুন;
- team member-এর আগে থেকে থাকা code/asset project-এ আনলে ownership/licence লিখিতভাবে ঠিক করুন;
- current Space Apps Terms-এ submission NASA-কে কী permission দেয় তা পুরোটা পড়ে বুঝুন।

জটিল licence conflict হলে legal expert বা rightsholder-এর সাহায্য নিন; hackathon deadline-এর চাপ দিয়ে অনুমান করবেন না।

## ১২. ২০২৬ Space Apps terms: ব্যবহারকারীর জন্য গুরুত্বপূর্ণ সতর্কতা

এই অংশটি **শুধু ২০২৬ Participant Terms-এর সারাংশ**:

1. সব ব্যবহৃত source cite করতে হবে, open-source ও freely available resource-সহ;
2. third-party material-এর public availability/licence যাচাই team-এর দায়িত্ব;
3. প্রযোজ্য licence project documentation-এ শনাক্ত করতে হবে;
4. original solution content posted হলে অন্যদের download/use-এর জন্য available হতে পারে;
5. original content unrestrictedভাবে available অথবা OSI-compliant open-source licence-এ থাকতে হবে;
6. Terms বলে, team নির্দিষ্ট OSI-compliant licence না দিলে NASA original content Apache 2.0-এ distribute করবে;
7. এমন content জমা দেওয়া যাবে না যার copyright/IP অধিকার team-এর নেই;
8. NASA site-এর third-party media-তে NASA-র নিজস্ব permission অন্যদের permission নয়।

পুরো Terms পড়ুন: [NASA Space Apps Participant Terms and Conditions](https://www.spaceappschallenge.org/legal/). **২০২৭ বা অন্য বছরের জন্য উপরোক্ত শর্তগুলো কপি করে প্রয়োগ করবেন না।** Current Terms বা official clarification ব্যবহার করুন।

## ১৩. Common licensing ও citation ভুল

| ভুল ধারণা | কেন ভুল/ঝুঁকিপূর্ণ | করণীয় |
|---|---|---|
| “Source cite করেছি, তাই ব্যবহার করতে পারি” | Citation permission দেয় না | Licence/permission আলাদা যাচাই |
| “NASA website-এ আছে, তাই সব public domain” | Third-party asset ও logo-র শর্ত আলাদা | Asset-specific rights note পড়ুন |
| “No-cost download, তাই commercial/reuse allowed” | Access আর reuse permission এক নয় | Terms ও redistribution শর্ত দেখুন |
| “MIT মানে credit দরকার নেই” | Notice সংরক্ষণের শর্ত থাকে | Licence notice/required attribution রাখুন |
| “সব Creative Commons একই” | BY/SA/NC/ND শর্ত আলাদা | Exact licence version পরীক্ষা |
| “GitHub-এ code আছে, licence নিশ্চয়ই open” | Licence না থাকলে reuse permission স্বয়ংক্রিয় নয় | Explicit licence না থাকলে ব্যবহার এড়িয়ে চলুন/অনুমতি নিন |
| “একটি LICENSE সব asset cover করে” | Dataset/media/font/library-এর terms আলাদা | Per-resource register রাখুন |
| “API key পেলেই data freely reusable” | Authentication access দেয়, rights নয় | Data/provider terms আলাদা পড়ুন |
| “AI citation সত্যি হবে” | Citation hallucinated হতে পারে | DOI/URL primary source-এ খুলে দেখুন |
| “NASA logo শুধু decoration” | NASA identifiers-এর আলাদা legal/brand restriction আছে | Official brand guidance না থাকলে ব্যবহার করবেন না |
| “Attribution দিলে NASA endorsement বোঝানো যায়” | Credit আর endorsement আলাদা | Endorsement implication এড়িয়ে factual credit দিন |

## ১৪. Copy-ready third-party asset inventory

| Resource ID | Type | Title/identifier | Creator/provider | URL/DOI | Version/date | Exact licence/terms | Required notice/credit | Modified? | Used in |
|---|---|---|---|---|---|---|---|---|---|
| | Dataset | | | | | | | | |
| | Code/library | | | | | | | | |
| | Image/video/audio | | | | | | | | |
| | Font/icon/map tile | | | | | | | | |
| | Paper/API/model | | | | | | | | |

## ১৫. Copy-ready `THIRD-PARTY-NOTICES.md` template

Project-এ বহু library বা asset থাকলে repository-তে আলাদা notice file রাখতে পারেন। এটি NASA-র বাধ্যতামূলক file নয়, যদি current submission guide তা না বলে।

```markdown
# Third-Party Notices

## Data
- Provider:
- Dataset/collection/version:
- DOI/URL:
- Licence/terms:
- Required attribution:
- Used for:

## Software
- Project/library + version:
- Repository:
- Licence:
- Required notice/changes:
- Used for:

## Media and design assets
- Creator/provider:
- Asset title/ID:
- Source URL:
- Licence/permission:
- Required credit:
- Modifications:

## Maps and services
- Provider/service/layer:
- URL:
- Attribution/usage terms:
- Used for:

## AI-generated content (if applicable)
- Tool/provider:
- Purpose:
- Current terms reviewed:
- Human review:
```

## ১৬. Copy-ready source register

```text
# Source and Licence Register

Project:
Team:
Challenge:
Review date:
Current-year Participant Terms URL:

## Data
1. Provider:
   Dataset/collection/version:
   DOI/URL:
   Date/area used:
   Citation:
   Licence/terms:

## Software/code
1. Package/repository:
   Version/commit:
   URL:
   Licence:
   Required notices:

## Media/design
1. Creator/asset ID:
   URL:
   Licence/permission:
   Required credit:
   Where used:

## Unresolved questions
- Resource:
- Question:
- Owner:
- Official contact/rightsholder response:
```

## ১৭. Final compliance checklist

### Citation

- [ ] Dataset, API, code/library, media, font, map tile ও paper—সব ব্যবহৃত source তালিকাভুক্ত।
- [ ] Provider-এর recommended citation/DOI/version ব্যবহার করেছি, যেখানে আছে।
- [ ] API/query ও access date record করেছি, যেখানে ফল পরিবর্তনশীল।
- [ ] Derived result-এর processing/method নথিবদ্ধ করেছি।
- [ ] Open-source বা free source বাদ পড়েনি।

### Rights ও licence

- [ ] প্রতিটি resource-এর exact licence বা usage terms পড়েছি।
- [ ] Access/login-কে permission বলে ভুল করিনি।
- [ ] Code, dataset, media ও model-এর licence আলাদা করে দেখেছি।
- [ ] Third-party notices, attribution ও modification notice রেখেছি।
- [ ] NASA logo/insignia বা third-party NASA-page media-র rights যাচাই।
- [ ] Team-এর সব original contribution-এর ownership/selected licence পরিষ্কার।
- [ ] Current Participant Terms-এর submission/publication effect বুঝেছি।

### Submission

- [ ] Current-year Project Submission Guide-এর exact reference field পূরণ।
- [ ] Citation/NOTICE file official form-এ প্রয়োজন হলে যুক্ত।
- [ ] Link, DOI ও source reference কাজ করছে।
- [ ] কোনো unlicensed/confidential/private content নেই।
- [ ] Unresolved rights question থাকলে resource বাদ/বদল করেছি বা official permission নিয়েছি।

## ১৮. Official references

- [NASA Space Apps Participant Terms and Conditions](https://www.spaceappschallenge.org/legal/)
- [NASA Space Apps Participant FAQs](https://www.spaceappschallenge.org/resources/participant-faqs/)
- [NASA Space Apps Resources](https://www.spaceappschallenge.org/resources/)
- [NASA Media Usage Guidelines](https://www.nasa.gov/nasa-brand-center/images-and-media/)
- [NASA Open Data Guide](./NASA%20Open%20Data%20Guide.md)
- [Open Source Initiative: Open Source Definition](https://opensource.org/osd)
- [Open Source Initiative: Approved Licenses](https://opensource.org/licenses)
- [NASA Earthdata Search](https://www.earthdata.nasa.gov/data/tools/earthdata-search)
- [NASA AppEEARS](https://www.earthdata.nasa.gov/data/tools/appeears)

> **শেষ কথা:** Source cite করুন, কিন্তু citation-কে permission ভাববেন না। Access, licence, attribution, ownership, privacy এবং current Space Apps Terms—প্রতিটি আলাদা করে যাচাই করুন। Rights পরিষ্কার নয় এমন resource ব্যবহার না করাই নিরাপদ।
