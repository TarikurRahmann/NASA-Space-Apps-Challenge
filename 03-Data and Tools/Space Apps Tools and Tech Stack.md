# Space Apps Tools and Tech Stack

## Mapping, data analysis, web app, visualization ও design-এর উপযোগী tool guide

> **এটি tool বাছাইয়ের ব্যবহারিক guide; NASA-র official বা বাধ্যতামূলক tech stack নয়।** NASA Space Apps-এ কোনো নির্দিষ্ট programming language, framework বা design tool ব্যবহার করতেই হবে—এমন সাধারণ নিয়ম এখানে ধরে নেওয়া হয়নি। Challenge Statement, current-year Participant Terms, Project Submission Guide, data provider-এর documentation এবং licence-ই চূড়ান্ত।
>
> Hackathon-এ নতুন framework শেখার চেয়ে team যা চালাতে পারে, সেটি দিয়ে একটি ছোট, পরীক্ষিত prototype বানানো সাধারণত বেশি বাস্তবসম্মত। NASA Earthdata tools ও external software-এর availability, access terms ও feature পরিবর্তিত হতে পারে; ব্যবহার করার আগে official documentation দেখুন।

## ১. এক নজরে: কোন কাজের জন্য কোন ধরনের tool?

| কাজ | সহজে শুরু | বেশি নিয়ন্ত্রণ/বড় project | কখন ব্যবহার করবেন |
|---|---|---|---|
| NASA Earth data খোঁজা | Earthdata Search, Worldview | Earthdata APIs, archive-specific tools | Earth observation collection খোঁজা/preview |
| ছোট geospatial sample নেওয়া | AppEEARS | Earthdata Search/API, GIS services | নির্দিষ্ট point/area, time ও layer subset দরকার |
| Planetary data খোঁজা | PDS catalog | PDS tools/API ও mission-specific software | Moon/Mars/planetary mission data |
| Fire data browse | NASA FIRMS map | FIRMS download/API/services | Active fire/thermal anomaly data |
| Table/time-series analysis | Spreadsheet, Giovanni | Python + Jupyter + pandas/xarray | CSV, API response, time series, calculations |
| Raster/vector GIS | QGIS | Python + GeoPandas/Rasterio, cloud GIS | Map, overlay, projection, raster/vector analysis |
| No/low-code interactive app | Streamlit, Observable | React + TypeScript | ছোট dashboard, interactive prototype |
| Web map | NASA Worldview/EGIS preview | Leaflet, MapLibre GL JS, OpenLayers | Browser-এ map layer/feature দেখানো |
| Scientific visualization | Giovanni, spreadsheet chart | Matplotlib, Plotly, Altair | Trend, comparison, uncertainty ও chart |
| UI/design | কাগজে sketch, Penpot | Figma বা web design system | User flow, interface prototype, collaboration |
| Code collaboration | GitHub web UI | Git + GitHub/GitLab | Version history, issue/task, team integration |
| Demo/storytelling | Slides, screenshot | Web demo/video/notebook | Project ব্যাখ্যা ও submission preparation |

এই table কেবল starting point। Challenge-এর required output ও team-এর skill অনুযায়ী tool বদলাতে পারে।

## ২. Tool stack বাছাইয়ের সাতটি নীতি

1. **Problem দিয়ে শুরু করুন:** প্রয়োজন না বুঝে map, AI, database বা framework বেছে নেবেন না।
2. **একটি core path রাখুন:** data থেকে user-visible result পর্যন্ত একটি সরল flow তৈরি করুন।
3. **আগে sample পরীক্ষা করুন:** পুরো data বা বড় library যোগ করার আগে ছোট sample খুলুন।
4. **পরিচিত tool-কে অগ্রাধিকার দিন:** event window-তে শেখা, install ও integration-এর ঝুঁকি কমান।
5. **Account/API dependency সীমিত করুন:** key, login, quota বা network failure-এর fallback রাখুন।
6. **Licence ও attribution লিখে রাখুন:** tool, library, asset ও dataset—সব source-এর শর্ত যাচাই করুন।
7. **Tool-এর output-কে scientific truth ভাববেন না:** metadata, units, quality flags ও limitations বুঝুন।

## ৩. NASA ও Earth-science data tools

