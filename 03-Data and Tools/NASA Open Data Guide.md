# NASA Open Data Guide

## NASA-র data খোঁজা, বোঝা, ব্যবহার ও citation করার বাংলা পরিচিতি

> **এই guide একটি ব্যবহারিক পরিচিতি; NASA-র official policy বা কোনো dataset-এর documentation-এর বিকল্প নয়।** NASA-র data portal, dataset, API, licence, access condition ও citation format একরকম নয়। যে নির্দিষ্ট dataset ব্যবহার করবেন, তার official landing page, metadata, user guide, licence/terms এবং citation নির্দেশনা পড়ুন।
>
> **NASA Space Apps-এর জন্য:** অংশগ্রহণের বছরের Participant Terms and Conditions, Challenge Statement ও Project Submission Guide অনুসরণ করুন। ২০২৬ সালের NASA Space Apps Terms-এ ব্যবহৃত প্রত্যেকটি source cite করতে, প্রযোজ্য third-party licence নথিভুক্ত করতে এবং original content প্রকাশ/লাইসেন্সের শর্ত মানতে বলা হয়েছে। এগুলো ২০২৬-এর যাচাইকৃত শর্ত; ভবিষ্যৎ বছরের terms আবার পড়ুন।

## ১. NASA Open Data বলতে কী বোঝায়?

NASA বিভিন্ন mission, satellite, instrument, research program ও engineering activity থেকে data প্রকাশ করে। “NASA open data” একটিমাত্র database বা একই format-এর dataset নয়। আলাদা archive বা service-এ থাকতে পারে:

- Earth observation: atmosphere, ocean, land, ice, climate, weather ও natural hazards;
- planetary science: Moon, Mars, asteroid, comet ও অন্যান্য planetary body;
- heliophysics: Sun, solar wind, magnetosphere ও space weather;
- astronomy ও astrophysics: telescope observation, catalog ও mission data;
- aerospace, engineering, laboratory ও technical report;
- API, map layer, image, audio, video এবং software/code।

একটি portal অনেক সময় dataset **খুঁজে দেয়**, কিন্তু data file নিজে host করে না। Download, visualization বা analysis-এর জন্য linked archive, API অথবা tool-এ যেতে হতে পারে।

## ২. কোন portal বা tool কোথায় কাজে লাগে?

