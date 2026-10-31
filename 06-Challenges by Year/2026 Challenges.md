# NASA Space Apps Challenge 2026: প্রতিটি Challenge-এর বিস্তারিত বাংলা গাইড
> **নথির পরিধি:** NASA Space Apps Challenge-এর ২০২৬ challenge list-এ দেখানো ১৪টি challenge-এর বাংলা ব্যাখ্যা, সম্ভাব্য প্রকল্প-ধারণা, কাজের ধাপ, সতর্কতা এবং সাধারণ প্রস্তুতি।
>
> **উৎস ও সীমাবদ্ধতা:** Challenge-এর নাম ও মূল বক্তব্য অফিসিয়াল ২০২৬ তালিকার ভিত্তিতে লেখা। প্রস্তাবিত feature, workflow, উদাহরণ ও checklist সহায়ক সম্পাদকীয় পরামর্শ; এগুলো NASA-র বাধ্যতামূলক নিয়ম, সম্পূর্ণ resource তালিকা বা judging rubric নয়। পূর্ণ statement ও Resources tab দেখতে সংশ্লিষ্ট অফিসিয়াল পৃষ্ঠা দেখুন।

## ১. NASA Space Apps Challenge কী?

NASA Space Apps Challenge একটি বৈশ্বিক hackathon, যেখানে নানা পটভূমির মানুষ NASA ও অন্যান্য উন্মুক্ত বিজ্ঞান-তথ্য কাজে লাগিয়ে পৃথিবী, মহাকাশ, পরিবেশ, প্রযুক্তি, শিক্ষা ও মানবজীবন নিয়ে সমস্যা সমাধানের চেষ্টা করেন। প্রকল্প শুধু coding নয়: data analysis, map, game, story, animation, lesson, sonification, hardware concept ও design-ও হতে পারে।

২০২৬ সালের অফিসিয়াল challenge page-এ **১৪টি challenge** দেখানো হয়েছে। কোন challenge বেছে নেবেন তা আপনার আগ্রহ, দলের দক্ষতা, সময় এবং উপলভ্য official resource দেখে ঠিক করুন। কোনো challenge card-এর short summary পুরো technical brief নয়; প্রতিটি statement-এর Details/Resources অংশও পড়তে হবে।

### এই গাইড কীভাবে পড়বেন

প্রতিটি challenge-এ রয়েছে:

1. নামের সহজ বাংলা ভাবার্থ;
2. অফিসিয়াল brief-এর মূল সমস্যা/উদ্দেশ্য;
3. প্রকল্পে কী বানানো যেতে পারে;
4. কাজের সম্ভাব্য ধাপ;
5. পরীক্ষা ও উপস্থাপনার পরামর্শ;
6. বৈজ্ঞানিক, নিরাপত্তা বা ব্যবহারিক সীমাবদ্ধতা।

এখানে “সম্ভাব্য” শব্দটি গুরুত্বপূর্ণ: ধারণাগুলো প্রকল্প পরিকল্পনায় সহায়তা করে, কিন্তু অফিসিয়াল requirement-এর বদলি নয়।

---

# ২. দ্রুত সূচি

| ক্রম | Challenge | প্রধান ক্ষেত্র |
|---:|---|---|
| ১ | Abandoned but not Forgotten: Storytelling about NASA's Discarded Equipment on the Moon and Mars | চাঁদ/মঙ্গলে NASA hardware ও বিজ্ঞান-গল্প |
| ২ | Be An Earth System Trend Detective! | Earth science time-series ও trend analysis |
| ৩ | Build a Junior Astronaut Mission Trainer | শিশুদের lunar/Martian outpost simulation |
| ৪ | Create Health Monitoring Software for Astronauts on Space Missions | দীর্ঘ মহাকাশ-মিশনে স্বাস্থ্য পর্যবেক্ষণ |
| ৫ | Dancing with the SARs | NISAR radar data-তে পৃথিবীর পৃষ্ঠ পরিবর্তন |
| ৬ | Field Shift: Adapting Farms with NASA Data | crop rotation ও কৃষি-সিদ্ধান্ত সহায়তা |
| ৭ | Flame in Freefall: SI-Powered Fire Safety Insights from Microgravity Combustion Data | microgravity-তে আগুনের গবেষণা ও dashboard |
| ৮ | Harmonization of MODIS and VIIRS Hot Spots | active fire hotspot-এর দীর্ঘমেয়াদি সমন্বিত ক্যালেন্ডার |
| ৯ | Identify Earth Locations that Analog the Permanent Moon Base Locations and Mars | পৃথিবীর চাঁদ/মঙ্গল-সদৃশ স্থান |
| ১০ | Interplanetary Survival Guide: Martian Map | Marswalk-এর জন্য একীভূত map |
| ১১ | Lunar Landing Site Navigator | চাঁদের দক্ষিণ মেরুতে আলো ও যোগাযোগ |
| ১২ | Planet X and SPHEREx | সময়ের সঙ্গে SPHEREx আকাশ-চিত্রের পরিবর্তন |
| ১৩ | Space Mission Design Game | সম্পূর্ণ মহাকাশ-মিশনের পরিকল্পনা ও simulation |
| ১৪ | The Earth Information Jukebox | Earth science data-কে real-time sound-এ রূপান্তর |

---

# ৩. প্রতিটি Challenge-এর বিস্তারিত

## Challenge 1 — Abandoned but not Forgotten: Storytelling about NASA's Discarded Equipment on the Moon and Mars