### ৩.১ Data.nasa.gov

**কাজ:** NASA dataset-এর catalogue/metadata খোঁজা।

**যখন কাজে লাগবে:** dataset কী আছে, কে দিয়েছে, কোথায় পাওয়া যায়—এমন discovery দরকার হলে।

**মনে রাখুন:** Data.nasa.gov সাধারণত catalogue ও metadata দেয়; মূল data file অন্য NASA archive বা service-এ থাকতে পারে। Dataset page-এর access link অনুসরণ করুন।

### ৩.২ Earthdata Search

**কাজ:** NASA Earth observation collection ও data item/গ্রানুল খোঁজা, location/time/discipline/platform/format-এর মতো filter ব্যবহার।

**যখন কাজে লাগবে:**

- নির্দিষ্ট region বা সময়ের satellite data দরকার;
- collection metadata, product version বা coverage তুলনা করতে হবে;
- sample/granule বেছে download করতে চান।

**মনে রাখুন:** কিছু data download বা tool-এর পূর্ণ কার্যকারিতার জন্য Earthdata Login এবং কোনো কোনো collection-এর জন্য EULA acceptance লাগতে পারে। Login লাগছে বলে data non-public—এমন নয়; collection-এর নির্দিষ্ট access instruction পড়ুন।

### ৩.৩ Worldview

**কাজ:** Satellite imagery layer browse, compare, animate ও নির্বাচিত data/imagery সম্পর্কে দ্রুত ধারণা নেওয়া।

**যখন কাজে লাগবে:**

- কোনো natural event-এর সময়গত পরিবর্তন visualভাবে explore;
- কোন layer বা date range প্রাসঙ্গিক তা খুঁজে দেখা;
- presentation-এর আগে pattern সম্পর্কে প্রাথমিক ধারণা।

**সতর্কতা:** Worldview-এর rendered imagery বা screenshot-কে স্বয়ংক্রিয়ভাবে raw/analysis-ready data হিসেবে ব্যবহার করবেন না। ব্যবহৃত layer-এর product, date, processing, scale, legend ও underlying-data option যাচাই করুন।

### ৩.৪ Giovanni

**কাজ:** নির্বাচিত geophysical parameter-এর map, time-averaged map, comparison plot, vertical plot বা animation তৈরি করে Earth science data explore করা।

**যখন কাজে লাগবে:** browser-এ দ্রুত data trend বা spatial pattern দেখতে চান এবং local data processing ছাড়াই exploratory analysis করতে চান।

**সতর্কতা:** কোন dataset, variable, aggregation, time/area range ও output ব্যবহার হয়েছে তা নথিবদ্ধ করুন। Plot দেখা মানেই সব scientific caveat শেষ—এমন নয়।

### ৩.৫ AppEEARS

**কাজ:** নির্দিষ্ট geographic point/area, সময়কাল ও layer অনুযায়ী geospatial data subset/sample তৈরি।

**যখন কাজে লাগবে:** পুরো global product না নিয়ে নির্দিষ্ট অঞ্চল বা sample-এর data দরকার হলে।

**মনে রাখুন:** AppEEARS-এর output-এর সঙ্গে সংশ্লিষ্ট data product-এর citation এবং tool/software citation থাকতে পারে। Generated README ও data product citation অংশটি পরীক্ষা করুন।

### ৩.৬ Earthdata GIS / EGIS

**কাজ:** NASA Earth science-এর GIS-ready service, imagery/raster service ও GIS workflow।

**যখন কাজে লাগবে:** বড় raster file download ও local preprocessing কমাতে বা published GIS service দিয়ে analysis করতে।

**সতর্কতা:** service endpoint, layer metadata, access, attribution এবং GIS operation-এর output কীভাবে তৈরি—তা নথিবদ্ধ করুন।

### ৩.৭ NASA FIRMS

**কাজ:** MODIS/VIIRS-based active fire ও thermal anomaly data map-এ দেখা, download বা service ব্যবহার।

**যখন কাজে লাগবে:** fire/hotspot-related visualization বা exploratory analysis।

**সতর্কতা:** satellite detection মানেই নিশ্চিতভাবে ground-verified fire—এমন নয়। Sensor, timestamp, confidence/quality fields, spatial resolution, latency ও product documentation দেখুন।

