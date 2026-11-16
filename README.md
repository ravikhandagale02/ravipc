# प्रगती दर्पण — योजनांचा नकाशा (10-11-2026)

## प्रती
1. **वेबसाइट (मुख्य शेअर लिंक) — https://ravikhandagale02.github.io/ravipc/** — पासवर्ड स्क्रीन (पासवर्ड `_build\hosted_gate.json` मध्ये; रविने 27-10 बदलून दिला).
   - रविचे GitHub account **ravikhandagale02** ("ravipc" नावाचे GitHub account दुसऱ्याचे — रविचे नाही). Repo `ravikhandagale02/ravipc` (Public); GitHub Pages: Deploy from branch `main`, `/ (root)`. Built-in browser मध्ये रविचे GitHub sign-in टिकलेले आहे (04-11 तपासले).
   - Repo मध्ये: `index.html` (वेबसाइट build — `out/site/index.html`) + `data/dr_*.js` (34). ⚠ लॅपटॉपची `प्रगती_दर्पण.html` कधीही अपलोड करू नये (पासवर्ड नाही, शीट IDs उघडे).
   - लॅपटॉप फाईलसारखीच: थेट 34 शीट्स, उपग्रह, CSV, पूर्ण/इतर योजना, 📍, पृष्ठजल, लाभक्षेत्र मोजणी, 📌/🧭, सादरीकरण; योजनांची माहिती व शीट IDs encrypted (`{"r","s"}`); noindex. शीटमधील बदल पुढच्या उघडण्यावर/⟳ ने आपोआप — Claude credit नाही (0–25 % योजनांचे नाव/किंमत शीटमध्ये बदलू नये — जुळवणी key).
   - 27-10 खरी तपासणी: एकूण 9850 योजना — ० % 2111 | १–५ % 200 | ६–१० % 187 | ११–२५ % 325 | इतर प्रगतीपथावरील 2313 | पूर्ण 4714; नकाशावर 9830.
   - नकाशात (template) बदल झाल्यास: build → नवीन `index.html` repo मध्ये अपलोड (https://github.com/ravikhandagale02/ravipc/upload/main). Claude कडे GitHub connection नाही — रविने फाईल drag करायची (built-in browser मध्ये upload पान उघडून Claude commit करू शकतो). Live site मध्ये सध्या फक्त 📍 आहे (04-11 तपासले); पृष्ठजल / लाभक्षेत्र / 📌 / सादरीकरण असलेली नवी `index.html` अपलोड बाकी.
2. **लॅपटॉप फाईल (रविची स्वतःची, पासवर्ड नाही)** — `software\PRAGATI DRSHAN\प्रगती_दर्पण\प्रगती दर्पण\प्रगती_दर्पण.html` + `data\` (34). जुनी प्रत `MWWC Office work\प्रगती दर्पण (नकाशा)\`. शीट IDs उघडे — शेअर/अपलोड करू नये.
   - Build kit: `software\PRAGATI DRSHAN\_build\` (template.html, assemble.py, gate.html, gate.js, hosted_gate.json, kml_build.py, kml_icons.js, assemble_data.py, build_data.py, match_all.py, talukas.py, common.py, drain_build.py, sheets.json, talukas_topo.json, taluka_name_map.csv).
   - `HOSTED` build flag (template `false`; फक्त Claude-लिंक build मध्ये `true`). `RetryTile` (3 वेळा + Esri backup host). `rad()` = 5 / 7 / 11.5 / 13 / 15.
3. **Claude लिंक (Artifact, जुनी)** — https://claude.ai/artifact/3pn66LDW5VJdZzShYrKAyR — public, पासवर्ड स्क्रीन, उपग्रह/थेट शीट नाही, 0–25 % snapshot (republish केलेली नाही). वेबसाइट वापरायची.

## सादरीकरण — वेगळी शीट / Excel नकाशावर (09-11)
- रवि: साहेबांनी "१ कोटीखालील योजना", "दुष्काळग्रस्त भाग" असे विचारल्यास वेगळ्या रचनेची शीट बनवून ती जोडून / अपलोड करून नकाशावर दाखवायची; **नेहमीचा (default) नकाशा = 34 जिल्हा शीट्स**.
- डावीकडे सर्वात वर "नकाशावरील माहिती": `#dsSel` (मूळ नकाशा + जतन सादरीकरणे), ➕ नवीन शीट / फाईल, ⛶ पूर्ण स्क्रीन; सादरीकरण उघडे असताना ⟳ ताजी (फक्त शीट), ⚙ कॉलम, 🔗 लिंक (फक्त शीट), 🗑 (दोनदा दाबल्यावर). नकाशावर crumb खाली "📊 नाव ✕ मूळ नकाशा".
- स्रोत: Google Sheet लिंक (Share → "Anyone with the link" → Viewer; लिंकमधील `gid` चा टॅब; gviz JSONP `select *`, `headers=1`; वर शीर्षक ओळ असल्यास `headers=1+skip` ने पुन्हा वाचते कारण संख्येच्या कॉलममधील header मजकूर Google null करते) किंवा Excel/CSV (`.xlsx/.xls/.ods` साठी SheetJS 0.18.5 cdnjs वरून — इंटरनेट लागते; CSV ऑफलाइन, "CSV UTF-8"). शीर्षक ओळ → सादरीकरणाचे default नाव. "एकूण/total" ओळी (Google ने मजकूर null केलेल्या सुद्धा) वगळल्या जातात.
- स्थान (आपोआप ओळख, ⚙ ने बदल): ① Lat/Long कॉलम (एकाच "Lat-Long" कॉलममध्ये दोन्हीही चालतात) → बिंदू; ② योजनेचे नाव (+ किंमत) मूळ यादी `S` शी जुळवून (key = `nk(नाव)|किंमत 2 दशांश`, नसल्यास एकमेव नाव / जिल्हा / तालुका) → बिंदू; ③ तालुका नाव → तालुके रंगवले (रंगीत तालुक्यांवर नावे); ④ जिल्हा नाव → जिल्हे रंगवले. मराठी/English/जुनी नावे (Ahmednagar, Aurangabad, Osmanabad, बुलडाणा…) ओळखतात; खेड, कर्जत, आष्टी, कळंब, मालेगाव, कारंजा — जिल्हा कॉलम लागतो. स्थान न सापडलेल्या नोंदी यादीत "स्थान नाही".
- रंग: ≤१२ मूल्यांचा मजकूर कॉलम (स्थिती/दुष्काळ/श्रेणी… आधी; गंभीर-लाल, मध्यम-नारंगी, सौम्य-पिवळा, पूर्ण-हिरवा, प्रगतीपथावर-जांभळा, अपूर्ण-लाल), नाहीतर किंमत/संख्या → ५ गट (quantile, गोलाकार कडा); "एकच रंग" पर्याय. बेरीज कॉलम (किंमत/रक्कम/क्षेत्र/संख्या; पूर्णांक असल्यास दशांश नाही).
- बाजूला: रंगनिहाय नोंदी + बेरीज (चेकबॉक्स), मंडळ/जिल्हानिहाय (जिल्हा निवडल्यावर तालुकानिहाय) गोषवारा, यादी (क्लिक → नकाशावर कार्ड), "ही यादी CSV". शोध पेटी सादरीकरणात त्या यादीत शोधते. मंडळ/जिल्हा/तालुका निवड सादरीकरणाच्या संख्यांनुसार. नकाशा legend, 📍 जवळच्या नोंदी, 📌 जवळची नोंद — सादरीकरणानुसार. सादरीकरणात ड्रेनेज फिकट, बिंदू मोठे (≥7 px).
- जतन: LS `pd_ds` = [{id, title, src:{type:'sheet',id,gid}|{type:'file',name}, map}] (map मध्ये कॉलम क्रमांक + `hn` कॉलम नावे — शीटमध्ये कॉलम हलवले/वाढवले तरी चालते). फाईलची माहिती LS `pd_dsr_<id>` (या डिव्हाइसवरच; नसल्यास "फाईल पुन्हा निवडा", तेच settings). शीट-सादरीकरणे दर वेळी थेट वाचली जातात.
- 🔗 लिंक: `वेबसाइट#ds=<base64url {t, s, m}>` (लॅपटॉप फाईलमधूनही वेबसाइटची लिंक). उघडणाऱ्याला पासवर्ड लागतो; उघडल्यावर त्याच्या डिव्हाइसवर जतन होऊन दिसते. लिंकमध्ये त्या सादरीकरण शीटचा ID असतो (34 जिल्हा शीट्सचे नाही).
- Claude लिंक (HOSTED) build: फक्त फाईल; शीट लिंक, 🔗, CSV नाहीत.
- कोड: template मधील `/* ===== सादरीकरण (presentation) ===== */` भाग (live-data भागानंतर, "misc" आधी); `let DS, HDRSUB0, HDRINFO0, SVER` वर (`st` नंतर). Hooks: `fillSelects`, `drawPoints`, `renderSide`, `renderMapLegend` (→ `dsRender`), `tipHTML` (→ `dsTip`), `renderCrumb`, `nearList/nearHTML`, `pinHTML`, `setBase` (→ `dsDraw`), `doSearch/pick`, `applyLive` (`SVER++`, header), `drainStyle`, `liveBtn`. `legExtras()` = पृष्ठजल + ड्रेनेज legend (दोन्ही legend मध्ये).
- तपासणी (Playwright, 09-11): शीर्षक ओळीची शीट + Lat-Long, नाव+किंमत जुळवणी, दुष्काळ तालुके (मराठी/English/जुनी नावे), CSV जिल्हा संख्या, दोन शीटची Excel + "Lat-Long" कॉलम, खाजगी शीट संदेश, reload, फाईल पुन्हा निवडणे, 🗑, फोनवर 🔗 लिंक + पासवर्ड — सर्व ठीक; जुन्या सर्व चाचण्या ठीक.

## साधने — डावीकडे "साधने" भाग (10-11; रविने सुचवलेल्या ६ पैकी "सर्व" मागितल्या)
- **📋 बाकी माहिती:** सर्व 34 शीट्सचे Ongoing + Complete (`select A,C,D,G,I,J,K,L`, 68 विनंत्या, १० मिनिटे cache) → जिल्हानिहाय Lat-Long / MHUID / GIS Mapping / जलदर्पण बाकी (Complete/Submitted नसलेले = बाकी; A रिकामी = एकूण ओळ, वगळली). जिल्हे "बाकी %" नुसार रंगवले; जिल्हा कार्डवर ⬇ बाकी यादी CSV, 💬 WhatsApp संदेश (`wa.me/?text=`, शीट लिंकसह), 📋 कॉपी. HOSTED मध्ये नाही.
- **📈 प्रगती बदल:** `s.p0` (फाईलमधील मूळ प्रगती, META.asof) किंवा मासिक नोंद (LS `pd_snap`, महिन्यात पहिल्यांदा live आल्यावर `snapSave()`, शेवटचे ८ महिने, डिव्हाइसनिहाय) विरुद्ध आताची. गट: ० % वरून सुरू झाली / पुढे सरकली / घटली (तपासा) / बदल नाही (सुरुवातीला बंद). फक्त ०–२५ % यादीतील योजना.
- **🖨 अहवाल (PDF):** `toolPrint()` → `#printRep` (नकाशा चित्र = vector canvas + नावे; उपग्रह चित्र येत नाही) + legend + गोषवारा + यादी (≤3000) → `window.print()`; A4, समास ~4 mm, header ओळी प्रत्येक पानावर, "पान x / y" (रविच्या PDF नियमांनुसार). सादरीकरण / साधन-यादी उघडी असल्यास तिचा अहवाल.
- **🚗 दौरा:** योजना / नोंद कार्डवर "➕ दौरा"; LS `pd_tour`; क्रमांकित निळे ठिपके + तुटक रेषा; ↕ जवळच्या क्रमाने (📍 चालू असल्यास तिथून), 🧭 Google Maps मार्ग (waypoints, पहिली १०), 📋 यादी / शेअर.
- **📝 नोंदी शीट + ⚠ अडचणी:** एक Google Form Responses शीट (कॉलम: योजनेचे नाव, शेरा, अडचण, फोटो, [किंमत, जिल्हा, दिनांक]) — LS `pd_notes` {sheet, form} (build मध्ये कायम करायचे असल्यास `META.notes`). नाव (+किंमत/जिल्हा) `matchS` ने जुळवून योजना कार्डवर "क्षेत्रीय नोंदी" (Drive फोटो thumbnail), "📝 शेरा" → Form (`{name}` `{district}` `{taluka}` `{cost}` placeholders, नसल्यास नाव कॉपी). ⚠ अडचणी = अडचणीनुसार रंगवलेली यादी. **रविने अजून Form / शीट बनवलेली नाही** — लिंक मिळाल्यावर `META.notes` मध्ये टाकल्यास सर्व पाहणाऱ्यांना दिसेल.
- कोड: `/* ===== साधने (work tools) ===== */` भाग (सादरीकरण भागानंतर). बाकी माहिती / प्रगती बदल / अडचणी = सादरीकरण यंत्रणेतील built-in यादी (`cfg.builtin`, `cfg.extra`, `cfg.off`, `cfg.note`, `mp.fix` ठराविक रंग; `builtinShow()`), `#dsSel` मध्ये "🛠 …". Playwright (10-11): सर्व ६ + जुन्या चाचण्या ठीक.

## सुविधा (वरून खाली बटणे: साधा·रस्ते·उपग्रह, ड्रेनेज, पृष्ठजल, +/−, 📍, लाभक्षेत्र, 📌)
- **📍 माझे ठिकाण (28-10):** `watchPosition`; निळा DOM ठिपका + accuracy; जवळच्या ५ योजना popup → कार्ड. Claude लिंकवर नाही.
- **पृष्ठजल (04-11):** JRC Global Surface Water occurrence tiles `https://storage.googleapis.com/global-surface-water/tiles2021/occurrence/{z}/{x}/{y}.png` (`RetryTile`, maxNativeZoom 13, opacity .85, zIndex 5) — १९८४–२०२१ (गुलाबी कधीकधी → निळा कायम). `st.sw` / LS `pd_sw` (default बंद), legend gradient. Claude लिंकवर नाही.
- **लाभक्षेत्र / क्षेत्रफळ मोजणी (04-11):** रविच्या मित्राचा video = MRSAC geoportal (Cadastral + गाव search + satellite + ArcGIS area measurement, Hectares). आपले tool: कोपरे टॅप; हे. + एकर, परिमिती; ↶ मागे / ✔ पूर्ण (पहिला कोपरा / double-click) / नवीन / निर्देशांक कॉपी; कोपरे ओढून बदल; मोजताना क्लिक = कोपरा (`measureClick`). Geodesic (1 km² ≈ 100.2 हे.). सर्व builds मध्ये. जतन नाही.
- **📌 ठिकाण चिन्हांकित + 🧭 मार्ग (04-11, रवि: "Google Maps सारखे — ठिकाण मार्क करून दिशा"):** पिन बटण → नकाशावर टॅप; उजवे-क्लिक / लांब दाबूनही; लाल पिन ओढता येतो; popup: lat,lon, तालुका व जिल्हा (`whereIs` → template मधील `polyIn`), 📍 चालू असल्यास सरळ अंतर, जवळची योजना; 🧭 मार्ग = Google Maps directions `https://www.google.com/maps/dir/?api=1&destination=LAT,LON&travelmode=driving` (फोनवर Google Maps app, turn-by-turn), 📤 शेअर (`navigator.share`, नसल्यास कॉपी), 📋 कॉपी, ✖ काढा; LS `pd_pin` (reload नंतर टिकतो, popup न उघडता). योजना कार्डच्या तळाशी "🧭 मार्ग" बटण + "Google Maps ↗". ⚠ template मध्ये `ringIn(ring,x,y)` आधीपासून आहे — त्याच नावाचे दुसरे function लिहू नये (hoisting मुळे शेवटचे जिंकते).
- **समोच्च रेषा (11-11, रवि: "शक्य तितक्या लहान अंतराच्या contours"):** `CTL` = `L.GridLayer` — AWS Terrarium उंची tiles (`https://s3.amazonaws.com/elevation-tiles-prod/terrarium/{z}/{x}/{y}.png`, SRTM ~30 m, native z13) वरून browser मध्येच रेषा काढते; अंतर `ctInt(z)`: 200 / 100 / 50 / 20 / 10 मी., z≥15 ला 5 मी. (interpolated — अंदाजे); दर ५ वी रेषा जाड. `st.ct` / LS `pd_ct`; "समोच्च" बटण (पृष्ठजल खाली); legend मध्ये चालू अंतर; 📌 popup मध्ये उंची (`elevAt`). साध्या नकाशावर पृष्ठजल / समोच्च चालू असताना जिल्हा fill पारदर्शक (`tileOv()`) — आधी पृष्ठजल साध्या नकाशावर पांढऱ्या fill खाली झाकले जात होते. HOSTED मध्ये नाही. ⚠ खऱ्या AWS tiles वर Claude च्या कार्यक्षेत्रातून तपासता आले नाही (नेटवर्क बंद) — फक्त नमुना tile वर चाचणी.
- **Cadastral (गट) layer:** MRSAC सेवा फक्त त्यांच्या geoportal proxy मधून — जोडता येत नाही.
- **भूजल — जोडले नाही (04-11):** CGWB Maharashtra GWRA 2023 (353 तालुके: Safe 277, Semi-critical 57, Critical 9, Over-exploited 9, Saline 1) व 2024 (359 तालुके, stage 52.99 %) अहवालांत फक्त संख्या; तालुकानिहाय यादी फक्त IN-GRES (उघडले नाही). Bhuvan Bhujal ला disclaimer (केले नाही). रविकडून IN-GRES Excel मिळाल्यास — आता सादरीकरणातूनच (तालुका + श्रेणी कॉलम) रंग-नकाशा होईल.

## Deploy स्थिती (10-11)
- नवी लॅपटॉप फाईल व वेबसाइट `index.html` (साधने + सादरीकरण + आधीचे सर्व) 10-11 ला chat मध्ये पाठवल्या (कॉम्प्युटर bridge शी जोडलेला नव्हता). रविने: लॅपटॉप फाईल दोन्ही ठिकाणी बदलायची; `index.html` GitHub upload पानावर drag करून Commit.
- `_build\template.html` कॉम्प्युटरवर अजून जुना (04-11) — पुढच्या वेळी कॉम्प्युटर जोडल्यावर बदलायचा (नवा template Claude च्या कार्यक्षेत्रात `pmap/template.html`; जुन्या प्रती template_v8pre_pres.html इ.).

## Build
- `python3 assemble.py out/pragati.html out/hosted/index.html out/site/index.html` → लॅपटॉप / Claude लिंक / वेबसाइट. वेबसाइटसाठी `out/site/data/` = `out/data/*.js`.
- पासवर्ड: hosted_gate.json (password, salt, iterations 200000); trim + lowercase; salt बदलू नये.
- App script `function PD_BOOT(){...}`; placeholders `<!--__GATE__-->`, `/*__START__*/`; gate.js payload array (Claude लिंक) किंवा `{"r","s"}` (वेबसाइट).

## माहितीचा स्रोत — 34 जिल्हा शीट्स
- Drive folder `15K_n2Psg5XxY-IWTbmlr1ULLe3cXpBoQ` = `<जिल्हा>_योजना_स्थिती` शीट्स (sheets.json मधील IDs; "anyone with the link can edit"). Tabs: गोषवारा, Complete, Ongoing, hidden RedList, प्रगती_नवीन, Q-R जुना बॅकअप, पिवळी_यादी, प्रगती_0-25.
- कॉलम: A अ.क्र., B प्रकार, C नाव, D तालुका, E जिल्हा, F प्र.मा. किंमत, G MHUID Status, H MHUID Number, I GIS Mapping, J Latitude, K Longitude, L Jaladarpan, M Impact, N Command Area Map, O Salient Features, P Catchment Map, Q.. प्रगती कॉलम.
- Live query: `select A,B,C,D,F,J,K,G,H,I,L where J is not null` (Ongoing + Complete) + hidden `प्रगती_0-25`. जुळवणी key = नाव (spaces/ZWJ काढून, NFC) | किंमत (2 दशांश).
- 0–25 % यादीत न जुळणाऱ्या, Lat-Long असलेल्या योजना: Complete → **पूर्ण योजना** (#1b9e77 हिरवा), Ongoing → **इतर प्रगतीपथावरील योजना** (#5e3c99 जांभळा).

## KML — बंद विषय
- 27-10 KMZ/KML बनवून दिल्या. **रवि: "KML/KMZ बद्दल विचार थांबवा" — पुढे काहीही सुचवू/करू नये** (रवि स्वतः मागेल तरच).

## Legends
- भौतिक प्रगती: ० % (#67000d), १–५ % (#d7301f), ६–१० % (#f78c1e), ११–२५ % (#eee24a), इतर प्रगतीपथावरील (#5e3c99), पूर्ण (#1b9e77); संख्या + प्र.मा. किंमत. कामनिहाय: 11 गट, चित्र-बॅज. पृष्ठजल gradient. ड्रेनेज.

## ड्रेनेज रेषा
- रविची 16_DEC.rar → Drainage_Maha.shp (1,311,364 रेषा; ORDER_ 1–10). क्रम 5+ HTML मध्ये; 1–4 जिल्हानिहाय data/*.js.

## पुढे शक्य
- भूजल तालुका रंग-नकाशा (IN-GRES Excel मिळाल्यास — सादरीकरणात थेट).
- लाभक्षेत्र आखलेले बहुभुज केंद्रीय जतन (शीट / Apps Script) — रविचा निर्णय नाही.
- फोटो कॉलम नाही; शीटमध्ये फोटो लिंक कॉलम जोडल्यास popup मध्ये दाखवता येईल.