| Portal/tool | সাধারণত কী খুঁজবেন বা করবেন | মনে রাখুন |
|---|---|---|
| [Data.nasa.gov](https://data.nasa.gov/) | NASA-সম্পর্কিত public dataset-এর catalogue/metadata খোঁজা | Dataset-এর metadata ও access link দেয়; underlying files অনেক সময় অন্য NASA archive-এ থাকে। |
| [NASA Earthdata](https://www.earthdata.nasa.gov/) | Earth observation data, tutorial, archive ও tool | Earth science-এর data-র জন্য প্রধান প্রবেশপথ। |
| [Earthdata Search](https://search.earthdata.nasa.gov/) | Earth science collection/granule স্থান, সময় ও metadata দিয়ে খোঁজা | কিছু data download/tool-এর জন্য Earthdata Login বা EULA প্রয়োজন হতে পারে। |
| [NASA Worldview](https://worldview.earthdata.nasa.gov/) | Satellite imagery layer map-এ browse, compare ও snapshot/underlying data খোঁজা | Map view দ্রুত exploration-এ উপকারী; screenshot নিজে raw dataset নয়। |
| [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/) | MODIS/VIIRS active fire ও thermal anomaly data, map, download/service | Near-real-time detection-কে সবসময় ground-confirmed fire ধরে নেওয়া যাবে না; product metadata দেখুন। |
| [NASA APIs](https://api.nasa.gov/) | NASA API catalogue, API key/access documentation | প্রতিটি endpoint-এর documentation, authentication ও rate limit যাচাই করুন; key-কে secret হিসেবে রাখুন। |
| [NASA Planetary Data System (PDS)](https://pds.nasa.gov/) | NASA planetary mission-এর archive করা data product | PDS catalog, instrument/product documentation ও data format বুঝে নিন। |
| [NASA Image and Video Library](https://images.nasa.gov/) | NASA image, video ও audio asset খোঁজা | Asset-এর item page, credit/usage note, third-party rights ও identifiable-person caveat দেখুন। |
| [NASA Technical Reports Server (NTRS)](https://ntrs.nasa.gov/) | NASA technical report, paper ও technical publication খোঁজা | Report-এর citation ও reuse terms আলাদাভাবে দেখুন। |
| [NASA Open Source Code](https://code.nasa.gov/) | NASA-র open-source software project খোঁজা | Repository-এর নির্দিষ্ট licence, dependency ও attribution পড়ুন। |

Portal-এর address বা feature সময়ের সঙ্গে বদলাতে পারে। Search engine-এর snippet নয়, provider-এর বর্তমান official page-কে source of truth ধরুন।

## ৩. Search শুরু করার কৌশল

### ধাপ ১: প্রশ্নকে data requirement-এ রূপ দিন

“জলবায়ু data চাই” খুব বড় প্রশ্ন। আগে ঠিক করুন:

- **বিষয়:** তাপমাত্রা, বৃষ্টি, আগুন, vegetation, ocean colour, air quality, ice, soil moisture?
- **স্থান:** বিশ্ব, দেশ, watershed, city, নির্দিষ্ট coordinate/bounding box?
- **সময়:** কোন তারিখ, ঋতু, বছর বা দীর্ঘমেয়াদি trend?
- **সময়-ব্যবধান:** প্রতি ঘণ্টা, দৈনিক, মাসিক, বার্ষিক?
- **মাপ:** কোন variable ও unit দরকার?
- **ব্যবহার:** map, time-series, comparison, alert, model, lesson বা story?
- **যে পরিমাণ precision দরকার:** approximate pattern, না নির্দিষ্ট pixel/point?

### ধাপ ২: সঠিক portal বেছে নিন

- পৃথিবীর satellite measurement হলে Earthdata Search বা সংশ্লিষ্ট NASA Earth science archive দিয়ে শুরু করুন।
- Map-এ layer দেখে কোন observation আছে বুঝতে Worldview উপকারী হতে পারে।
- Active fire-এর near-real-time detection চাইলে FIRMS documentation দেখুন।
- Planetary mission-এর instrument product চাইলে PDS catalog দেখুন।
- নির্দিষ্ট endpoint/data service লাগলে NASA API catalogue ও endpoint documentation দেখুন।
- NASA-র media asset চাইলে NASA Image and Video Library item page পরীক্ষা করুন।

### ধাপ ৩: Search-এ বৈজ্ঞানিক শব্দ ব্যবহার করুন

যতটা সম্ভব variable, instrument, platform/mission, location, temporal range ও product type যোগ করুন। উদাহরণ:

```text
variable + location + time range + platform/instrument + product
```

উদাহরণস্বরূপ, “forest data” না লিখে “forest canopy height”, নির্দিষ্ট region/time range এবং lidar/GEDI-সম্পর্কিত collection খোঁজা অধিক কার্যকর হতে পারে। এটি শুধু search pattern-এর উদাহরণ—নির্দিষ্ট collection বেছে নেওয়ার আগে official metadata পড়ুন।

### ধাপ ৪: Collection ও file আলাদা করে বুঝুন

- **Collection/dataset:** একই ধরনের data product-এর সংগৃহীত series; version, সময়কাল ও processing level থাকতে পারে।
- **Granule/file/item:** collection-এর একক data item বা file; একটি নির্দিষ্ট স্থান/সময়/segment কভার করতে পারে।
- **Metadata:** data কে তৈরি করেছে, কী মাপা হয়েছে, কোথায়/কখন, কীভাবে process হয়েছে ও কীভাবে ব্যবহার করতে হবে—তার বর্ণনা।
- **Browse image/preview:** data-র preview; সবসময় scientific analysis-এর উপযোগী মূল data নয়।

## ৪. Dataset ব্যবহার করার আগে metadata পড়ুন

শুধু title বা colourful map দেখে dataset বেছে নেবেন না। Dataset landing page, metadata, user guide ও version note থেকে যাচাই করুন:

| Metadata বিষয় | কী বুঝবেন |
|---|---|
| Provider/mission/instrument | কে data তৈরি বা archive করেছে? কোন platform/instrument? |
| Variable/measurement | সরাসরি কী মাপা হয়েছে, আর কোনটি derived estimate? |
| Spatial coverage | পুরো পৃথিবী, নির্দিষ্ট অঞ্চল, track, point, tile বা grid? |
| Temporal coverage | কোন তারিখ থেকে কোন তারিখ? Observation frequency কত? |
| Spatial resolution | একটি grid cell/pixel/footprint আনুমানিক কত এলাকা বোঝায়? |
| Temporal resolution | একটি record কত সময়ের observation বা average? |
| Units | K, °C, mm/day, m/s, W/m², index—কোন একক? |
| Coordinate reference/projection | Latitude/longitude নাকি অন্য CRS? Axis order কী? |
| Processing level | Raw/near-raw, calibrated, geophysical, gridded বা composite product? |
| Product version | Version বদলালে ফল বদলেছে কি? কোন version ব্যবহার করছেন? |
| Quality flags | কোন measurement গ্রহণ/বাদ দিতে হবে? Cloud, retrieval quality বা uncertainty flag কী? |
| Missing values | Missing/invalid value কীভাবে encode করা? Zero কি আসল measurement? |
| Uncertainty/limitations | Measurement-এর error, confidence, known caveat কী? |
| Update/latency | Near-real-time, provisional না final/archived? কখন update হয়? |
| Licence/access | Login, EULA, attribution, redistribution বা other use terms আছে কি? |
| Citation | Provider কীভাবে collection, version, DOI ও access date cite করতে বলেছে? |

যে metadata আপনার project-এর জন্য দরকার কিন্তু পাওয়া যাচ্ছে না, সেটি assumption হিসেবে লিখুন এবং ফলাফলের সীমা স্পষ্ট করুন।

## ৫. Data format-এর প্রাথমিক ধারণা

| Format | সাধারণ ব্যবহার | সাধারণত কী দিয়ে পড়া হয় |
|---|---|---|
| CSV/TSV | টেবিল, sample, time series | spreadsheet, Python/R/JavaScript |
| JSON | API response, nested record, configuration | text editor, programming language |
| GeoJSON | geographic feature ও coordinate | GIS, map library, code |
| GeoTIFF | georeferenced raster/grid | GIS, raster library |
| NetCDF | multidimensional Earth science data ও coordinate/metadata | GIS, Python/R/scientific tools |
| HDF/HDF5 | instrument/product-ভিত্তিক structured data | domain tool, Python/R library |
| CDF | কিছু space physics/heliophysics data product | mission-specific tool/library |
| FITS | astronomy image/table/spectral product | astronomy tool/library |
| KML/SHP | map feature, point, line, polygon | GIS/map tool |
| MP4/MP3/WAV/JPEG/PNG | media, presentation বা browse asset | media/image tools |

Format-এর নাম জানলেই data-এর অর্থ বোঝা যায় না। File-এর সঙ্গে দেওয়া schema, label, units, coordinate, metadata ও documentation-ও পড়ুন। File extension বদলে দিলে format convert হয় না।

## ৬. NASA data account, API key ও access

### Earthdata Login

NASA Earthdata-এর official guidance অনুযায়ী, data holdings উন্মুক্ত হলেও কিছু Earth science data download বা tool-এর পূর্ণ কার্যকারিতার জন্য Earthdata Login প্রয়োজন হতে পারে। কিছু collection-এর জন্য account profile-এ End User License Agreement (EULA) গ্রহণের প্রয়োজন হতে পারে। যেই collection ব্যবহার করবেন, তার access instructions যাচাই করুন।

### NASA API key

NASA API-র প্রতিটি endpoint-এর access, key requirement, rate limit ও response schema এক নয়। API ব্যবহার করার আগে:

1. endpoint-এর official documentation পড়ুন;
2. authentication ও rate limit যাচাই করুন;
3. API key code, public repository, screenshot বা project submission-এ প্রকাশ করবেন না;
4. key-কে environment variable বা local secret storage-এ রাখুন;
5. কেবল প্রয়োজনীয় sample request দিয়ে শুরু করুন;
6. API না চললে project-এর নিরাপদ fallback ঠিক করুন;
7. project-এর data endpoint ও access date নথিবদ্ধ করুন।

NASA API key ব্যবহার মানেই data licence, attribution বা rate-limit rule থেকে ছাড়—এমন নয়।

### Download ও storage

- প্রথমে ছোট region/time range বা sample file নিন।
- বড় dataset নামানোর আগে file size, storage, network ও processing requirement দেখুন।
- Public project-এ raw data copy রাখার দরকার আছে কি না যাচাই করুন; source link/collection identifier-ও যথেষ্ট হতে পারে।
- Dataset বা derived file-এ version ও processing note রাখুন।
- Data অসম্পূর্ণ download হলে file-কে valid ধরে analysis চালাবেন না।

## ৭. Data বুঝে নেওয়া ও quality-check

### ৭.১ প্রথমে ছোট sample পরীক্ষা

পুরো dataset process করার আগে:

1. File/response খোলে কি না দেখুন।
2. Column/variable name ও type নোট করুন।
3. Unit, time format ও coordinate range পরীক্ষা করুন।
4. কয়েকটি row/pixel/record হাতে দেখে expected pattern বুঝুন।
5. Missing value, duplicate, invalid flag ও outlier খুঁজুন।
6. Documentation-এর উদাহরণ বা published visualization-এর সঙ্গে sanity-check করুন।

### ৭.২ Common interpretation trap

- **Pixel size = ground truth নয়:** resolution যতই সূক্ষ্ম হোক, তা measurement uncertainty দূর করে না।
- **Satellite pixel = নির্দিষ্ট একক বস্তু নয়:** Pixel/footprint-এর ভেতরে বহু ধরনের ভূমি বা বস্তু মিশতে পারে।
- **Map colour = raw measurement নয়:** Visualization layer-এ scale, palette, composite বা processing applied থাকতে পারে।
- **Near-real-time = final নয়:** Provisional product পরে বদলাতে পারে; latency ও validation note দেখুন।
- **Cloud/quality flag উপেক্ষা নয়:** Bad/low-quality observation বাদ দিলে coverage কমে যেতে পারে, কিন্তু flag বাদ দিলে ভুল বাড়তে পারে।
- **Missing = zero নয়:** Missing code বা no-data value-কে আসল শূন্য ধরে নেবেন না।
- **Correlation = causation নয়:** দুই dataset-এ একসঙ্গে pattern মানেই একটির কারণে অন্যটি হয়েছে—এমন নয়।
- **Different instruments সরাসরি comparable নাও হতে পারে:** Time, calibration, resolution, unit, footprint ও processing আলাদা হতে পারে।
- **Map projection ভুল হতে পারে:** Coordinate order/CRS ভুল হলে feature ভুল স্থানে দেখা দিতে পারে।
- **Average মানে প্রতিটি স্থানের অবস্থা নয়:** Spatial/temporal aggregation detail মুছে দিতে পারে।

### ৭.৩ Derived calculation নথিবদ্ধ করুন

আপনি data filter, unit conversion, aggregation, normalization, interpolation, classification বা model ব্যবহার করলে লিখুন:

- input dataset/collection ও version;
- কোন record/সময়/স্থান বাদ বা রাখা হয়েছে;
- quality flag/missing value কীভাবে সামলানো হয়েছে;
- conversion বা formula;
- threshold/parameter;
- processing script/tool version;
- output-এর known limitation।

এতে অন্য কেউ আপনার ফল পুনরায় বুঝতে ও যাচাই করতে পারে।

## ৮. Data থেকে project বানানোর কার্যকর workflow

### ধাপ ১: User-এর প্রশ্ন নির্দিষ্ট করুন

উদাহরণ কাঠামো:

> “[ব্যবহারকারী] কোন স্থান/সময়/পরিস্থিতি সম্পর্কে কী জানতে বা সিদ্ধান্ত নিতে চান?”

### ধাপ ২: Data-তে সেই প্রশ্নের measurement আছে কি না যাচাই

Data-তে যা মাপা হয়েছে তা আর user যা জানতে চান—দুটির মধ্যে ব্যবধান আছে কি? Proxy variable হলে সেটিকে সরাসরি outcome হিসেবে উপস্থাপন করবেন না।

### ধাপ ৩: Sample access ও metadata check

একটি ছোট sample দিয়ে access, format, unit, projection, date range ও quality flag পরীক্ষা করুন।

### ধাপ ৪: Minimum processing path তৈরি

```text
Input data
  → quality/format check
  → প্রয়োজনীয় filter বা calculation
  → chart/map/table/output
  → user-এর প্রশ্নের উত্তর
```

### ধাপ ৫: Test ও limitation লিখুন

- একটি expected case;
- একটি edge case;
- data/measurement limitation;
- uncertainty বা assumption;
- user-কে ভুল ব্যাখ্যা থেকে রক্ষার label/note।

### ধাপ ৬: Source ও citation যোগ করুন

Source register event চলাকালেই পূরণ করুন; শেষে স্মৃতি থেকে বানাবেন না।

## ৯. Citation ও attribution

### ৯.১ Citation কেন দরকার?

Citation দিয়ে পাঠক জানতে পারেন:

- data/asset কে তৈরি বা প্রদান করেছে;
- কোন collection, product, instrument বা API ব্যবহার হয়েছে;
- কোন version/date range নেওয়া হয়েছে;
- data কোথায় খুঁজে পাওয়া যায়;
- আপনার ফল পুনরায় যাচাই করতে কী লাগবে।

### ৯.২ Citation-এর অগ্রাধিকার

1. Dataset landing page বা provider-এর recommended citation হুবহু অনুসরণ করুন।
2. DOI থাকলে DOI ও version ব্যবহার করুন।
3. API হলে endpoint/documentation, accessed date এবং প্রযোজ্য parameter/data product উল্লেখ করুন।
4. Media হলে item page-এ দেওয়া creator/credit/source ব্যবহার করুন।
5. Citation format না থাকলে নিচের template-কে পূরণ করে স্পষ্ট, পুনরুদ্ধারযোগ্য reference দিন।
6. আপনার বছরের Space Apps form-এ citation field থাকলে সব ব্যবহৃত source সেখানে দিন।

### ৯.৩ Citation template

```text
প্রদানকারী/সংস্থা. (বছর বা release date). Dataset/collection/product-এর নাম,
version (যদি থাকে), mission/instrument (প্রযোজ্য হলে), সময়কাল/স্থান।
Dataset landing page বা DOI/URL. Accessed: YYYY-MM-DD.
Licence/usage note: [যা provider উল্লেখ করেছে]
```

API-এর জন্য:

```text
NASA/API provider. Endpoint বা API/product-এর নাম. API documentation URL.
ব্যবহৃত query/parameter-এর সংক্ষিপ্ত বর্ণনা। Accessed: YYYY-MM-DD.
Data version/period (যদি থাকে). Licence/usage note: [provider নির্দেশনা]
```

Image/video/audio-এর জন্য:

```text
Creator/credit as listed by NASA. Asset title/ID. NASA Image and Video Library.
Asset page URL. Accessed: YYYY-MM-DD. Credit/rights note: [item page অনুযায়ী]
```

### ৯.৪ Source register

| ID | কী ব্যবহার | Provider/creator | Collection/asset/version | URL/DOI | Licence/terms | কীভাবে ব্যবহার | Citation ready? |
|---|---|---|---|---|---|---|---|
| 1 | | | | | | | |
| 2 | | | | | | | |
| 3 | | | | | | | |
| 4 | | | | | | | |

Code library, API, map tiles, font, icon, paper, model, audio, image ও synthetic/generated material-ও project-এ ব্যবহৃত হলে register-এ বিবেচনা করুন।

## ১০. Open data মানে কী—এবং কী নয়?

“Publicly accessible” বা “open data” দেখলেই সব asset-এর জন্য একই reuse permission আছে ধরে নেবেন না।

- Dataset page-এ থাকা licence, usage note, attribution ও access restriction পড়ুন।
- NASA web page-এ থাকা third-party content-এর অধিকার NASA-র page-এ দেখানো থাকলেও সেটি আপনার reuse right নিশ্চিত করে না।
- NASA-র logo/insignia, endorsement, identifiable person, contractor content ও third-party material-এর আলাদা নিয়ম থাকতে পারে।
- NASA content-এর general media guidance-ও সব image/asset-এর জন্য blanket permission নয়; individual credit/rights note দেখুন।
- NASA-র API/data access সম্ভব হলেও project-এর licence ও source citation obligation আলাদা থাকতে পারে।
- Challenge-এর Terms যদি অন্য source-এর জন্য আরও কঠোর শর্ত দেয়, সেটিই অনুসরণ করুন।

**২০২৬ Space Apps Terms-এ যাচাইকৃত:** সব ব্যবহৃত source cite করতে বলা হয়েছে। Terms-এ third-party material-এর public availability/licence যাচাই, প্রযোজ্য licence project documentation-এ শনাক্ত এবং প্রয়োজনীয় licence documentation জমা দেওয়ার শর্ত আছে। Terms-এ original project content-এর প্রকাশ/OSI-compliant open-source licensing এবং team নির্দিষ্ট OSI licence না দিলে Apache 2.0-এ বিতরণের কথাও আছে। ভবিষ্যৎ বছরের ক্ষেত্রে current Terms পড়ুন; এই paragraph-কে legal advice মনে করবেন না।

### NASA media-র জন্য অতিরিক্ত সতর্কতা

NASA-র Media Usage Guidelines অনুযায়ী NASA content সাধারণত educational/informational ব্যবহারে পাওয়া যেতে পারে, তবে:

- NASA insignia, logotype ও identifiers-এর ব্যবহার আলাদাভাবে সুরক্ষিত;
- NASA site-এ থাকা third-party copyright asset-এ NASA-র ব্যবহারের অনুমতি আপনার কাছে স্বয়ংক্রিয়ভাবে আসে না;
- identifiable মানুষের ছবি/নাম/কণ্ঠ ব্যবহারে privacy/publicity ও consent issue হতে পারে;
- NASA-র content দিয়ে commercial product বা service-এ NASA endorsement বোঝানো যাবে না;
- asset-এর page ও [NASA Media Usage Guidelines](https://www.nasa.gov/nasa-brand-center/images-and-media/) দুটোই দেখুন।

## ১১. Data quality ও project claim-এর সততা

Project-এর ভাষা data যা সমর্থন করে তার চেয়ে বড় দাবি করবে না।

### Claim check

- [ ] Claim কি data-র সরাসরি measurement, নাকি model/proxy/inference?
- [ ] সময় ও location project-এর প্রশ্নের সঙ্গে মেলে?
- [ ] Data quality/uncertainty-এর কোনো গুরুত্বপূর্ণ caveat বাদ পড়েছে?
- [ ] Visualization axis, colour scale, unit ও aggregation স্পষ্ট?
- [ ] কোনো sample বা synthetic data-কে real observation বলা হচ্ছে না?
- [ ] Algorithm-এর output-কে নিশ্চিত forecast/diagnosis/ground truth বলা হচ্ছে না?
- [ ] User ভুল ব্যাখ্যা করলে কীভাবে বুঝবেন—এমন explanation আছে?

যদি project output decision support দেয়, তা professional, medical, emergency বা legal advice নয়—এমন caveat প্রাসঙ্গিক হলে স্পষ্ট করুন।

## ১২. Common tool: কোন কাজের জন্য?

| কাজ | উদাহরণ tool/path | কী শিখতে হবে |
|---|---|---|
| Earth data খোঁজা | Earthdata Search | Collection, granule, filters, metadata |
| Satellite layer দ্রুত দেখা | Worldview | Layer, time, map display ও underlying product |
| Earth data analysis না করে browse | Giovanni | Selected variable, time/area aggregation ও output limitations |
| Data subsetting/sample extraction | AppEEARS বা provider tool | Sample request, projection, output format |
| Fire detection browse/download | FIRMS | Sensor/product, timestamp, confidence/quality, detection caveat |
| Planetary archive | PDS | Mission, instrument, product label, coordinate ও archive docs |
| API data | api.nasa.gov ও endpoint docs | Key/auth, request parameters, schema, rate limits |
| Map/geospatial analysis | GIS software বা code library | CRS, resolution, raster/vector, attribution |
| File exploration | Spreadsheet, notebook, command-line tool | Encoding, schema, units ও reproducibility |

Tool-এর নাম শেখার চেয়ে আপনার প্রশ্নের জন্য data সঠিক কি না বোঝা বেশি জরুরি।

## ১৩. Hackathon-এর জন্য দ্রুত data workflow

### প্রথম ৩০–৬০ মিনিটের data check

সময় project ও dataset অনুযায়ী বদলাতে পারে; এটি কেবল ছোট feasibility session-এর উদাহরণ।

1. Challenge statement-এর user question লিখুন।
2. Official portal থেকে ১–২টি সম্ভাব্য collection খুঁজুন।
3. Landing page, version, variable, time/location coverage, units ও licence পড়ুন।
4. ছোট sample বা একটি API response নিন।
5. Sample খুলে column/variable, missing value, coordinate ও date inspect করুন।
6. একটি map/chart/summary বানিয়ে metadata-এর সঙ্গে মিলিয়ে দেখুন।
7. Source register-এ URL, version ও access date লিখুন।
8. Data না পেলে fallback বা challenge scope update করুন।

### Data spike pass/fail note

```text
Dataset/API:
Official URL:
Question-এর সঙ্গে relevance:
Sample access: Pass / Fail / Unknown
Format:
Variable ও unit:
Spatial/time coverage:
Quality flag/missing value:
Licence/citation:
Main caveat:
Fallback:
Decision: Use / Test more / Replace
```

## ১৪. Common ভুল

| ভুল | ফল | প্রতিকার |
|---|---|---|
| Search result-এর snippet থেকে dataset বেছে নেওয়া | Version, unit বা limitation অজানা থাকে | Provider landing page ও metadata খুলুন |
| Preview image-কে analysis-ready data ভাবা | Processing/scale ভুল বোঝা | Underlying product ও product guide খুঁজুন |
| Map-এ দেখতে সুন্দর বলেই data গ্রহণ | User question-এর সঙ্গে data fit নাও হতে পারে | Variable, time, location ও resolution মিলান |
| API response-এর field name-কে অর্থ ধরে নেওয়া | Schema/unit interpretation ভুল | Endpoint documentation ও sample inspect |
| সব no-data-কে ০ করা | False signal/trend তৈরি | No-data encoding ও quality flags যাচাই |
| Celsius/Kelvin বা সময় zone না মিলিয়ে তুলনা | ভুল comparison | Unit ও timestamp normalize, method document |
| Different sensor series সরাসরি জোড়া | Instrument/method difference উপেক্ষা | Calibration, product version ও comparability পরীক্ষা |
| NASA website-এর সব image পুনর্ব্যবহারযোগ্য ভাবা | Third-party/likeness/logo issue | Asset-specific credit/rights ও Media Guidelines দেখুন |
| Source শেষ মুহূর্তে মনে করার চেষ্টা | Citation হারায় | কাজের সঙ্গে সঙ্গে source register পূরণ |
| API key public code-এ রাখা | Key misuse বা quota exhaustion | Secret storage; exposed key revoke/rotate |
| Dataset এত বড় download করা যে prototype আটকে যায় | সময়/storage নষ্ট | ছোট spatial/time subset দিয়ে শুরু |
| Data limitation project-এ না বলা | Output অতিরঞ্জিত/বিভ্রান্তিকর হয় | Limitation ও uncertainty UI/demo-তে দেখান |

## ১৫. Ready-to-copy data inventory

| প্রশ্ন | উত্তর |
|---|---|
| User-এর প্রশ্ন | |
| প্রয়োজনীয় variable | |
| স্থান ও coordinate system | |
| সময়কাল ও frequency | |
| সম্ভাব্য collection/API | |
| Provider/mission/instrument | |
| Version/processing level | |
| Format ও approximate size | |
| Unit ও quality flag | |
| Missing value handling | |
| Access/login/EULA/API key | |
| Licence/attribution | |
| Citation/DOI | |
| Known uncertainty/limitation | |
| Fallback data/tool | |

## ১৬. Ready-to-copy citation bibliography

```text
# Data and Resources

## Datasets
1. Provider:
   Dataset/collection:
   Version:
   DOI/URL:
   Time/area used:
   Access date:
   Licence/attribution:

## APIs and tools
1. Provider:
   API/endpoint/tool:
   Documentation:
   Parameters/product:
   Access date:
   Licence/terms:

## Code and software
1. Project/library:
   Version:
   Repository:
   Licence:
   Used for:

## Images, audio, video and other media
1. Creator/credit:
   Asset title/ID:
   Asset page:
   Rights/usage note:
   Used for:

## Publications and other references
1. Author/agency:
   Title:
   DOI/URL:
   Access date:
   Used for:
```

## ১৭. Official references

- [Data.nasa.gov — public NASA dataset catalogue](https://data.nasa.gov/)
- [NASA Earthdata](https://www.earthdata.nasa.gov/)
- [Earthdata Search](https://search.earthdata.nasa.gov/)
- [Earthdata Search user information](https://www.earthdata.nasa.gov/data/tools/earthdata-search)
- [NASA Worldview](https://worldview.earthdata.nasa.gov/)
- [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/)
- [NASA APIs](https://api.nasa.gov/)
- [NASA Planetary Data System](https://pds.nasa.gov/)
- [NASA Image and Video Library](https://images.nasa.gov/)
- [NASA Technical Reports Server](https://ntrs.nasa.gov/)
- [NASA Open Source Code](https://code.nasa.gov/)
- [NASA Media Usage Guidelines](https://www.nasa.gov/nasa-brand-center/images-and-media/)
- [NASA Space Apps Participant FAQs](https://www.spaceappschallenge.org/resources/participant-faqs/)
- [NASA Space Apps Participant Terms and Conditions](https://www.spaceappschallenge.org/legal/)

## ১৮. শেষ checklist

- [ ] Dataset-এর provider ও official landing page শনাক্ত।
- [ ] User-এর প্রশ্নের সঙ্গে variable, place ও time মেলে।
- [ ] Collection version, unit, resolution, quality flag ও limitations দেখা।
- [ ] ছোট sample/API response সফলভাবে inspect।
- [ ] Missing data, projection, time zone ও unit যাচাই।
- [ ] Licence, login/EULA, redistribution ও attribution note পড়া।
- [ ] NASA media, third-party asset, logo ও identifiable person-এর rights যাচাই।
- [ ] API key/credential public code বা submission-এ নেই।
- [ ] সব source কাজের সময়ই source register-এ লেখা।
- [ ] Current-year Space Apps Terms ও submission guide অনুসরণ।
- [ ] Project claim-এ data limitation ও uncertainty সৎভাবে দেখানো।

> **মনে রাখুন:** ভালো data workflow শুরু হয় একটি স্পষ্ট প্রশ্ন দিয়ে, তারপর metadata ও sample দিয়ে। “NASA data” বললেই সব dataset একই রকম, একই licence-এর, সহজে ব্যবহারযোগ্য বা আপনার দাবিকে সমর্থনকারী হয়ে যায় না।