### ৩.৮ Planetary Data System (PDS)

**কাজ:** NASA planetary mission-এর archive করা data product, catalog ও documentation খোঁজা।

**যখন কাজে লাগবে:** Moon, Mars, asteroid, comet বা planetary mission-এর instrument data দরকার।

**মনে রাখুন:** Product label, instrument, coordinate frame, calibration, unit ও mission-specific format-এর documentation গুরুত্বপূর্ণ। File খুলতে পারা মানেই data-র অর্থ জানা নয়।

### ৩.৯ NASA APIs

**কাজ:** বিভিন্ন NASA service/API থেকে structured response বা data নেওয়া।

**যখন কাজে লাগবে:** project-এর জন্য documented endpoint-এর data সরাসরি প্রয়োজন হলে।

**সতর্কতা:**

- প্রতিটি endpoint-এর API key, authentication, rate limit ও terms আলাদা হতে পারে;
- endpoint-এর official docs-ই schema ও parameter-এর source;
- key public repository, browser bundle, screenshot বা submission text-এ রাখবেন না;
- API unreachable হলে static sample বা recorded demo fallback রাখুন;
- API response-এ data version, units ও access date থাকলে সংরক্ষণ করুন।

### NASA data-tool quick selector

```text
“কী dataset আছে?”             → Data.nasa.gov / Earthdata Search / PDS
“Satellite image দ্রুত দেখতে” → Worldview
“Earth variable-এর plot চাই”  → Giovanni
“Point/area sample দরকার”     → AppEEARS
“GIS service দিয়ে কাজ”        → Earthdata GIS / EGIS
“Active fire detection”       → FIRMS
“NASA endpoint দরকার”         → NASA API catalogue + endpoint docs
```

## ৪. Data analysis ও notebook

### ৪.১ Spreadsheet

**উদাহরণ:** Excel, LibreOffice Calc, Google Sheets (প্রতিষ্ঠান/ব্যক্তিগত policy অনুযায়ী)।

**ভালো:** ছোট CSV/TSV, filter, sort, simple chart, column inspection।

**সীমা:** খুব বড় file, multidimensional raster, reproducible processing বা complex geospatial analysis-এর জন্য উপযুক্ত নাও হতে পারে।

### ৪.২ Python + Jupyter Notebook

**উপযোগী:** API call, CSV/JSON processing, reproducible calculation, chart ও small prototype।

সাধারণ library:

| Library | সাধারণ কাজ |
|---|---|
| `pandas` | table/CSV, filtering, grouping ও time-series |
| `numpy` | array ও numerical calculation |
| `xarray` | labeled multidimensional scientific data, যেমন NetCDF |
| `matplotlib` | static chart ও scientific plotting |
| `plotly` | interactive chart |
| `geopandas` | vector geospatial data ও spatial operation |
| `rasterio` | raster/geospatial raster file |
| `requests` | HTTP/API request |

**শুরুতে সব install করবেন না।** Data format ও task দেখে প্রয়োজনীয় package যোগ করুন; current version, dependency ও licence নথিবদ্ধ করুন।

### ৪.৩ R

**উপযোগী:** statistical analysis, time-series, scientific chart ও reproducible report—বিশেষ করে team আগে থেকে R জানলে।

সম্ভাব্য ecosystem: `tidyverse`, `sf`, `terra`, `stars`, `ggplot2`। নির্দিষ্ট package-এর licence, version ও format support যাচাই করুন।

### ৪.৪ Giovanni বা AppEEARS বনাম local code

| পরিস্থিতি | সম্ভাব্য পছন্দ |
|---|---|
| দ্রুত trend/area-average map বা plot দেখতে | Giovanni |
| নির্দিষ্ট point/area-এর analysis-ready sample নিতে | AppEEARS |
| নিজের method, data transformation ও test সম্পূর্ণ নিয়ন্ত্রণে রাখতে | Python/R notebook |
| বড় raster download এড়াতে, service-based workflow যথেষ্ট হলে | Earthdata GIS/EGIS service |
| Event demo-তে internet নির্ভরতা ঝুঁকি হলে | ছোট permitted sample/cached result + স্পষ্ট label |

