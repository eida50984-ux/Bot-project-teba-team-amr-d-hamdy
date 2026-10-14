[PowerWise Egypt](#top)

[Foundations](#foundations)[Components](#components)[Mobile screens](#screens)[Tablet & desktop](#layouts)[Specs & tokens](#specs)

# PowerWise Egypt

مراقبة ذكية لاستهلاك الكهرباء

The complete UI kit for an AI electricity monitor built for prepaid meter users in Egypt. Arabic RTL first, mobile first, with tablet and desktop layouts, a component library and design tokens. Everything on this page is live, so the theme switch restyles every screen.

Arabic RTL firstMobile firstLight & darkMaterial 3 · HIG · Fluent23 screens & states

[See the screens](#screens) [Design tokens](#specs)

## Foundations

A calm, premium base: electric blue for action, green for savings, energy yellow for attention. Neutrals lean slightly blue so cards, charts and the glass surfaces share one temperature.

### Color palette

Swatches use the live tokens, so toggling the theme shows the dark values. Text on tinted fills always uses the matching `-ink` variant to keep contrast at 4.5:1 or better.

Aa**Electric Blue**`primary`#1F5BFF · dark #5B8CFF\
Actions, links, active states

Aa**Savings Green**`secondary / success`#0E9F6E · dark #34D399\
Savings, success, healthy balance

Aa**Energy Yellow**`accent`#FFC21A · dark #FFD24D\
Highlights, scan frame, AI sparks

Aa**Warning Orange**`warning`#F58A07 · dark #FFA23A\
Low balance, high usage

Aa**Danger Red**`danger`#E5383B · dark #FF6B6B\
Errors, abnormal consumption

Aa**Background**`background`#F3F6FC · dark #070B14

Aa**Surface**`surface`#FFFFFF · dark #0F1626\
Cards, sheets, inputs

Aa**Surface variant**`surface-variant`#E9EEF8 · dark #172036\
Segmented controls, skeletons

Aa**On surface**`on-surface`#0A1226 · dark #EAF0FF

Aa**On surface variant**`on-surface-variant`#47536E · dark #A3B0CE

Aa**Brand gradient**`gradient.brand`135° #1F5BFF → #0B8A63\
Balance card, splash, AI badge

glass**Glass**`glass`16% white fill, 30% white edge, 10px blur. Only over the gradient.

### Typography

Cairo carries Arabic and Latin text in the Arabic UI. Inter carries the English locale and every meter reading and money figure, set with tabular figures so digits never jitter while they animate. Arabic never gets letter-spacing, italics or uppercase.

#### CAIRO · ARABIC UI · 400 500 600 700 800

الرصيد الحالي

أ ب ت ث ج ح خ د ذ ر ز س ش ص ض ط ظ ع غ ف ق ك ل م ن ه و ي — IBM Plex Sans Arabic is the approved fallback.

#### INTER · ENGLISH UI + NUMERALS · 400 500 600 700

184.50

Current balance · kWh · EGP · 0123456789 · tabular figures on for all readings.

#### TYPE SCALE · SIZE / LINE HEIGHT · WEIGHT

| ROLE | ARABIC · CAIRO | ENGLISH · INTER | SPEC |
| --- | --- | --- | --- |
| Display | وفّر كهرباءك | Save power | `40 / 48 · 800` |
| Meter figure | 184.50 ج.م · EGP | `44 / 48 · Inter 700` |  |
| Headline | تحليل الاستهلاك | Usage analysis | `28 / 36 · 800` |
| Title | رصيدك يكفي 13 يوماً | Balance lasts 13 days | `20 / 28 · 700` |
| Body large | اشحن قبل 25 أكتوبر لتجنب الانقطاع. | Recharge before 25 Oct to avoid a cut-off. | `16 / 27 · 500` |
| Body | استهلاك اليوم أعلى من المتوسط. | Today is above your average. | `14 / 24 · 500` |
| Label | ك.و.س · ج.م | kWh · EGP | `12 / 18 · 600` |

Numerals: Western digits (0–9) by default for readings and money, matching the digits on Egyptian prepaid meters. Eastern Arabic digits are available as a locale option and never mix with Western digits in one figure.

#### SPACING · 4 PT BASE

space-1 · 4

space-2 · 8

space-3 · 12

space-4 · 16

space-5 · 20

space-6 · 24

space-8 · 32

space-10 · 40

space-12 · 48

space-16 · 64

Screen margin 16 · card padding 14–20 · gap between cards 12 · minimum touch target 48 × 48.

#### RADIUS & ELEVATION

8

12

16

22

28

full

elev-1

elev-2

elev-3

Buttons 16 · inputs 14 · cards 22 · balance card 26 · sheets and dialogs 28. Shadows are soft and blue-tinted, never grey.

### Icon guidelines

One outline family, drawn on a 24 px grid with a 2 px safe margin, 1.75 px stroke and round caps and joins. Active navigation icons sit on a tinted pill instead of switching to a filled glyph. Core set first, then the appliance set.

**Electricity**كهرباء

**Home**الرئيسية

**Devices**الأجهزة

**Balance**الرصيد

**Camera**الكاميرا

**AI**الذكاء الاصطناعي

**Analytics**التحليلات

**Settings**الإعدادات

**Notifications**الإشعارات

**Reports**التقارير

**Recharge**الشحن

**Warnings**التحذيرات

**Air conditioner**تكييف

**Refrigerator**ثلاجة

**Television**تلفزيون

**Washing machine**غسالة

**Fan**مروحة

**Heater**دفاية

**Microwave**ميكروويف

**Kettle**غلاية

**Iron**مكواة

**LED bulb**لمبة LED

**Normal bulb**لمبة عادية

**Router**راوتر

**Laptop**لابتوب

**Computer**كمبيوتر

**Water pump**طلمبة مياه

**Electric oven**فرن كهربائي

**Cooker**بوتاجاز كهربائي

#### ICON RULES

- **Sizes:** 20 in buttons and inputs, 22 in app bars and rows, 26 in tiles and the scan button, 54+ in illustrations.
- **Color:** inherit the text color. On tinted tiles use the paired `-ink` color, never the raw accent.
- **Mirroring:** back, forward, chevrons, progress and list arrows flip in RTL. Bolt, camera, charts, clocks, plugs and appliances never flip.
- **Meaning:** never rely on an icon alone for a state. Pair it with a label or a badge.

#### APPLIANCE TILES

- Each category sits on a 46 px rounded tile: cooling in blue, kitchen in orange, lighting in yellow, network in green, motors and entertainment in grey.
- Users can replace the icon with a photo of their own appliance. Photos crop to the same 16 px radius and keep the category tile as a fallback.
- Every appliance icon is single-weight line art, readable at 20 px.

### Accessibility

#### VISUAL

- **Contrast:** 4.5:1 for text, 3:1 for icons, borders of controls and chart marks. Both themes are checked.
- **Not color alone:** usage levels pair color with a label (*normal*, *high*, *abnormal*) and an icon.
- **Type:** body text scales to 200% without clipping. Arabic keeps a 1.7 line height so diacritics never collide.
- **Glass:** only used over the brand gradient, with white text at 4.5:1 or better.

#### INTERACTION

- **Targets:** at least 48 × 48 dp. Chips and small buttons are 34–40 dp tall with extended hit areas.
- **Screen readers:** every icon button has an Arabic label. Charts expose a one-line summary, for example “Usage this week, highest on Wednesday, 9.4 kWh”.
- **Focus:** a 3 px blue ring with 2 px offset on keyboard and switch-access focus.
- **Motion:** every animation has a still end state and turns off with “reduce motion”. Nothing flashes more than 3 times per second.
- **OCR flow:** manual entry is always one tap away from the camera, with the same validation.

## Component library

Every reusable piece, drawn in RTL on the app background. The controls respond to hover, press and focus; the toggles and segmented tabs work.

#### BUTTONS

52 px tall, radius 16, Cairo 700 16. Press scales to 97% in 120 ms.

#### INPUTS

البريد الإلكتروني

رقم الهاتف

+20

كلمة المرور

8 أحرف على الأقل

رقم العداد

#### DROPDOWN · SELECT

المحافظة

القاهرة

القاهرة

الجيزة

الإسكندرية

الدقهلية

#### SELECTION · SWITCH · CHECKBOX · SEGMENTED · CHIPS · RADIO CARDS

**الإشعارات**

**تذكرني**

الكلتبريدمطبخإضاءة

**عداد كارت**مسبق الدفع

**عداد فوترة**فاتورة شهرية

#### CARDS

**استهلاك اليوم**أعلى من المتوسط

9.4 ك.و.س

**تكييف**1,200 واط108 kWh

**ثلاجة**150 واط43 kWh

الرصيد الحالي

184.50ج.م

Plain cards hover up 3 px with elevation-2. The balance card is the only surface that uses the gradient.

#### BADGES · PROGRESS · GAUGE

طبيعيمرتفعغير معتادجديدAI

الشريحة الحالية**112 / 200**

اقتربت من حد الشريحة**91%**

تجاوزت الحد**104%**

**13**يوم

**6**أيام

**2**يومان

Gauge colors follow days left: green above 7, orange 3–7, red under 3.

#### DIALOG

##### حذف الجهاز؟

سيتم حذف «تكييف» وسجل استهلاكه. لا يمكن التراجع.

#### BOTTOM SHEET

**إضافة جهاز**

تكييف

ثلاجة

غلاية

آخر

#### SNACKBARS · TOOLTIP

تم حفظ القراءة**تراجع**

تعذّر الاتصال بالخادم**إعادة**

هذه القدرة بالواط من ملصق الجهاز

لمسة طويلة تُظهر التلميح

#### NAVIGATION · APP BAR · BOTTOM NAV · FAB

# تفاصيل الجهاز

#### LOADING · SKELETON

#### CHARTS · LINE · BAR · DONUT · SPARKLINE

**الاستهلاك اليومي**ك.و.س

**مقارنة شهرية**ك.و.س

**توزيع الطاقة**240 ك.و.س

**45%**تكييف

تكييف*45%*

ثلاجة*18%*

طلمبة*12%*

تلفزيون*8%*

أخرى*17%*

### Micro-animations

Each effect ends on a visible resting state. Durations: 120 ms press, 200 ms hover and toggles, 450 ms page transitions, 800–1200 ms data reveals. Easing: `cubic-bezier(.2,.8,.2,1)` for entrances, linear for loops.

**مرّر الفأرة**

**Card hover**Lift 3 px, elevation 1 to 2 · 200 ms

**Button press**Scale to 97%, shadow tightens · 120 ms

**Chart animation**Line draws right to left in RTL · 1.2 s

الرئيسية

الأجهزة

**Page transition**Forward slides in from the left in RTL · 450 ms

**Loading**Spinner for actions, shimmer skeleton for screens

184.50

**Balance animation**Count up with tabular figures · 900 ms

**AI scanning**Light bar sweeps the frame while OCR runs · 1.6 s loop

## Mobile screens

Every screen at 300 × 660, drawn right to left. Money and readings use sample data for a household in Cairo with a card meter: 184.50 EGP left, about 13 days at today's pace. Scroll each row sideways.

### Onboarding

Splash, login, and registration split into two short steps so each screen fits one thumb: account first, then address and meter. Meter number can be read from a photo.

9:41

# PowerWise Egypt

مراقبة ذكية للكهرباء

SMART ELECTRICITY MONITORING

v1.0

Splash

9:41

**PowerWise Egypt**

## أهلاً بعودتك

سجّل الدخول لمتابعة استهلاك الكهرباء

البريد الإلكتروني

name@example.com

كلمة المرور

••••••••

تذكرني

أو

ليس لديك حساب؟

Login

9:41

# إنشاء حساب

1 من 2

الاسم الكامل

أحمد سمير

رقم الهاتف

+2010 1234 5678

البريد الإلكتروني

name@example.com

كلمة المرور

8 أحرف على الأقل

تأكيد كلمة المرور

••••••

كلمتا المرور غير متطابقتين

Register · account

9:41

# بيانات العداد

2 من 2

العنوان

12 شارع النيل، المعادي

المحافظة

القاهرة

رقم العداد

4521 0098 7731

أو اضغط على الكاميرا لقراءته من الصورة

نوع العداد

**عداد كارت**مسبق الدفع، تشحن برصيد

**عداد فوترة**فاتورة شهرية

أوافق على الشروط وسياسة الخصوصية

Register · address & meter

### Home and devices

The balance card leads: current balance, days left on a tick-ring dial, and three glass chips. The AI line, quick actions and usage chart follow. Home scrolls; the mock shows the first screen.

9:41

أ

صباح الخير

# أحمد

الرصيد الحالي

184.50ج.م

رصيد يكفي حتى 27 أكتوبر

**13**يوم متبقٍ

*اليوم***9.4***ك.و.س*

*هذا الشهر***112***ك.و.س*

*التكلفة***168***ج.م*

**توقع الذكاء الاصطناعي**ينفد الرصيد حوالي 27 أكتوبر

[تصوير العداد](#)[إضافة جهاز](#)[التقارير](#)[نصائح التوفير](#)

**الاستهلاك**

الشريحة الحالية (101–200)**112 / 200**

Home dashboard

9:41

# أجهزتي

ابحث عن جهاز…

الكلتبريدمطبخإضاءةشبكة

**تكييف 1.5 حصان**1,200 واط108 ك.و.س/شهر

**ثلاجة**150 واط43 ك.و.س/شهر

**طلمبة مياه**750 واط29 ك.و.س/شهر

**تلفزيون LED**100 واط19 ك.و.س/شهر

**غلاية**2,000 واط14 ك.و.س/شهر

**راوتر**12 واط9 ك.و.س/شهر

Devices

9:41

# تكييف 1.5 حصان

صورة الجهاز

القدرة**1,200 W**

الاستهلاك اليومي**3.6 kWh**

التشغيل**3 h**

التكلفة اليومية

5.4 ج.م

التكلفة الشهرية

162 ج.م

**سجل التشغيل**ساعات / آخر 7 أيام

**اقتراح للتوفير**

اضبط الترموستات على 25° لتقليل الاستهلاك حتى 10% شهرياً.

Device details

### Meter photo and OCR

Five steps from viewfinder to result. The yellow frame, the sweep line and the reading itself are the only bright elements on the dark camera surface. Failure always offers manual entry beside the retry button.

9:41

ضع شاشة العداد في الإطار

PREPAID METER · 220V

184.50

Camera

9:41

PREPAID METER · 220V

184.50

**معاينة الصورة**اسحب الأطراف للقص

Preview & crop

9:41

PREPAID METER · 220V

184.50

**جارٍ قراءة الشاشة…**

**68%**

تحسين الصورة

تحديد أرقام العداد

التحقق من القراءة

Scanning · OCR progress

9:41

PREPAID METER

184.50

**تمت القراءة بنجاح**

دقة القراءة 98%

موثوقة

الرصيد المقروء

184.50

ج.م

Reading success

9:41

PREPAID METER

1 4.5

**تعذّرت قراءة الصورة**

الأرقام غير واضحة

**صوّر في إضاءة أفضل وتجنب الانعكاس**

**ثبّت الهاتف واملأ الإطار بالشاشة**

Reading failed

### Balance, analytics and AI

Balance answers “when do I need to recharge”. Analytics answers “where is it going”. The AI screen turns both into a score, warnings and next steps. Warnings use orange and a label; red is kept for abnormal consumption.

9:41

# الرصيد

الرصيد الحالي

184.50ج.م

**13**يوم متبقٍ

*آخر شحن***6 أكتوبر**

*ينفد في***27 أكتوبر**

*مصروف يومي***14.1 ج.م**

**توصية الشحن**

اشحن 200 ج.م قبل 25 أكتوبر لتفادي الانقطاع.

**آخر عمليات الشحن**

**6 أكتوبر**شحن كارت

**+300**

**21 سبتمبر**شحن كارت

**+250**

Balance

9:41

# التحليلات

اليوم**+16%**عن أمس

الشهر**−15%**عن سبتمبر

السنة**−6%**عن 2025

**توزيع الطاقة**240 ك.و.س

**45%**تكييف

تكييف*45%*

ثلاجة*18%*

طلمبة*12%*

تلفزيون*8%*

الأعلى**التكييف**

الأقل**الراوتر**

**مقارنة شهرية**ك.و.س

Analytics

9:41

# التحليل الذكي

AI

**78**من 100

جيد

درجة كفاءة استهلاكك

تحسنت 4 نقاط عن الأسبوع الماضي

موعد الشحن المتوقع**27 أكتوبر**

اتجاه صاعد +6%

**تحذير**

استهلاك التكييف أعلى 22% من المعتاد بين 2 و5 مساءً.

**مشكلة محتملة**

قد تنخفض كفاءة التكييف. ننصح بتنظيف الفلتر أو الصيانة.

**التوصيات**

**اضبط التكييف على 25°**

**شغّل الغسالة خارج ساعات الذروة**

AI analysis

### Notifications and settings

Alerts carry a tinted tile, a one-line action, and an unread dot. Settings keep the language choice and dark mode one tap away.

9:41

# الإشعارات

الكلالرصيدالاستهلاكالأجهزة

اليوم

**رصيد منخفض**الرصيد أقل من 200 ج.م. يُفضّل الشحن قبل 25 أكتوبر.

**استهلاك مرتفع**استهلاكك اليوم أعلى 16% من أمس.

**استهلاك غير معتاد**ارتفاع مفاجئ بين 2 و5 مساءً.

أمس

**تذكير بالشحن**موعد الشحن المقترح بعد 11 يوماً.

**تنبيه جهاز**التكييف يعمل منذ 9 ساعات متواصلة.

Notifications

9:41

# الإعدادات

أ

**أحمد سمير**

عداد كارت · 4521 0098 7731

**الملف الشخصي**

**اللغة**

**الوضع الداكن**

**الإشعارات**

**حول التطبيق**

**المساعدة**

**الخصوصية**

Settings

### Empty, loading, error and success states

Each state says what happened and offers the next action. Skeletons copy the layout of the screen they replace, so nothing jumps when data arrives.

9:41

# أجهزتي

## لا توجد أجهزة بعد

أضف أجهزتك لتعرف كم تستهلك كل منها وكم تدفع.

Empty

9:41

Loading · skeleton

9:41

أ

صباح الخير

# أحمد

## تعذّر تحميل البيانات

تحقق من اتصالك بالإنترنت ثم حاول مرة أخرى.

لا يوجد اتصال**إعادة**

Error

9:41

# تسجيل الشحن

## تم تسجيل الشحن

أُضيف 200 ج.م إلى رصيدك.

الرصيد الجديد

384.50 ج.م

يكفي حتى 10 نوفمبر

تم حفظ العملية**تراجع**

Success

## Wireframes and responsive layouts

Structure first, then the same content on larger windows. Navigation moves from a bottom bar on phones, to a rail on tablets, to a labelled sidebar on desktop. The first column always starts on the right.

### Wireframes

Low fidelity, ordered by what the user needs first. Dashed boxes are content regions, solid boxes are the primary object on the screen.

av

greeting

bell

Balance card · amount · days dial · 3 stats

AI prediction line

act

act

act

act

Usage chart · day / week / month · tier bar

nav

nav

scan

nav

nav

Home

title

+

search

all

cat

cat

cat

device

device

device

device

device

device

\+ add device

nav

nav

scan

nav

nav

Devices

x

hint

Viewfinder\
meter frame + corners

tip text

gallery

shutter

flash

Camera

‹

title

Balance · dial · recharge date · finish date · daily spend

Recharge recommendation + button

Recharge history list

nav

nav

scan

nav

nav

Balance

### Tablet · expanded window 1024 × 720

A navigation rail replaces the bottom bar. The balance column stays at 300 px; charts take the remaining width and the donut and device ranking sit side by side underneath.

[الرئيسية](#)[الأجهزة](#)[التحليلات](#)[الرصيد](#)[الإعدادات](#)

# لوحة التحكم

الأربعاء، 14 أكتوبرأ

الرصيد الحالي

184.50ج.م

يكفي حتى 27 أكتوبر

**13**يوم متبقٍ

*اليوم***9.4***ك.و.س*

*الشهر***112***ك.و.س*

*التكلفة***168***ج.م*

**توقع الذكاء الاصطناعي**ينفد الرصيد حوالي 27 أكتوبر

[تصوير العداد](#)[إضافة جهاز](#)[التقارير](#)[نصائح](#)

**نصيحة اليوم**

شغّل الغسالة والمكواة خارج ساعات الذروة لتقليل الشريحة.

**الاستهلاك اليومي**

**توزيع الطاقة**

**240**ك.و.س

تكييف*45%*

ثلاجة*18%*

طلمبة*12%*

تلفزيون*8%*

**أعلى الأجهزة استهلاكاً**

**تكييف**

**108**

**ثلاجة**

**43**

**طلمبة مياه**

**29**

### Desktop · large window 1440 × 900

A labelled sidebar and a KPI row put every number from the phone's balance card in one glance. The chart and the device table share the wide column; the AI summary and distribution live in a 400 px side column.

PowerWise Egypt

[الرئيسية](#)[الأجهزة](#)[التحليلات](#)[الرصيد](#)[التحليل الذكي](#)[الإشعارات](#)[الإعدادات](#)

**حدّث قراءة العداد**

ارفع صورة من الهاتف أو من الكمبيوتر.

# لوحة التحكم

ابحث عن جهاز أو تقرير…

أ

الرصيد الحالي**184.50 ج.م***يكفي 13 يوماً · حتى 27 أكتوبر*

استهلاك اليوم**9.4 ك.و.س***+16% عن أمس*

هذا الشهر**112 ك.و.س***المتوقع 240 · أقل 15% من سبتمبر*

التكلفة الحالية**168 ج.م***الشريحة 101–200 · 56%*

**الاستهلاك اليومي**

**الأجهزة الأعلى استهلاكاً**

| الجهاز | القدرة | الاستهلاك الشهري | التكلفة | الحصة |
| --- | --- | --- | --- | --- |
| **تكييف 1.5 حصان** | 1,200 W | 108 kWh | 162 ج.م |  |
| **ثلاجة** | 150 W | 43 kWh | 65 ج.م |  |
| **طلمبة مياه** | 750 W | 29 kWh | 44 ج.م |  |
| **تلفزيون LED** | 100 W | 19 kWh | 29 ج.م |  |

**78**من 100

التحليل الذكي

كفاءة استهلاكك جيدة

الشحن المتوقع: 27 أكتوبر

**تحذير**

استهلاك التكييف أعلى 22% من المعتاد بين 2 و5 مساءً.

**توزيع الطاقة**

**240**ك.و.س

تكييف*45%*

ثلاجة*18%*

طلمبة*12%*

تلفزيون*8%*

أخرى*17%*

Both frames are scaled previews of the real layouts. Scroll sideways on small screens.

### Layout grids and breakpoints

#### COMPACT · 4 COLUMNS · MARGIN 16 · GUTTER 16

#### MEDIUM · 8 COLUMNS · MARGIN 24 · GUTTER 16

#### EXPANDED · 12 COLUMNS · MARGIN 32 · GUTTER 24

| WINDOW | WIDTH (dp) | NAVIGATION | HOME LAYOUT | CARDS PER ROW |
| --- | --- | --- | --- | --- |
| **Compact** | `0–599` | Bottom bar with raised scan button | One column: balance, AI line, actions, chart | 1 (device cards 2) |
| **Medium** | `600–839` | Rail, 88 wide | Two columns: balance and AI left, charts right | 2 |
| **Expanded** | `840–1199` | Rail, 88 wide | 300 px balance column, chart, donut and ranking | 2–3 |
| **Large** | `1200+` | Sidebar, 248 wide | KPI row, wide column and 400 px side column | 4 KPIs, 2 columns |

Content stops growing at 1280. Charts keep their aspect ratio and add gridlines as they widen. Landscape phones use the medium layout without the rail labels.

## Specifications and tokens

Numbers a developer can build from, a Figma file structure that matches them, and the token set as JSON.

### Component specifications

| COMPONENT | SIZE | RADIUS | TYPE | BEHAVIOR |
| --- | --- | --- | --- | --- |
| **Top app bar** | `56 high · 16 side` | `icon buttons 14` | Cairo 700 18 | Title fills; back arrow mirrors in LTR |
| **Primary button** | `52 high · min 120` | `16` | Cairo 700 16 | Press 97% · 120 ms; loading keeps width |
| **Small button** | `40 high` | `12` | Cairo 700 14 | Inside cards and dialogs |
| **Text input** | `52 high` | `14` | Cairo 500 14, label 12/600 | Focus 2 px blue ring; error adds red ring and a hint line |
| **Card** | `padding 14–20` | `22` | Title 15/700 | Elevation 1; hover lifts 3 px |
| **Balance card** | `padding 16 · dial 92` | `26` | Inter 700 38 for the amount | Dial: 30 ticks, 260° sweep, fills on load |
| **Bottom navigation** | `72 high` | `24 top` | Cairo 600 10.5 | Active item sits on a 52 × 30 tinted pill |
| **Scan button** | `58 × 58` | `20` | Icon 26 | Raised 30 above the bar, gradient fill |
| **Chip** | `34 high (48 hit)` | `full` | Cairo 600 13 | Single select for filters |
| **Switch** | `48 × 28` | `full` | - | Thumb moves toward the end edge when on |
| **Bottom sheet** | `grabber 40 × 4` | `28 top` | Title 16/700 | Drag to dismiss; scrim 45% |
| **Dialog** | `max 340 · padding 20` | `28` | Title 17/700 | Cancel on the start side, destructive action on the end |
| **Snackbar** | `padding 12 / 14` | `14` | Cairo 600 13 | 4 s, one action, sits above the bottom bar |
| **Progress bar** | `8 high` | `full` | - | Fills from the start edge; turns orange at 90%, red at 100% |

#### FIGMA FILE STRUCTURE

```
PowerWise Egypt.fig
├─ Cover
├─ Foundations
│   ├─ Color        variables, modes: Light / Dark
│   ├─ Type         styles: AR Cairo, EN Inter, Numeric
│   ├─ Space & Radius
│   ├─ Elevation & Glass
│   ├─ Icons        24 px grid, core + appliance sets
│   └─ Motion       durations, easing curves
├─ Components     (variants: state, size, theme, direction)
│   ├─ Button · Input · Select · Switch · Chip
│   ├─ Card · Balance Card · Device Card
│   ├─ Navigation · App Bar · Bottom Nav · Rail · Sidebar
│   ├─ Overlay · Dialog · Bottom Sheet · Snackbar · Tooltip
│   └─ Charts · Line · Bar · Donut · Dial · Skeleton
├─ Wireframes
├─ Mobile · AR · Light
│   ├─ Onboarding · Core · Meter OCR · Money & AI · System
│   └─ States · Empty · Loading · Error · Success
├─ Mobile · AR · Dark
├─ Mobile · EN · Light      (auto-mirrored from AR)
├─ Tablet · 1024 · AR
├─ Desktop · 1440 · AR
├─ Prototypes     splash → login → home → scan → result
└─ Handoff        specs, tokens, accessibility notes
```

Frames use auto layout with start/end padding so a single component set serves both directions. Boolean property `rtl` mirrors icons that should flip.

#### DESIGN TOKENS · JSON

```
{
  "color": {
    "primary":          { "light": "#1F5BFF", "dark": "#5B8CFF" },
    "on-primary":       { "light": "#FFFFFF", "dark": "#04102E" },
    "secondary":        { "light": "#0E9F6E", "dark": "#34D399" },
    "accent":           { "light": "#FFC21A", "dark": "#FFD24D" },
    "warning":          { "light": "#F58A07", "dark": "#FFA23A" },
    "danger":           { "light": "#E5383B", "dark": "#FF6B6B" },
    "success":          { "alias": "secondary" },
    "background":       { "light": "#F3F6FC", "dark": "#070B14" },
    "surface":          { "light": "#FFFFFF", "dark": "#0F1626" },
    "surface-variant":  { "light": "#E9EEF8", "dark": "#172036" },
    "outline":          { "light": "#D9E1F0", "dark": "#243050" },
    "on-surface":       { "light": "#0A1226", "dark": "#EAF0FF" },
    "on-surface-variant": { "light": "#47536E", "dark": "#A3B0CE" }
  },
  "gradient": {
    "brand": { "angle": 135, "stops": ["#1F5BFF", "#0B8A63"] }
  },
  "font": {
    "family": { "ar": "Cairo", "en": "Inter", "mono": "JetBrains Mono" },
    "size":   { "label": 12, "body": 14, "body-lg": 16, "title": 20, "headline": 28, "display": 40, "meter": 44 },
    "weight": { "regular": 400, "medium": 500, "semibold": 600, "bold": 700, "black": 800 }
  },
  "space":  [4, 8, 12, 16, 20, 24, 32, 40, 48, 64],
  "radius": { "xs": 8, "sm": 12, "md": 16, "lg": 22, "xl": 28, "full": 999 },
  "size":   { "touch": 48, "button": 52, "button-sm": 40, "input": 52, "app-bar": 56, "bottom-nav": 72 },
  "shadow": {
    "1": "0 1px 2px rgba(10,18,38,.06)",
    "2": "0 8px 24px rgba(23,50,110,.12)",
    "3": "0 22px 56px rgba(23,50,110,.22)"
  },
  "motion": {
    "press": "120ms", "hover": "200ms", "page": "450ms", "reveal": "1000ms",
    "ease-out": "cubic-bezier(.2,.8,.2,1)"
  },
  "breakpoint": { "compact": 0, "medium": 600, "expanded": 840, "large": 1200 }
}
```

PowerWise Egypt design system. All balances, readings and prices are sample data for illustration.