**সহজ বাংলা ভাবার্থ:** ভুলে যাওয়া নয়—চাঁদ ও মঙ্গলে রেখে আসা NASA যন্ত্রপাতির গল্প  
**মূল ক্ষেত্র:** মহাকাশ অনুসন্ধান, planetary science, বিজ্ঞান যোগাযোগ, শিশু-কিশোর শিক্ষা  
**অফিসিয়াল পৃষ্ঠা:** [Abandoned but not Forgotten](https://www.spaceappschallenge.org/2026/challenges/nasas-discarded-equipment-storytelling/)

### সমস্যাটি কী?

১৯৬০-এর দশক থেকে NASA চাঁদ, মঙ্গল এবং গভীর মহাকাশে নানা ধরনের hardware পাঠিয়েছে। কোনো rover বা instrument তার বিজ্ঞান-কার্যক্রম শেষ করেছে, কোনো probe এখনও পৃথিবী থেকে দূরে ভ্রমণ করছে। যন্ত্রগুলোর উদ্দেশ্য, অবস্থা এবং এখনো কাজ করছে কি না—এসব একরকম নয়।

Challenge-টি এসব যন্ত্রের কিছু বা সবকিছুর গল্প বলতে বলে, যাতে school-age মহাকাশ-আগ্রহীরা জানতে পারে:

- যন্ত্রটি কী ছিল;
- কেন পাঠানো হয়েছিল;
- কীভাবে কাজ করত বা করে;
- সেটি কোন বিজ্ঞান সম্ভব করেছে;
- mission শেষে সেটির কী অবস্থা হয়েছে।

### “Discarded” শব্দটি বোঝার উপায়

এখানে discarded hardware মানে সব জিনিসকে “আবর্জনা” বলা নয়। কোনো যন্ত্র কাজ শেষ করে কোনো গ্রহ/উপগ্রহে থেকে যেতে পারে; কোনো probe mission শেষেও চলতে পারে। গল্পে প্রতিটি বস্তু সম্পর্কে সঠিক অবস্থা যাচাই জরুরি।

### সম্ভাব্য deliverable

- শিশুদের illustrated digital story;
- interactive timeline বা map;
- short animation/ভিডিও;
- mission card collection;
- classroom activity বা printable story;
- একটি lander/rover/probe-এর perspective থেকে narrative।

### গল্পের কাঠামোর উদাহরণ

1. **চরিত্র:** একটি lander, instrument, rover বা probe বেছে নিন।
2. **যাত্রা:** কোথা থেকে, কখন, কেন পাঠানো হয়েছিল।
3. **কাজ:** কোন measurement বা ছবি সংগ্রহ করেছে।
4. **আবিষ্কার:** কোন প্রশ্নের উত্তর দিতে সাহায্য করেছে।
5. **বর্তমান অবস্থা:** চালু, নিষ্ক্রিয়, যোগাযোগহীন, নাকি এখনও যাত্রায়—উৎস দেখে বলুন।
6. **উত্তরাধিকার:** পরবর্তী mission বা মানুষের জ্ঞানে এর অবদান।

### গবেষণা ও যাচাই

- NASA mission page, image caption ও mission archive থেকে তথ্য নিন।
- তারিখ, অবস্থান, mission status ও instrument-এর নাম মিলিয়ে দেখুন।
- “চাঁদে ফেলে রাখা” আর “ইচ্ছাকৃতভাবে mission শেষে রেখে আসা”—দুইটি এক করে দেখাবেন না।
- শিল্পিত চরিত্রের কণ্ঠ ব্যবহার করলে বাস্তব তথ্য ও কল্পিত সংলাপ আলাদা রাখুন।

### শিশুদের জন্য নকশা

- নতুন শব্দের glossary;
- অল্প বাক্য ও স্পষ্ট ছবি;
- “তুমি হলে কী জানতে চাইতে?” ধরনের প্রশ্ন;
- image alt text, audio narration ও caption;
- বাস্তব scale না হলে “not to scale” চিহ্ন।

### সতর্কতা

- কোনো hardware-এর অবস্থা সম্পর্কে পুরোনো blog নয়, বর্তমান/বিশ্বস্ত NASA source ব্যবহার করুন।
- গল্পে কল্পিত আবেগ বা সংলাপ থাকলে সেটিকে ঐতিহাসিক উদ্ধৃতি বলে দেখাবেন না।
- শিশুদের জন্য বিষয় সহজ করুন, কিন্তু মূল বৈজ্ঞানিক তথ্য বদলে ফেলবেন না।

---

## Challenge 2 — Be An Earth System Trend Detective!

**সহজ বাংলা ভাবার্থ:** পৃথিবীর পরিবেশগত পরিবর্তনের গোয়েন্দা হোন  
**মূল ক্ষেত্র:** Earth science data, time-series, trend, statistical significance  
**অফিসিয়াল পৃষ্ঠা:** [Be An Earth System Trend Detective!](https://www.spaceappschallenge.org/2026/challenges/earth-system-trend-detective/)

### সমস্যাটি কী?

পৃথিবীর পরস্পর-সংযুক্ত পরিবেশে পরিবর্তন সবসময় চলতে থাকে। কোনো মাপ একদিকে বাড়তে বা কমতে পারে; একই প্রক্রিয়া এক অঞ্চলে এক রকম trend, অন্য অঞ্চলে বিপরীত trend তৈরি করতে পারে। প্রচুর Earth science variable থাকার কারণে:

- কোন variable পরিবর্তনের ইঙ্গিত দিতে পারে তা বেছে নেওয়া কঠিন;
- সেই variable-এর সময়ভিত্তিক বিশ্লেষণ করাও কঠিন;
- trend কোথায়, কতটা এবং তা statistically significant কি না বোঝাও কঠিন।

### Challenge-এর লক্ষ্য

এমন একটি tool তৈরি করা, যা:

1. Earth science mission থেকে মাপা বা model থেকে তৈরি variable বেছে নিতে পারে;
2. সময়ের সঙ্গে variable কীভাবে বদলায় দেখাতে পারে;
3. কী বদলাচ্ছে, কোথায় বদলাচ্ছে ও কতটা বদলাচ্ছে নির্ণয়ে সহায়তা করে;
4. পরিবর্তনটি বিজ্ঞানীদের অর্থে “significant” কি না বিশ্লেষণে সহায়তা করে।

### সম্ভাব্য feature

- variable catalog ও data source;
- অঞ্চল/সময় নির্বাচন;
- time-series chart;
- map-এ স্থানিক trend;
- slope/rate-of-change estimate;
- confidence interval বা uncertainty;
- statistical significance-এর ব্যাখ্যা;
- region-to-region comparison।

### বিশ্লেষণের ধাপ

1. variable-এর সংজ্ঞা, unit, dataset ও সময়সীমা বুঝুন।
2. missing value, sensor change ও data quality flag পরীক্ষা করুন।
3. trend-এর baseline method নির্ধারণ করুন।
4. seasonality ও autocorrelation বিবেচনা করুন।
5. একই analysis বহু অঞ্চলে চালিয়ে ফল তুলনা করুন।
6. significance test-এর assumptions স্পষ্ট করুন।
7. map ও chart-এ uncertainty দেখান।

### “Significant” মানে কী?

Statistical significance সবসময় “বাস্তব জীবনে বড় প্রভাব” বোঝায় না। বড় sample-এ খুব ছোট পরিবর্তনও statistically significant হতে পারে; আবার ছোট sample-এ গুরুত্বপূর্ণ পরিবর্তন ধরা নাও পড়তে পারে। তাই effect size/rate-of-change, confidence interval, statistical test এবং practical/ecological context একসঙ্গে ব্যাখ্যা করুন।

### সতর্কতা

- correlation-কে কারণ হিসেবে ঘোষণা করবেন না।
- এক অঞ্চল ও অন্য অঞ্চলের trend বিপরীত হলে তা গড়ে লুকিয়ে ফেলবেন না।
- model output ও satellite measurement আলাদা label দিন।
- variable-এর সময়/স্থানিক resolution-এর চেয়ে বেশি সূক্ষ্ম ফল দেখাবেন না।

---

## Challenge 3 — Build a Junior Astronaut Mission Trainer

**সহজ বাংলা ভাবার্থ:** ছোটদের জন্য মহাকাশচারী-মিশন প্রশিক্ষণ game  
**মূল ক্ষেত্র:** STEM education, game design, Moon/Mars outpost, resource trade-off  
**অফিসিয়াল পৃষ্ঠা:** [Build a Junior Astronaut Mission Trainer](https://www.spaceappschallenge.org/2026/challenges/junior-astronaut-mission-trainer/)

### সমস্যাটি কী?

মহাকাশভিত্তিক STEM কনটেন্ট অনেক সময় বাস্তব মিশনের engineering trade-off-কে অতিরিক্ত সরল করে, অথবা এত জটিল করে যে তরুণ শিক্ষার্থী আগ্রহ হারায়। এমন tool কম, যা trade-off-কে একই সঙ্গে বাস্তবধর্মী ও মজার করে।

### Challenge-এর লক্ষ্য

একটি interactive game বা app বানানো, যাতে শিক্ষার্থী lunar বা Martian outpost পরিচালনা করে সীমিত সম্পদের মধ্যে একাধিক চাহিদার ভারসাম্য রাখবে:

- life support;
- radiation shielding;
- power;
- food production।

শিক্ষার্থীকে সিদ্ধান্তের ফল দেখতে হবে—মিশন সফল বা ব্যর্থ হওয়ার পেছনে কোন সিদ্ধান্ত কী ভূমিকা রাখল।

### সম্ভাব্য game loop

1. Moon/Mars ও crew size বেছে নেওয়া;
2. power, water, food, shielding, maintenance-এর budget দেখা;
3. outpost-এ module/technology নির্বাচন;
4. environmental event বা equipment failure সামলানো;
5. mission status ও crew well-being দেখা;
6. সিদ্ধান্তের ফল থেকে পরবর্তী run-এ শেখা।

### সম্ভাব্য trade-off

- বেশি radiation shielding নিলে mass/transport cost বাড়ে;
- বড় food-production system power ও পানি চায়;
- বেশি power system রাখলে spare mass/space কমতে পারে;
- crew size বাড়লে life support ও food need বাড়ে।

এসব game mechanic হিসেবে ব্যবহার করলে relation-গুলো বাস্তব বৈজ্ঞানিক/engineering উৎসের সঙ্গে মিলিয়ে নিন; সহজীকরণ থাকলে সেটি জানান।

### সতর্কতা

- একটি game model বাস্তব mission-এ ব্যবহারের উপযোগী engineering software নয়।
- বাস্তব mission-এর performance guarantee বা exact requirement বলে দেখাবেন না।
- gameplay সহজ করতে assumption পরিবর্তন করলে তা teacher note-এ লিখুন।

---

## Challenge 4 — Create Health Monitoring Software for Astronauts on Space Missions

**সহজ বাংলা ভাবার্থ:** দীর্ঘ মহাকাশ-মিশনে astronaut-এর স্বাস্থ্য নজরদারির software  
**মূল ক্ষেত্র:** human spaceflight, health indicators, self-monitoring, decision support  
**অফিসিয়াল পৃষ্ঠা:** [Create Health Monitoring Software for Astronauts on Space Missions](https://www.spaceappschallenge.org/2026/challenges/health-monitoring-software/)

### সমস্যাটি কী?

দীর্ঘ মহাকাশ-মিশনে astronaut-রা space radiation, isolation/confinement, altered gravity এবং hostile closed environment-এর মুখোমুখি হন। এর সঙ্গে immune change, bone loss, cardiovascular event ও behavioral health problem-এর ঝুঁকি যুক্ত হতে পারে। দীর্ঘ মিশনে astronaut-দের নিজেদের health change শনাক্ত করার দায়ও অনেক সময় নিজেদের ওপর থাকে।

### Challenge-এর লক্ষ্য

এমন health-monitoring software তৈরি করা, যা health indicator সংগ্রহ করে astronaut-কে নিজের health status মূল্যায়ন করতে এবং উপযুক্ত পদক্ষেপ নিতে সাহায্য করে।

### সম্ভাব্য user flow

1. astronaut দৈনিক/নিয়মিত health indicator নথিভুক্ত করেন;
2. software সময়ের সঙ্গে trend দেখায়;
3. ব্যক্তিগত baseline-এর তুলনায় পরিবর্তন দেখায়;
4. গুরুত্বপূর্ণ পরিবর্তন হলে review/attention-এর নির্দেশ দেয়;
5. astronaut ও প্রাসঙ্গিক medical/mission support-এর জন্য summary তৈরি করে।

### সম্ভাব্য design principle

- ব্যক্তিগত baseline-কে গুরুত্ব;
- দীর্ঘমেয়াদি trend ও short-term alert আলাদা;
- low-bandwidth/offline use;
- data privacy ও access control;
- health record auditability;
- কোন indicator কেন flag হয়েছে তা ব্যাখ্যা;
- manual entry ও sensor data-এর উৎস আলাদা।

### Human factors

- ব্যস্ত crew-র জন্য দ্রুত input;
- fatigue/low-light/limited interface context;
- alert overload এড়ানো;
- ব্যক্তিগত স্বাস্থ্য-তথ্য গোপন রাখা;
- crew member-কে সম্মানজনক, non-judgmental ভাষা;
- mission control ও astronaut-এর data-sharing control।

### সতর্কতা

- prototype-কে diagnosis বা clinical treatment tool বলবেন না।
- synthetic sample data-কে real astronaut health record বলে দেখাবেন না।
- alert threshold-এর চিকিৎসাবৈজ্ঞানিক ভিত্তি না থাকলে “demo threshold” বলে চিহ্নিত করুন।
- sensitive health information নিরাপদে সংরক্ষণ, access ও delete করার নীতি দেখান।
- জরুরি অবস্থায় বাস্তব medical professional/mission protocol-ই কর্তৃত্বপূর্ণ।

---

## Challenge 5 — Dancing with the SARs

**সহজ বাংলা ভাবার্থ:** NISAR radar data দিয়ে পৃথিবীর পৃষ্ঠের পরিবর্তনের নৃত্য দেখা  
**মূল ক্ষেত্র:** SAR, NISAR, ভূ-পৃষ্ঠের পরিবর্তন, interactive Earth science app  
**অফিসিয়াল পৃষ্ঠা:** [Dancing with the SARs](https://www.spaceappschallenge.org/2026/challenges/dancing-with-the-sars/)

### সমস্যাটি কী?

পৃথিবীর পৃষ্ঠে প্রাকৃতিক প্রক্রিয়া ও মানুষের কাজের কারণে অবিরাম পরিবর্তন ঘটে—জলাভূমি হারানো, বন-আগুন, ভূমিকম্প, কৃষিকাজ, হিমবাহের গতি ইত্যাদি। এসব পরিবর্তন বোঝা ও যোগাযোগ করা কঠিন হতে পারে।

### Challenge-এর লক্ষ্য

NASA-ISRO Synthetic Aperture Radar (NISAR) mission-এর radar remote-sensing data ব্যবহার করে পৃথিবীর বিভিন্ন স্থানে এক বা একাধিক ধরনের surface change track ও visualize করার interactive application তৈরি করা।

### SAR সহজভাবে

SAR পৃথিবীতে radar signal পাঠায় এবং পৃষ্ঠের সঙ্গে signal-এর interaction-এর পর ফিরে আসা energy পরিমাপ করে। এটি optical camera-র মতো দৃশ্যমান আলো-নির্ভর ছবি নয়। এর ফলে মেঘ বা অন্ধকারের মধ্যেও কিছু পর্যবেক্ষণ সম্ভব হতে পারে, তবে SAR image ব্যাখ্যার নিজস্ব জটিলতা আছে।

### সম্ভাব্য change type ও feature

- বন্যা বা জলাভূমির পরিবর্তন;
- ভূমিকম্প/ভূ-পৃষ্ঠের deformation;
- glacier movement;
- forest disturbance;
- কৃষি/ভূমি ব্যবহারের পরিবর্তন;
- আগ্নেয়গিরি বা ভূমিধস-সম্পর্কিত পরিবর্তন;
- স্থান/ঘটনা বেছে নিয়ে বিভিন্ন সময়ের image তুলনা;
- change layer, time slider, annotation ও data-quality indicator।

### কাজের ধাপ

1. একটি phenomenon এবং study area বেছে নিন।
2. ওই area-র NISAR data availability ও observation date যাচাই করুন।
3. pre/post-event বা repeated observation তুলনা করুন।
4. SAR processing, polarization, geometry ও quality flag বুঝুন।
5. change detection-এর একটি transparent method প্রয়োগ করুন।
6. ফল map-এ দেখিয়ে alternative explanation লিখুন।

### সতর্কতা

- SAR backscatter পরিবর্তনকে সরাসরি “এখানে বন্যা/ভূমিকম্প হয়েছে” বলে ধরে নেবেন না।
- incidence angle, terrain shadow/layover, speckle, surface moisture ও processing ফলকে প্রভাবিত করতে পারে।
- NISAR-এর data coverage, cadence ও product availability official resource দিয়ে যাচাই করুন।
- algorithm যে signal ধরেছে, তার scientific interpretation আলাদা ধাপ।

---

## Challenge 6 — Field Shift: Adapting Farms with NASA Data

**সহজ বাংলা ভাবার্থ:** NASA data ব্যবহার করে ফসল-পর্যায় পরিবর্তনের মাধ্যমে খামারকে অভিযোজিত করা  
**মূল ক্ষেত্র:** কৃষি, crop rotation, soil health, climate adaptation, decision support  
**অফিসিয়াল পৃষ্ঠা:** [Field Shift: Adapting Farms with NASA Data](https://www.spaceappschallenge.org/2026/challenges/adapting-farms-with-nasa-data/)

### সমস্যাটি কী?

বিশ্বের কৃষকেরা পরিবর্তিত তাপমাত্রা, বৃষ্টিপাত, পানির ঘাটতি, extreme weather ও মাটির স্বাস্থ্যহানির মুখোমুখি হন। এই পরিস্থিতিতে জমি রক্ষা, পানি সংরক্ষণ ও দীর্ঘমেয়াদি resilience বাড়াতে কোন crop rotation বেছে নেওয়া উচিত তা নির্ধারণ কঠিন।

### Challenge-এর লক্ষ্য

এমন decision-support tool তৈরি করা, যা NASA Earth observation, স্থানীয় মাটির তথ্য, ফসলের বৈশিষ্ট্য এবং কৃষকের অগ্রাধিকার একসঙ্গে বিবেচনা করে soil health বাড়াতে ও পরিবর্তিত অবস্থার সঙ্গে খাপ খাওয়াতে সম্ভাব্য crop rotation strategy অন্বেষণে সাহায্য করে।

### Crop rotation কী?

একই জমিতে বিভিন্ন মৌসুম/বছরে পরিকল্পিতভাবে ভিন্ন ফসল চাষ করা। ফসল নির্বাচন মাটির পুষ্টি, পানি, pest/disease cycle, বাজার, শ্রম ও আবহাওয়ার ওপর প্রভাব ফেলতে পারে।

### সম্ভাব্য user input/output

ইনপুট:

- location/field boundary;
- soil type/soil condition;
- বর্তমান/সম্ভাব্য crop;
- পানি/সেচের সুবিধা;
- farmer priorities: yield, soil cover, water saving, market value;
- climate conditions/seasonal outlook;
- local constraints।

আউটপুট:

- alternative rotation sequence;
- soil/water indicator-এর qualitative comparison;
- trade-off chart;
- input assumptions ও data source;
- farmer preference অনুযায়ী ranking;
- uncertainty/region coverage note।

### কাজের ধাপ

1. কৃষকের বাস্তব সিদ্ধান্ত—কোন ফসল কখন ঘোরাবেন—সুনির্দিষ্ট করুন।
2. NASA Earth observation data-র সঙ্গে local soil/crop data কীভাবে যুক্ত হবে ঠিক করুন।
3. দুই বা তিনটি rotation option তুলনা করুন।
4. scoring method প্রকাশ করুন; কৃষকের preference-কে গোপনে weight দেবেন না।
5. স্থানীয় কৃষি-বিশেষজ্ঞ/ব্যবহারকারীর feedback নিন।
6. একটি sample farm-এ prototype demo করুন।

### সতর্কতা

- উপগ্রহ-তথ্য একাই মাটির সব বৈশিষ্ট্য বা ফলন নির্ধারণ করে না।
- “সেরা rotation” স্থানীয় বাজার, বীজ, শ্রম, সেচ ও মাটির ওপর নির্ভরশীল।
- tool-কে কৃষিবিদের বিকল্প নয়, সিদ্ধান্ত-আলোচনার সহায়ক হিসেবে উপস্থাপন করুন।
- model score-কে measured outcome বলে দেখাবেন না।

---

## Challenge 7 — Flame in Freefall: SI-Powered Fire Safety Insights from Microgravity Combustion Data

**সহজ বাংলা ভাবার্থ:** মাইক্রোগ্র্যাভিটিতে আগুনের তথ্য থেকে মহাকাশের fire-safety insight  
**মূল ক্ষেত্র:** combustion, microgravity, space safety, SI dashboard, research data  
**অফিসিয়াল পৃষ্ঠা:** [Flame in Freefall](https://www.spaceappschallenge.org/2026/challenges/flame-in-freefall/)

### সমস্যাটি কী?

NASA কয়েক দশক ধরে microgravity-তে flame ও fire-এর আচরণ নিয়ে গবেষণা করেছে। চাঁদে ফিরে যাওয়া ও মঙ্গল অনুসন্ধানের আগে এই জ্ঞান আরও গুরুত্বপূর্ণ, কিন্তু গবেষণার ফল অনেক হওয়ায় সেগুলো খুঁজে পাওয়া, তুলনা করা ও বোঝা কঠিন।

### Challenge-এর লক্ষ্য

একটি interactive, **super intelligence (SI)-powered** dashboard তৈরি করা, যা microgravity combustion data/findings:

- summarize করে;
- rank করে;
- interpret করে;
- human space exploration-এর fire-safety insight দিতে সাহায্য করে।

### সম্ভাব্য dashboard feature

Challenge statement SI শব্দ ব্যবহার করেছে; কোন নির্দিষ্ট প্রযুক্তি/architecture বাধ্যতামূলক—তা পূর্ণ resource থেকে যাচাই করুন। সম্ভাব্য ক্ষমতা:

- natural-language search;
- paper/experiment comparison;
- condition অনুযায়ী filtering;
- evidence-linked summary;
- safety-relevant result ranking;
- user প্রশ্নের উত্তরে source passage দেখানো।

### সম্ভাব্য data structure

- experiment/test-এর নাম;
- fuel, oxidizer, pressure, atmosphere;
- gravity condition;
- flame size/temperature/behavior;
- ignition/extinction outcome;
- instrument, date, mission/facility;
- publication, report বা source link।

সব field প্রতিটি study-তে থাকবে এমন নয়; absent/unknown আলাদা করে দেখাতে হবে।

### Workflow ও যাচাই

1. Official resource-এ থাকা combustion experiment/data সংগ্রহ করুন।
2. metadata ও vocabulary normalize করুন।
3. experiment condition ও outcome-এর structured index তৈরি করুন।
4. dashboard search/filter ও comparison দিন।
5. SI-generated summary-তে source passage/citation যুক্ত করুন।
6. ranking কীভাবে কাজ করে ব্যাখ্যা করুন।
7. fire-safety conclusion review/validation করুন।

### সতর্কতা

- AI summary-কে operational fire procedure হিসেবে ব্যবহার করা যাবে না।
- source ছাড়া “এটাই নিরাপদ” দাবি করবেন না।
- “Super intelligence” নাম শুনে model-এর ক্ষমতা অতিরঞ্জিত করবেন না; prototype-এর বাস্তব ক্ষমতা বলুন।
- human review, citation ও failure reporting রাখুন।

---

## Challenge 8 — Harmonization of MODIS and VIIRS Hot Spots

**সহজ বাংলা ভাবার্থ:** MODIS ও VIIRS উপগ্রহের আগুনের hotspot record-কে তুলনাযোগ্য করা  
**মূল ক্ষেত্র:** active fire detection, satellite data harmonization, fire calendar, response planning  
**অফিসিয়াল পৃষ্ঠা:** [Harmonization of MODIS and VIIRS Hot Spots](https://www.spaceappschallenge.org/2026/challenges/modis-and-viirs-hot-spots/)

### সমস্যাটি কী?

বন-আগুন ও কৃষিজ burning-সহ পৃথিবীতে কোথায়/কখন আগুন জ্বলছে তা বোঝা জরুরি। দুই দশকেরও বেশি সময় ধরে satellite active-fire hotspot track করেছে, কিন্তু record বিভিন্ন sensor-এ বিভক্ত এবং সেগুলো সরাসরি তুলনাযোগ্য নয়। ফলে fire manager-দের কাছে কখন/কোথায় burning হয়েছে তার একটানা consistent picture থাকে না।

### Challenge-এর লক্ষ্য

একটি web application তৈরি করা, যা MODIS ও VIIRS-এর active-fire hotspot record harmonize করে **burning activity calendar** তৈরি করবে। এতে selected area-র historical fire pattern, অস্বাভাবিক অবস্থা এবং গুরুত্বপূর্ণ সময় দেখা যাবে; emergency responder, scientist ও land manager-রা তথ্য পর্যালোচনা করতে পারবেন।

### Harmonization কেন দরকার?

বিভিন্ন sensor-এর spatial resolution, detection threshold, orbit/overpass, calibration ও algorithm এক নয়। ভিন্ন sensor-এর point count সরাসরি যোগ করলে দীর্ঘমেয়াদি trend ভুল বোঝা যেতে পারে।

### সম্ভাব্য feature

- area of interest নির্বাচন;
- বছর/মাস/দিনের calendar view;
- hotspot frequency/seasonality;
- MODIS বনাম VIIRS overlap/coverage;
- sensor-specific filter;
- unusual activity highlight;
- source time ও quality indicator;
- downloadable chart/table।

### কাজের ধাপ

1. official hotspot product, unit ও quality flags বুঝুন।
2. sensor-specific resolution/detection differences নথিভুক্ত করুন।
3. harmonization rule বেছে নিয়ে document করুন।
4. একই এলাকার overlap data দিয়ে method sanity-check করুন।
5. calendar-এ missing observation ও uncertainty আলাদা দেখান।
6. historical pattern এবং anomaly সংজ্ঞা স্পষ্ট করুন।

### সতর্কতা

- satellite hotspot মানেই আগুনের পূর্ণ perimeter নয়।
- একটি hotspot সরাসরি আগুনের মোট ক্ষেত্রফল বলে না।
- cloud, overpass time, sensor sensitivity ও false detection ফলকে প্রভাবিত করে।
- “early warning” বলতে historical/near-real-time context বোঝালে latency স্পষ্ট করুন; ভবিষ্যৎ আগুন নিশ্চিতভাবে forecast করার দাবি করবেন না।

---

## Challenge 9 — Identify Earth Locations that Analog the Permanent Moon Base Locations and Mars

**সহজ বাংলা ভাবার্থ:** চাঁদ/মঙ্গলের স্থায়ী ঘাঁটির অনুরূপ পৃথিবীর স্থান খুঁজে বের করা  
**মূল ক্ষেত্র:** planetary analog sites, Earth/Moon/Mars data, field testing, GIS  
**অফিসিয়াল পৃষ্ঠা:** [Identify Earth Locations that Analog the Permanent Moon Base Locations and Mars](https://www.spaceappschallenge.org/2026/challenges/permanent-moon-base-locations-and-mars/)

### সমস্যাটি কী?

চাঁদের স্থায়ী ঘাঁটি বা ভবিষ্যৎ landing site নির্বাচন করতে topography, geology, environment ও resource-এর মতো অনেক বিষয় বিবেচনা করতে হয়। পৃথিবীর Atacama Desert, Haughton Crater, Death Valley-এর মতো স্থান চাঁদ/মঙ্গলের কিছু পরিবেশের analog হিসেবে equipment ও method পরীক্ষা করতে সাহায্য করে; কিন্তু এসব terrestrial analog পুরোপুরি characterize করা হয়নি।

### Challenge-এর লক্ষ্য

NASA ও অন্যান্য space agency-র উন্মুক্ত Earth, Moon ও Mars data ব্যবহার করে নতুন terrestrial analog location শনাক্ত ও characterize করা। ফলাফল map, visualization বা অন্য tool-এ দেখাতে হবে। সম্ভাব্য পরিবেশের মধ্যে মরুভূমি, মেরু অঞ্চল, আগ্নেয়/শুষ্ক ভূমি, গুহা ও lunar/Martian surface-এর সঙ্গে কিছু বৈশিষ্ট্য ভাগ করা অন্যান্য স্থান আছে।

### Analog site মানে কী?

Analog site হলো পৃথিবীর এমন পরিবেশ, যার নির্দিষ্ট বৈশিষ্ট্য অন্য গ্রহ/উপগ্রহের পরিবেশের সঙ্গে তুলনা করে equipment বা procedure পরীক্ষা করা যায়। এটি চাঁদ বা মঙ্গলের হুবহু duplicate নয়।

### তুলনার সম্ভাব্য dimension

- ভূমির ঢাল/উচ্চতা;
- geology/mineral/rock context;
- temperature range;
- radiation exposure-এর analog condition;
- dust/soil characteristics;
- water/ice বা resource availability;
- isolation/accessibility;
- communication/terrain visibility;
- field testing logistics।

সব মাত্রার data পাওয়া নাও যেতে পারে; absent data-কে “অজানা” রাখুন, বানিয়ে পূরণ করবেন না।

### সম্ভাব্য tool ও workflow

- Earth analog site map;
- Moon/Mars target-এর সঙ্গে side-by-side comparison;
- multi-criteria ranking;
- selected site profile;
- environment factor-এর radar/chart;
- data provenance/uncertainty layer।

কাজের ধাপ:

1. lunar/Martian target environment নির্ধারণ করুন।
2. তুলনীয় Earth/Moon/Mars datasets নির্বাচন করুন।
3. spatial projection ও resolution সামঞ্জস্য করুন।
4. কোন বৈশিষ্ট্যে analog, কোন বৈশিষ্ট্যে ভিন্ন তা প্রকাশ করুন।
5. scoring থাকলে criterion ও weight দেখান।
6. map-এ candidate site ও confidence দেখান।

### সতর্কতা

- পৃথিবীর স্থানকে “মঙ্গলের সমান” বলা যাবে না।
- analog উদ্দেশ্যভেদে বদলে যায়—suit test, mobility, geology, human factors এক নয়।
- বহু-মানদণ্ড score scientific truth নয়; design choice।
- বাস্তব field work-এ land access, protected area ও স্থানীয় জনগোষ্ঠীর অধিকার গুরুত্বপূর্ণ।

---

## Challenge 10 — Interplanetary Survival Guide: Martian Map

**সহজ বাংলা ভাবার্থ:** মঙ্গলে নিরাপদে হাঁটা ও বিজ্ঞান করার জন্য layered map  
**মূল ক্ষেত্র:** Mars exploration, route planning, mission science data, geospatial visualization  
**অফিসিয়াল পৃষ্ঠা:** [Interplanetary Survival Guide: Martian Map](https://www.spaceappschallenge.org/2026/challenges/interplanetary-survival-guide-martian-map/)

### সমস্যাটি কী?

NASA কয়েক দশক ধরে robotic mission দিয়ে Mars-এর কঠিন পরিবেশ গবেষণা, পৃষ্ঠ মানচিত্রায়ন এবং বিভিন্ন ধরনের data সংগ্রহ করেছে। পৃথিবী থেকে দূরে প্রথম astronaut-রা Mars-এ গেলে তাদের দরকার হবে route ও destination-এর সূক্ষ্ম বিবরণ, বর্তমান condition-এর update এবং দ্রুত ও নিরাপদে mission সম্পন্নের জন্য দরকারি data।

### Challenge-এর লক্ষ্য

একটি Martian location বা route-এর **layered, integrated view** বানানো, যা একাধিক NASA science mission-এর data একত্র করে human explorer-কে Marswalk পরিকল্পনা, নিরাপদে সম্পন্ন ও পাশাপাশি নতুন বিজ্ঞান করতে সাহায্য করতে পারে।

### সম্ভাব্য map layer

- terrain/topography;
- slope ও roughness;
- imagery;
- geology/mineral context;
- rover/lander observation;
- hazard/route constraint;
- science target;
- distance/time estimate;
- mission status বা data freshness।

এইগুলো প্রস্তাবিত layer; data availability official resource অনুযায়ী যাচাই করতে হবে।

### Marswalk user workflow

1. Mars-এর area/target নির্বাচন;
2. start/end point নির্ধারণ;
3. terrain ও hazard layer দেখা;
4. science target বা stop point যুক্ত;
5. alternate route তুলনা;
6. route-এর distance, slope, uncertainty ও source দেখা;
7. field/mission note export।

### “Survival Guide” নামের অর্থ

এটি শুধু narrative survival manual নয়; map-টির মূল কাজ হলো route/location-এর সঙ্গে বহু mission data যুক্ত করে explorer-এর planning-এ সহায়তা। বাস্তব astronaut safety protocol-কে prototype-এ নিজে থেকে উদ্ভাবন করবেন না।

### সতর্কতা

- rover path বা remote sensing data human-scale terrain-এর সম্পূর্ণ নিরাপত্তা নিশ্চিত করে না।
- map resolution, coordinate reference, data age ও missing region উল্লেখ করুন।
- route algorithm একটি candidate দিতে পারে; mission team review অপরিহার্য।
- Mars-এর বর্তমান local weather/environment data না থাকলে static geology/topography-কে “live current condition” বলবেন না।

---

## Challenge 11 — Lunar Landing Site Navigator

**সহজ বাংলা ভাবার্থ:** চাঁদের landing site ও তারিখের আলো-যোগাযোগ তুলনার navigator  
**মূল ক্ষেত্র:** lunar south pole, Sun/Earth geometry, power, communication, mission planning  
**অফিসিয়াল পৃষ্ঠা:** [Lunar Landing Site Navigator](https://www.spaceappschallenge.org/2026/challenges/lunar-landing-site-navigator/)

### সমস্যাটি কী?

চাঁদের দক্ষিণ মেরুতে mission চালাতে অত্যন্ত জটিল lighting ও communication condition মোকাবিলা করতে হয়। Candidate landing site-এ সূর্য ও পৃথিবীর অবস্থান জানার tool থাকলেও interface জটিল হতে পারে; science ও engineering team-এর পক্ষে গুরুত্বপূর্ণ তথ্য দ্রুত তুলনা করা কঠিন হয়।

### Challenge-এর লক্ষ্য

একটি intuitive tool/app বানানো, যাতে mission planner, educator ও public:

- landing site তুলনা;
- তারিখ তুলনা;
- horizon-এর তুলনায় Sun/Earth-এর অবস্থান visualize;
- power generation potential;
- direct-to-Earth communication window;

দ্রুত মূল্যায়ন করতে পারে।

### কেন Sun position জরুরি?

Solar-powered equipment-এর জন্য সূর্যালোকের সময় ও কোণ গুরুত্বপূর্ণ। Moon-এর terrain/horizon-এর কারণে কোনো স্থানে সূর্য সব সময় দৃশ্যমান নাও হতে পারে। Landing site ও date অনুযায়ী illumination window বদলে যায়।

### কেন Earth position জরুরি?

Direct-to-Earth communication-এর জন্য Earth-এর line-of-sight দরকার হতে পারে। স্থানীয় terrain বা Moon-এর curvature যোগাযোগে বাধা দিতে পারে। Tool-এ visibility window ও occlusion-এর ধারণা দেখানো যেতে পারে।

### সম্ভাব্য interface

- map-এ candidate site নির্বাচন;
- date/time slider;
- local horizon profile;
- Sun altitude/azimuth diagram;
- Earth visibility/communication window;
- sunlight duration/illumination chart;
- location/date side-by-side comparison;
- input assumptions ও source data।

### সতর্কতা

- Sun দৃশ্যমান থাকা মানেই solar power নিরবচ্ছিন্ন/যথেষ্ট হবে না; equipment, angle, terrain shadow ও dust বিবেচনা জরুরি।
- Earth দৃশ্যমানতা মানেই যোগাযোগ নিশ্চিত নয়; antenna, relay, bandwidth ও network architecture লাগে।
- prototype-কে mission-certified planning software বলবেন না।

---

## Challenge 12 — Planet X and SPHEREx

**সহজ বাংলা ভাবার্থ:** SPHEREx-এর আকাশ-চিত্রে সময়ের সঙ্গে বদলানো বস্তু দেখা  
**মূল ক্ষেত্র:** SPHEREx, time-domain astronomy, near-infrared image, object detection  
**অফিসিয়াল পৃষ্ঠা:** [Planet X and SPHEREx](https://www.spaceappschallenge.org/2026/challenges/planet-x-and-spherex/)

### সমস্যাটি কী?

২০২৫ সাল থেকে NASA-র SPHEREx mission প্রতি ছয় মাসে পুরো আকাশকে near-infrared আলোতে ১০২টি band-এ map করছে; এতে এক বিলিয়নের বেশি object-এর image তৈরি হচ্ছে। বিভিন্ন image-এ position বদলে যাওয়া comet, asteroid, star, brown dwarf বা নতুন planet-জাতীয় object দেখা দিতে পারে। এত data একা একজন মানুষের যাচাই করা সম্ভব নয়।

### Challenge-এর লক্ষ্য

একটি public-facing web tool তৈরি করা, যা SPHEREx mission-এর sky image দেখায় এবং যে কেউ সময়ের সঙ্গে image কীভাবে বদলায় দ্রুত দেখতে পারে।

### “Planet X” নামটি কী বোঝায়?

Challenge title-এ Planet X আছে, কিন্তু card statement-এ tool-এর লক্ষ্য SPHEREx image-এ পরিবর্তনশীল বস্তু দেখতে দেওয়া। তাই কোনো নির্দিষ্ট অজানা গ্রহ আবিষ্কার project-এর নিশ্চিত ফল—এমন বলা যাবে না। পরিবর্তন দেখা, candidate চিহ্নিত করা ও scientific validation পৃথক ধাপ।

### সম্ভাব্য user flow

1. আকাশের অঞ্চল/coordinate নির্বাচন;
2. আলাদা observation date বা band নির্বাচন;
3. image blink/slider দিয়ে তুলনা;
4. moving/transient candidate highlight;
5. known object catalog বা metadata overlay;
6. source image ও observation details দেখা;
7. user candidate annotation জমা দিতে পারে।

### সতর্কতা

- image shift হতে পারে astrometric alignment, instrument, artifact বা registration error-এর জন্য।
- একটি moving dot মানেই নতুন গ্রহ নয়।
- SPHEREx data-র release/availability ও band semantics official resource দেখে যাচাই করুন।
- public user candidate-কে confirmed discovery বলা যাবে না।

---

## Challenge 13 — Space Mission Design Game

**সহজ বাংলা ভাবার্থ:** সম্পূর্ণ মহাকাশ-মিশন পরিকল্পনা করার interactive game  
**মূল ক্ষেত্র:** mission engineering, resource management, game design, education  
**অফিসিয়াল পৃষ্ঠা:** [Space Mission Design Game](https://www.spaceappschallenge.org/2026/challenges/space-mission-design-game/)

### সমস্যাটি কী?

মহাকাশ-মিশন design করতে অনেক প্রতিযোগী চাহিদা একসঙ্গে বিবেচনা করতে হয়:

- mission objective;
- spacecraft design;
- scientific instrument;
- launch vehicle;
- budget;
- power;
- mass;
- communication;
- orbital constraint।

শিক্ষার্থীরা প্রায়ই পুরো mission concept থেকে operation পর্যন্ত experiment করার সুযোগ পায় না, ফলে এই trade-off abstract থেকে যায়।

### Challenge-এর লক্ষ্য

একটি interactive game তৈরি করা, যাতে অংশগ্রহণকারী পুরো space mission design, manage ও simulate করতে পারে; engineering decision নেয়, সীমিত resource সামলায় এবং প্রতিটি choice mission success-কে কীভাবে বদলায় তা মূল্যায়ন করে।

### সম্ভাব্য game stages

1. mission goal নির্বাচন;
2. target, spacecraft ও instrument নির্বাচন;
3. launch vehicle ও budget সামলানো;
4. mass/power/communication budget মিলানো;
5. orbit/trajectory বা mission timeline;
6. operation-এ unexpected event;
7. data return/science success মূল্যায়ন।

### মূল design lesson

একটি subsystem-এ উন্নতি অন্য constraint-এ খরচ বাড়াতে পারে। উদাহরণস্বরূপ, বেশি instrument science value বাড়ালেও mass/power/data budget বাড়াতে পারে। Game mechanic-এ এসব relation সহজ করে দেখানো যায়, তবে আসল physics/engineering থেকে কতটা সরল করা হয়েছে তা স্পষ্ট করুন।

### সতর্কতা

- game-এর simplified orbital/engineering model বাস্তব mission design tool নয়।
- একটি মাত্র “সঠিক” উত্তর নাও থাকতে পারে; trade-off-কে শেখার অংশ করুন।
- budget/mission performance-এর সংখ্যাগুলো illustrative হলে তা জানান।

---

## Challenge 14 — The Earth Information Jukebox

**সহজ বাংলা ভাবার্থ:** পৃথিবীর data-কে শব্দ/সংগীতে শোনার “Earth Jukebox”  
**মূল ক্ষেত্র:** NASA Earth Information Center, sonification, accessibility, multimedia  
**অফিসিয়াল পৃষ্ঠা:** [The Earth Information Jukebox](https://www.spaceappschallenge.org/2026/challenges/the-earth-information-jukebox/)

### সমস্যাটি কী?

NASA-র Earth Information Center (EIC) বদলে যাওয়া পৃথিবীর চমৎকার visualization তৈরি করে। শুধু visual দিয়ে Earth science উপস্থাপন করলে সবার কাছে পৌঁছানো যায় না। Challenge-টি sight-কে sound-এ রূপান্তর করে জটিল Earth science-কে accessible, engaging ও multisensory করতে আহ্বান জানায়।

### Challenge-এর লক্ষ্য

একটি “Earth Jukebox”—interface, script বা application—তৈরি করা, যা EIC-এর visual frame-এর সঙ্গে real time-এ তৈরি dynamic sonification যুক্ত করে।

### Sonification কী?

বৈজ্ঞানিক data-কে sound-এর বৈশিষ্ট্য—pitch, rhythm, timbre, volume বা spatial position—এর সঙ্গে mapping করে শোনানোকে sonification বলে। এটি data-র বিকল্প প্রমাণ নয়; অন্য ইন্দ্রিয় দিয়ে pattern বোঝার উপায়।

### সম্ভাব্য design

- EIC visual frame থেকে নির্দিষ্ট data layer বেছে নেওয়া;
- সময়/স্থান পরিবর্তনে sound পরিবর্তন;
- high/low data value-কে pitch বা rhythm-এ map;
- বহু variable-এর জন্য পৃথক instrument/timbre;
- user-নিয়ন্ত্রিত playback ও pause;
- sound-এর পাশে textual explanation;
- visual ও sonification-কে synchronized করা।

### Sonification mapping উদাহরণ

একটি variable বাড়লে pitch উঁচু করা যেতে পারে, অন্য variable-কে rhythm density-তে দেখানো যেতে পারে। তবে একসঙ্গে অনেক variable শুনালে noise/বিভ্রান্তি তৈরি হতে পারে; তাই একটি প্রধান variable দিয়ে শুরু করুন, mapping legend প্রকাশ করুন, user-কে variable toggle করতে দিন এবং data range/normalization ব্যাখ্যা করুন।

### Accessibility ও sensory design

- deaf/hard-of-hearing user-এর জন্য text/visual equivalent;
- blind/low-vision user-এর জন্য spoken description;
- volume/speed control;
- headphones বাধ্যতামূলক নয় এমন design;
- flashing visual/audio overload এড়ানো;
- sonification-এর meaning/legend সহজে পাওয়া।

### সতর্কতা

- sound সুন্দর হলেই data accurate হয় না; mapping scientifically transparent হওয়া দরকার।
- EIC-এর visual frame-এর copyright/attribution শর্ত যাচাই করুন।
- sound composition ও measured signal আলাদা label করুন।
- real-time data না হলে prerecorded/sample mode বলে দিন।

---

# ৪. ২০২৬ সালে event ও participation সম্পর্কে

Challenge list হলো প্রকল্পের বিষয়ের তালিকা; এটি event date, submission deadline, award eligibility বা registration status-এর পূর্ণ উৎস নয়। ২০২৬-এর সঠিক সময়, local event, submission policy, judging criteria ও award rules দেখতে ২০২৬-এর official event pages এবং সংশ্লিষ্ট Local Event-এর নির্দেশনা পড়ুন।

এই নথিতে event date অনুমান করে লেখা হয়নি। কারণ challenge list-এ একা প্রতিটি local schedule বা deadline নিশ্চিত নাও হতে পারে; তারিখ/নিয়ম সময়ের সঙ্গে বদলায়।

---

# ৫. Team কীভাবে বেছে নেবে?

## আগ্রহভিত্তিক বাছাই

- **পৃথিবী/পরিবেশ/মানচিত্র:** ২, ৫, ৬, ৮, ৯, ১০
- **মহাকাশ/চাঁদ/মঙ্গল:** ১, ৩, ৫, ৭, ৯, ১০, ১১, ১২, ১৩
- **AI/data analysis:** ২, ৪, ৭, ৮, ১২
- **শিক্ষা/game/story:** ১, ৩, ১৩
- **স্বাস্থ্য ও human factors:** ৪, ৫, ১১
- **sonification/arts:** ১৪
- **কৃষি:** ৬
- **space business/operations:** ৭, ১৩

## দক্ষতা অনুযায়ী ভূমিকা

| দক্ষতা | সম্ভাব্য কাজ |
|---|---|
| বিজ্ঞান/বিষয়জ্ঞান | source যাচাই, data interpretation, assumption review |
| Software | frontend/backend, data pipeline, API integration |
| Data science | cleaning, analysis, model, uncertainty/validation |
| Design/UX | user flow, interface, accessibility, visual clarity |
| Storytelling | narrative, educational text, demo script |
| Art/multimedia | illustration, animation, audio, 3D/VR |
| Project management | scope, task split, timebox, integration |
| Testing | user test, edge case, data quality, demo fallback |

একজন সদস্য একাধিক ভূমিকা নিতে পারেন; তবে বিজ্ঞান-নির্ভর ফলের source/validation-এর দায় নির্দিষ্ট করা ভালো।

---

# ৬. Hackathon-এ A-to-Z কাজের পরিকল্পনা

## A — Ask: প্রশ্ন লিখুন

এক বাক্যে লিখুন: “আমাদের project কার কোন সমস্যায় সাহায্য করবে?” প্রশ্নের উত্তর অস্পষ্ট হলে project scope ছোট করুন।

## B — Beneficiary: ব্যবহারকারী নির্ধারণ

শিক্ষার্থী, planner, কৃষক, জনসাধারণ, গবেষক, astronaut বা শিশু—কারা ব্যবহার করবে তা ঠিক করুন। “সবাই” ব্যবহারকারী হলে feature ও ভাষা নির্দিষ্ট করা কঠিন হয়।

## C — Challenge statement পড়ুন

শুধু card description নয়, পূর্ণ challenge page-এর Details ও Resources অংশ পড়ুন। প্রয়োজনীয় submission format বা resource-specific নির্দেশনা থাকলে সেটি আলাদা করে নোট করুন।

## D — Data source যাচাই

- data accessible কি?
- file/API format কী?
- resolution কত?
- time range কী?
- units/coordinate system কী?
- quality flag/missing data আছে?
- attribution/license কী?
- update latency কত?

প্রথমেই ছোট sample খুলে দেখুন। inaccessible data-র ওপর পুরো project নির্ভর করবেন না।

## E — Evidence & assumptions

প্রকল্প কোন observed data, কোন model, কোন user input ও কোন assumption ব্যবহার করছে আলাদা করে লিখুন।

## F — Feature priority

Must-have, should-have, could-have তালিকা করুন। hackathon-এ প্রথমে end-to-end মূল user journey শেষ করুন।

## G — Get a prototype running

prototype কাজ করুক; polished animation/feature পরে। Data → analysis → result → explanation—এই flow demo-তে শেষ পর্যন্ত চালাতে পারা চাই।

## H — Human-centered design

ব্যবহারকারীকে prototype নিজে চেষ্টা করতে দিন। “কোথায় click করতে হবে?” না বুঝিয়েও তিনি interface ব্যবহার করতে পারেন কি না লক্ষ্য করুন এবং বিভ্রান্তির জায়গাগুলো নোট করুন।

## I — Iterate

ব্যবহারকারীর প্রতিক্রিয়া, data error ও বিজ্ঞান-যাচাই অনুযায়ী দ্রুত সংশোধন করুন।

## J — Judge evidence

সাফল্য মাপুন: detector-এর metric, user task completion, lesson learning gain, map accuracy, বা forecast uncertainty—project অনুযায়ী।

## K — Keep it accessible

- readable contrast/font;
- keyboard navigation;
- subtitles/captions;
- alt text;
- color-blind friendly palette;
- mobile/low bandwidth consideration;
- সহজ ভাষার glossary।

## L — Label visualizations

Chart/map-এ title, date, units, legend, source, scale, projection/coordinate, missing data ও uncertainty দেখান।

## M — Make limitations visible

আপনার tool কী জানে না তা জানান। “এই data দিয়ে এটি বলা যায় না” বলাও ভালো বিজ্ঞান যোগাযোগ।

## N — No fabricated precision

উৎসের resolution যতটুকু, ফলকে তার চেয়ে বেশি precision দেখাবেন না। coarse satellite pixel থেকে বাড়ি-স্তরের সিদ্ধান্ত দাবি করবেন না।

## O — Open sources, proper credit

NASA/USGS/অন্যান্য data, image, sound, font, library ও third-party asset-এর source/license উল্লেখ করুন।

## P — Plan the demo

সংক্ষিপ্ত demo-তে সমস্যা, ব্যবহারকারী, data, সমাধান, live prototype, limitation ও next step দেখান।

## Q — Quality check

ফাইল load, broken link, incorrect units, mobile display, error message এবং offline/demo fallback পরীক্ষা করুন।

## R — Reproducibility

সম্ভব হলে data version, model parameters, steps ও code/source link দিন, যাতে অন্যরা ফল পুনরায় দেখতে পারে।

## S — Safety and privacy

location, sensitive community data, animal tracking, user account, health-related output—এসব ক্ষেত্রে privacy ও harm minimization বিবেচনা করুন।

## T — Team roles

একজনের ওপর সব কাজ না দিয়ে science/data, development, design, storytelling, testing ও presentation ভাগ করুন।

## U — User feedback

কমপক্ষে একজন প্রকৃত/সম্ভাব্য ব্যবহারকারীর feedback নিন; তবে project scope অতিক্রম করে user data সংগ্রহ করবেন না।

## V — Visual narrative

দর্শক যেন দেখতে পারে: “কী সমস্যা → কী তথ্য → কী পরিবর্তন/ফল → কেন এটি প্রাসঙ্গিক।”

## W — What is next?

Hackathon prototype-এর পরবর্তী উন্নয়ন—আরও data, validation, community trial, production engineering—চিহ্নিত করুন।

## X — eXplain uncertainty

probability, confidence interval, error bar বা qualitative uncertainty ব্যবহার করুন। “নিশ্চিত” বলে ঢেকে দেবেন না।

## Y — Your actual contribution

দলের সদস্য ও ব্যবহৃত tool-এর ভূমিকা সত্যভাবে উল্লেখ করুন।

## Z — Zero surprise submission

শেষ মুহূর্তে upload/format সমস্যা এড়াতে submission-এর নিয়ম, URL, access permission, backup video ও documentation আগে যাচাই করুন।

---

# ৭. সংক্ষিপ্ত শব্দ ও ধারণার অভিধান

| শব্দ | সহজ ব্যাখ্যা |
|---|---|
| **Earth System** | বায়ুমণ্ডল, জল, ভূমি, বরফ ও জীবজগতের পারস্পরিক সংযুক্ত ব্যবস্থা |
| **Trend** | সময়ের সঙ্গে কোনো variable-এর ধারাবাহিক বাড়া/কমা বা পরিবর্তনের ধারা |
| **Statistical significance** | নির্দিষ্ট statistical test ও assumptions অনুযায়ী পর্যবেক্ষিত পরিবর্তনকে chance দিয়ে ব্যাখ্যা করা কতটা অসঙ্গত |
| **Life support** | মানুষের বেঁচে থাকার জন্য বাতাস, পানি, তাপমাত্রা ইত্যাদি নিয়ন্ত্রণ |
| **Radiation shielding** | বিকিরণ থেকে crew/equipment-কে রক্ষার উপকরণ বা ব্যবস্থা |
| **SAR** | Synthetic Aperture Radar; radar signal ব্যবহার করে পৃষ্ঠ পর্যবেক্ষণ |
| **NISAR** | NASA-ISRO Synthetic Aperture Radar mission |
| **Crop rotation** | একই জমিতে বিভিন্ন সময়ে/মৌসুমে পরিকল্পিত ফসল পরিবর্তন করে চাষ |
| **Microgravity** | কক্ষপথে মুক্ত-পতনের কারণে কার্যকরভাবে কম মাধ্যাকর্ষণ অনুভূত হওয়ার পরিবেশ |
| **Combustion** | জ্বালানি ও oxidizer-এর রাসায়নিক বিক্রিয়া, যার ফলে তাপ/আলো উৎপন্ন হয় |
| **MODIS** | NASA-র Moderate Resolution Imaging Spectroradiometer instrument |
| **VIIRS** | Visible Infrared Imaging Radiometer Suite; satellite sensor instrument |
| **Hot spot** | satellite fire product-এ active burning-এর সম্ভাব্য pixel/স্থান |
| **Terrestrial analog** | অন্য গ্রহ/উপগ্রহের নির্দিষ্ট বৈশিষ্ট্যের সঙ্গে তুলনার জন্য ব্যবহৃত পৃথিবীর স্থান |
| **Marswalk** | মঙ্গলের পৃষ্ঠে astronaut-এর বাইরে গিয়ে কাজ/অনুসন্ধান |
| **Line of sight** | দুই অবস্থানের মধ্যে বাধাহীন সরল দৃষ্টিপথ/যোগাযোগের পথ |
| **SPHEREx** | আকাশের near-infrared survey করা NASA mission |
| **Time-domain astronomy** | সময়ের সঙ্গে জ্যোতির্বৈজ্ঞানিক বস্তু/উজ্জ্বলতা/অবস্থান বদল বিশ্লেষণ |
| **Sonification** | data-কে sound-এর বৈশিষ্ট্যে রূপান্তর করে শোনানো |
| **Decision support** | ব্যবহারকারীকে তথ্যভিত্তিক বিকল্প তুলনা করতে সাহায্যকারী ব্যবস্থা; নিজে চূড়ান্ত সিদ্ধান্ত নয় |
| **Harmonization** | ভিন্ন উৎস/সেন্সরের ডেটাকে তুলনাযোগ্য করার প্রক্রিয়া |
| **Uncertainty** | মাপ বা model result কতটা অনিশ্চিত তার পরিমাণ/বর্ণনা |
| **Prototype** | ধারণা ও মূল user flow যাচাইয়ের প্রাথমিক কার্যকর সংস্করণ |
| **Data provenance** | ডেটার উৎস, processing history ও version-এর রেকর্ড |

---

# ৮. অফিসিয়াল উৎস

- [NASA Space Apps Challenge 2026 — challenge তালিকা](https://www.spaceappschallenge.org/2026/challenges/)
- প্রতিটি challenge-এর সম্পূর্ণ official statement, additional details ও resources সংশ্লিষ্ট section-এর link-এ দেওয়া আছে।

## উৎস-নোট

1. অফিসিয়াল challenge list-এ ১৪টি challenge দেখানো হয়েছে; এই গাইড সেই ১৪টিই অন্তর্ভুক্ত করেছে।
2. এই নথিতে ২০২৬ সালের challenge-গুলো সম্পর্কে বলা হয়েছে—২০২৫ সালের তালিকা নয়।
3. Challenge page-এর brief সংক্ষিপ্ত হতে পারে; Resources tab-এ dataset বা অতিরিক্ত ব্যাখ্যা থাকতে পারে।
4. সম্ভাব্য feature ও project workflow সহায়ক পরামর্শ, NASA-র বাধ্যতামূলক নির্দেশনা নয়।
5. event date, deadline, judging, award, registration ও submission policy-এর জন্য official event/local event page-ই চূড়ান্ত উৎস।