এই tool-গুলো একে অন্যের পূর্ণ বিকল্প নয়; input collection ও output capability মেলান।

## ৫. Mapping ও geospatial tools

### ৫.১ QGIS

**ধরন:** Desktop GIS; raster/vector layer দেখা, style, reproject, query, overlay ও map layout।

**ভালো যখন:**

- code ছাড়াই spatial data inspect করতে হবে;
- CRS, raster/vector ও layer alignment যাচাই করতে হবে;
- demo-র জন্য map layout বা layer comparison দরকার।

**মনে রাখুন:** Coordinate Reference System (CRS), axis order, pixel resolution ও unit পরীক্ষা করুন। Export করা map-এ scale/legend/source দিন; map rendering-কে raw measurement বলে দেখাবেন না।

### ৫.২ Leaflet

**ধরন:** JavaScript library দিয়ে সহজ browser map।

**ভালো যখন:** ছোট web map-এ marker, GeoJSON, popup, layer control বা basic tile layer দরকার।

**সতর্কতা:** Base map/tile provider-এর attribution ও usage terms মেনে চলুন; private key-সহ tile service হলে secret handling ও provider rules যাচাই করুন।

### ৫.৩ MapLibre GL JS

**ধরন:** Vector/raster tile-ভিত্তিক interactive web map rendering।

**ভালো যখন:** styled vector map, interaction, zoom/feature layer দরকার এবং team JavaScript জানে।

**সতর্কতা:** MapLibre library নিজে map data বা tile permission দেয় না। Tile/style/data provider-এর terms ও attribution আলাদা।

### ৫.৪ OpenLayers

**ধরন:** Browser-এ geospatial mapping-এর বিস্তৃত JavaScript library।

**ভালো যখন:** বিভিন্ন OGC service, projection ও geospatial layer সমর্থন দরকার এবং team-এর কাছে mapping experience আছে।

### ৫.৫ Web map বাছাই

| প্রয়োজন | শুরু করার tool |
|---|---|
| দ্রুত map browse, আলাদা app না বানিয়ে | NASA Worldview |
| GIS analyst-এর desktop workflow | QGIS |
| simple points/GeoJSON web map | Leaflet |
| vector tile/style-centric web map | MapLibre GL JS |
| OGC/projection-rich custom map | OpenLayers |

**নতুনদের জন্য:** map library বেছে নেওয়ার আগে sample GeoJSON বা small raster map-এ দেখান। NASA Earthdata GIS service ব্যবহার করলে service-এর terms, layer attribution ও data lineage পড়ুন।

## ৬. Visualization ও chart

### সহজ chart

- Spreadsheet chart: ছোট table-এর দ্রুত trend/check;
- Matplotlib/ggplot2: static plot ও analysis report;
- Plotly/Altair: interactive chart ও linked filtering;
- Giovanni: selected Earth science parameter-এর দ্রুত exploratory plot।

### Chart review

- Chart title প্রশ্ন বা result বোঝায়?
- X/Y axis, unit, date range ও source আছে?
- Missing value বা gaps বোঝা যাচ্ছে?
- Zero থেকে axis শুরু না হলে তা বিভ্রান্ত করছে কি?
- Colour palette, scale, binning ও clipping effect ব্যাখ্যা করা?
- Uncertainty/error range থাকলে দেখানো?
- Aggregated data-কে individual point-এর result হিসেবে দেখানো হয়নি?
- Colourblind ব্যবহারকারীর জন্য label/shape/pattern আছে?

## ৭. Web app ও prototype

### ৭.১ No-code / low-code

#### Streamlit

Python-এ দ্রুত data dashboard, map/chart ও interaction prototype বানানোর জন্য উপযোগী—যদি team Python জানে।

**ভালো:** notebook analysis-কে ছোট interactive app-এ রূপান্তর; দ্রুত input/filter/result demo।

**সীমা:** deployment, secrets, file size, app sleep/quota এবং external hosting-এর terms যাচাই করতে হবে।

#### Observable

JavaScript-এ interactive visualization/notebook-style prototype; data storytelling ও chart experiment-এ উপকারী।

**সীমা:** hosting/account, public/private sharing ও external data access-এর শর্ত current service documentation থেকে দেখুন।

### ৭.২ Front-end web app

#### HTML/CSS/JavaScript

সাধারণ prototype-এর জন্য ছোট static page যথেষ্ট হতে পারে। Framework যোগ করার আগে plain web page দিয়ে core problem দেখানো যায় কি না ভাবুন।

#### React + TypeScript

**ভালো:** component-ভিত্তিক interactive app, বড় interface বা একাধিক team member-এর front-end কাজ।

**সতর্কতা:** project-এর জন্য framework প্রয়োজন কি না যাচাই করুন; অতিরিক্ত boilerplate ও integration risk hackathon-এ সময় নিতে পারে।

#### Backend/API

যদি server-side processing সত্যিই প্রয়োজন হয়, team-এর পরিচিত technology (যেমন Python/Flask/FastAPI বা Node.js) নিন। User-এর browser-এ secret রাখার জন্য backend ব্যবহার করলেও hosting, authentication, access control ও data handling বুঝতে হবে।

### ৭.৩ Prototype বনাম deployed product

- Local app, notebook, static site বা hosted app—সবই demo-র উপায় হতে পারে; কোনটি গ্রহণযোগ্য তা current submission guide নির্ধারণ করে।
- Public deployment করলে test credentials, private data ও API secret বাদ দিন।
- External hosting/API-এর uptime বা cost-কে guarantee ধরে নেবেন না।
- Demo-র copy বা screenshot থাকলে live product-এর বিকল্প হিসেবে সত্যভাবে label করুন।
- Data mock হলে interface-এ এবং pitch-এ স্পষ্ট লিখুন।

## ৮. UI/UX ও design tools

### শুরু করার সহজ পদ্ধতি

1. প্রথমে কাগজ/whiteboard-এ user flow আঁকুন।
2. ৩–৫টি screen-এর low-fidelity sketch করুন।
3. একজন teammate-কে prototype দেখে ব্যবহারকারীর কাজ করতে বলুন।
4. কোন label, control বা data view বিভ্রান্তিকর—নোট করুন।
5. তারপর প্রয়োজন হলে design tool বা coded UI-তে যান।

### Tool option

| Tool | কাজ | মনে রাখুন |
|---|---|---|
| কাগজ/whiteboard | দ্রুত flow ও layout | দ্রুত বদলানো যায়; final UI নয় |
| Figma | Collaborative interface/prototype design | Account, sharing permission ও current terms দেখুন |
| Penpot | Open-source design/prototyping workflow | Hosting/permissions ও specific licence দেখুন |
| Canva/slide tool | Pitch deck, poster, simple visual | Template, font ও image asset-এর licence/credit যাচাই |

### Accessibility minimum

- পর্যাপ্ত text/background contrast;
- map/chart-এ colour ছাড়াও label, symbol বা pattern;
- ছোট font এড়িয়ে চলা;
- keyboard দিয়ে মূল action করা যায় কি না পরীক্ষা;
- button/field-এর নাম পরিষ্কার;
- image-এর প্রয়োজনীয় alt text/caption;
- video-তে প্রযোজ্য হলে caption/transcript;
- chart data শুধু colour দিয়ে encoded হলে text/table alternative।

## ৯. Version control ও team collaboration

### Git/GitHub বা সমতুল্য

**ব্যবহার:** code change history, branch/merge, issue, README ও team contribution record।

**ব্যবহারিক নিয়ম:**

- ছোট, বর্ণনামূলক commit করুন;
- README-তে setup/run instructions রাখুন, যদি reviewer-এর দরকার হয়;
- `.env`, API key, password ও private data commit করবেন না;
- merge-এর আগে app/notebook run করে দেখুন;
- external contributor বা public repository হলে permission ও licence যাচাই করুন;
- বড় data file-কে repository-তে রাখার আগে size, access terms ও policy দেখুন।

### দলিল ও কাজ ভাগ

- Task board: GitHub Issues/Projects, Trello বা team-এর পরিচিত equivalent;
- Shared documentation: README, notes বা collaborative document;
- Source register: project-এর সঙ্গে একটি ছোট table;
- Decision record: scope, data choice, assumption ও fallback লিখে রাখা।

একই কাজে একাধিক tool ব্যবহার করে context ছড়িয়ে দেবেন না। একটি task list ও একটি project source-of-truth রাখুন।

## ১০. Stack বাছাইয়ের ready matrix

প্রতিটি option-কে ১–৫ score দিন; এটি NASA rubric নয়, team-এর সিদ্ধান্তে সহায়তা।

| মানদণ্ড | Option A | Option B | Option C |
|---|---:|---:|---:|
| Team আগে থেকে জানে | | | |
| Dataset/format-এর সঙ্গে compatible | | | |
| Event window-তে setup করা যাবে | | | |
| Internet/account dependency কম | | | |
| Demo/test করা সহজ | | | |
| Licence/attribution পরিষ্কার | | | |
| Fallback আছে | | | |

**Stack rule of thumb:** সবচেয়ে বেশি feature-এর tool নয়—যে tool দিয়ে সবচেয়ে দ্রুত, নির্ভরযোগ্যভাবে challenge-এর core user journey দেখানো যায় সেটি নিন।

## ১১. উদাহরণ stack

এগুলো কেবল উদাহরণ; কোনো project-এর জন্য একমাত্র সঠিক stack নয়।

### A. Beginner: map + simple interaction

```text
Data discovery: Earthdata Search / Worldview
Small sample: GeoJSON / CSV
Map: Leaflet
Interface: HTML + CSS + JavaScript
Version control: GitHub
```

### B. Data dashboard

```text
Data discovery: Earthdata Search / AppEEARS / Giovanni
Analysis: Python + Jupyter + pandas
Charts: Plotly বা Matplotlib
App: Streamlit
Documentation: README + source register
```

### C. Geospatial analysis

```text
Data discovery: Earthdata Search
Sample/subset: AppEEARS বা provider service
Desktop inspection: QGIS
Code processing: Python + GeoPandas/Rasterio (প্রয়োজনে)
Presentation: web map বা exported map layout
```

### D. Planetary-data storytelling

```text
Archive: PDS
Product documentation: mission/instrument user guide
Inspection: suitable PDS/mission tool or Python notebook
Visualization: Plotly/Matplotlib/QGIS (data type অনুযায়ী)
Story: simple web page, slide বা interactive visualization
```

### E. No-code/low-code visual story

```text
Data exploration: Worldview/Giovanni
Map image/layer: provider documentation অনুযায়ী
Design: slide/design tool
Interactive element: challenge-সমর্থিত, সহজ-to-test option
Citation: asset page + dataset landing page
```

**প্রতিটি stack-এর data, library, map tile ও media-র licence/citation আলাদাভাবে যাচাই করুন।**

## ১২. Setup ও integration checklist

- [ ] Team-এর সবার machine-এ প্রয়োজনীয় tool চালু।
- [ ] Input file/API sample-এ অন্তত একজন নয়, অন্য teammate-ও কাজ করতে পারেন।
- [ ] Coordinate system, unit, time zone ও data version team-এর সবার কাছে স্পষ্ট।
- [ ] Environment/dependency version নথিবদ্ধ।
- [ ] API key secret হিসেবে রাখা; public repository-তে নেই।
- [ ] Network/API ছাড়া demo-এর fallback আছে।
- [ ] Raw, processed ও generated files আলাদা/নামযুক্ত।
- [ ] Source register ও licence note project-এর সঙ্গে রাখা।
- [ ] Prototype-এর user journey end-to-end চলে।
- [ ] নতুন framework বা service যোগ করার আগে তার প্রয়োজন যাচাই।

## ১৩. Common pitfalls

| Pitfall | কেন ঘটে | কী করবেন |
|---|---|---|
| একসঙ্গে অনেক framework যোগ | tool শেখা project-এর লক্ষ্য হয়ে যায় | একটি ছোট stack বেছে core flow আগে বানান |
| Browser map tile-কে NASA data বলে উল্লেখ | Basemap provider ও scientific layer আলাদা | প্রতিটি layer-এর provider/citation আলাদা করুন |
| API key client-side code-এ | Browser source সবার জন্য দেখা যায় | Secret storage/backend বা key-free fallback |
| Earthdata login পরে করা | Download/API setup সময় নেয় | Dataset-এর access requirements আগে যাচাই |
| NetCDF/HDF খুলতে না পেরে data বদলানো | Format-specific metadata অচেনা | Documentation ও suitable viewer/library ব্যবহার |
| Map-এ layer ঠিক, কিন্তু CRS ভুল | projection/axis order অমিল | CRS, coordinate range ও sample point পরীক্ষা |
| Preview দেখে ফল claim | Preview processed/visual product হতে পারে | Underlying product/metadata দিয়ে claim যাচাই |
| Hosted app/API-এর ওপর পুরো demo নির্ভর | Network/quota/login সমস্যা | Offline/sample fallback ও rehearsal |
| License/source review শেষে করা | Asset/source-এর শর্ত ভুলে যায় | source register কাজের শুরু থেকেই পূরণ |
| Feature বেশি, tested path নেই | Integration/QA-র সময় থাকে না | MVP, test, demo-র জন্য সময় reserve |

## ১৪. Official documentation ও tool links

### NASA data ও tools

- [Data.nasa.gov](https://data.nasa.gov/)
- [NASA Earthdata](https://www.earthdata.nasa.gov/)
- [Earthdata Search](https://search.earthdata.nasa.gov/)
- [Earthdata Search tool overview](https://www.earthdata.nasa.gov/data/tools/earthdata-search)
- [NASA Worldview](https://www.earthdata.nasa.gov/data/tools/worldview)
- [NASA Giovanni](https://www.earthdata.nasa.gov/data/tools/giovanni)
- [NASA AppEEARS](https://www.earthdata.nasa.gov/data/tools/appeears)
- [NASA Earthdata GIS](https://www.earthdata.nasa.gov/data/tools/earthdata-gis)
- [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/)
- [NASA API catalogue](https://api.nasa.gov/)
- [NASA Planetary Data System](https://pds.nasa.gov/)
- [NASA Image and Video Library](https://images.nasa.gov/)
- [NASA Technical Reports Server](https://ntrs.nasa.gov/)
- [NASA Open Source Code](https://code.nasa.gov/)
- [NASA Media Usage Guidelines](https://www.nasa.gov/nasa-brand-center/images-and-media/)

### Software documentation

- [QGIS Documentation](https://docs.qgis.org/)
- [Python Documentation](https://docs.python.org/3/)
- [Project Jupyter](https://jupyter.org/)
- [pandas Documentation](https://pandas.pydata.org/docs/)
- [xarray Documentation](https://docs.xarray.dev/)
- [GeoPandas Documentation](https://geopandas.org/en/stable/)
- [Rasterio Documentation](https://rasterio.readthedocs.io/)
- [Leaflet Documentation](https://leafletjs.com/reference.html)
- [MapLibre GL JS Documentation](https://maplibre.org/maplibre-gl-js/docs/)
- [OpenLayers Documentation](https://openlayers.org/doc/)
- [Streamlit Documentation](https://docs.streamlit.io/)
- [React Documentation](https://react.dev/learn)
- [Figma Help Center](https://help.figma.com/)
- [Penpot Documentation](https://help.penpot.app/)
- [Git Documentation](https://git-scm.com/doc)

## ১৫. সম্পর্কিত গাইড

- [NASA Open Data Guide](./NASA%20Open%20Data%20Guide.md)
- [NASA Space Apps Project Roadmap](../02-Planning%20and%20Team/NASA%20Space%20Apps%20Project%20Roadmap.md)
- [Challenge Selection Guide](../02-Planning%20and%20Team/Challenge%20Selection%20Guide.md)
- [Project Submission Checklist](../04-Build%20and%20Submit/Project%20Submission%20Checklist.md)
- [Project Pitch and Demo Guide](../04-Build%20and%20Submit/Project%20Pitch%20and%20Demo%20Guide.md)
- [Team Formation and Roles](../02-Planning%20and%20Team/Team%20Formation%20and%20Roles.md)

> **শেষ কথা:** Challenge-এর প্রশ্ন থেকে শুরু করুন, data access ও metadata যাচাই করুন, team যে stack চালাতে পারে সেটি বেছে নিন, এবং ছোট end-to-end prototype আগে তৈরি করুন। Tool শুধু উপায়—challenge-এর সঠিক, স্বচ্ছ ও পরীক্ষা করা সমাধানই project-এর কেন্দ্র।
