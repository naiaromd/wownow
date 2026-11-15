# BIB Design System

**Beauty Innovation & Beyond**  
Version r02 · 20 July 2026 · Working Design System  
Companion to `BIB_Brand_Guideline_r04_20260720.md`

> ระบบนี้แปลง Brand Guideline ให้เป็นกติกาที่ทีมออกแบบและทีมการตลาดนำไปใช้ซ้ำได้ งาน final ทุกชิ้นต้องผ่าน font, logo, image-rights, claims และ commercial review

---

## 1. System Idea

**Clarity before story. Product before atmosphere. Proof before promise.**

งานของ BIB ต้องช่วยให้ผู้อ่านรู้ทันทีว่ากำลังดูอะไร เหมาะกับเขาอย่างไร และต้องตัดสินใจเรื่องใด ความพรีเมียมเกิดจาก hierarchy, spacing, quality of image และความชัดเจนของข้อมูล ไม่ใช่การใส่ concept หรือบรรยากาศให้ทุกชิ้น

### Design Principles

1. **Immediate clarity:** ภายในไม่กี่วินาทีต้องรู้ subject และสารหลัก
2. **Solution fit:** เริ่มจากบริบทธุรกิจ แล้วจึงเสนอ technology/commercial path
3. **Evidence anchor:** ทุกข้อความสำคัญมี proof, source cue หรือขอบเขตการกล่าวอ้าง
4. **Quiet confidence:** ไม่ใช้ decoration หรือคำเร่งขายแทนความน่าเชื่อถือ
5. **Human respect:** ภาพและภาษาไม่สร้างความรู้สึกว่าร่างกายหรือชีวิตต้องสมบูรณ์แบบ
6. **Story is optional:** เพิ่ม narrative เฉพาะเมื่อช่วยอธิบาย use case, experience หรือ brand belief

---

## 2. Foundation Tokens

### Color Tokens

| Token | Value | Role |
|---|---|---|
| `color.brand.graphite` | `#6F6F75` | Primary logo, heading, key label |
| `color.brand.taupe` | `#B8A086` | Connector, rule, premium accent |
| `color.ink.charcoal` | `#2F3033` | Body text, dark field |
| `color.surface.ivory` | `#F6F3EE` | Warm editorial canvas |
| `color.surface.white` | `#FFFFFF` | Clinical/evidence canvas |
| `color.story.blush` | `#E1C3B8` | Human/body story, ≤20% |
| `color.story.sand` | `#DBD189` | Warm editorial field, ≤15% |
| `color.story.mist` | `#D4DDDC` | Medical/recovery field, ≤25% |

**Default ratio:** 70% White/Ivory · 20% Graphite/Charcoal · 10% Taupeหรือ secondary เพียงหนึ่งสี

### Typography Tokens

| Token | Thai | English | Weight | Use |
|---|---|---|---:|---|
| `type.display` | Kanit | Muli | 300/400 | Editorial headline สั้น |
| `type.heading` | Kanit | Muli | 500/600 | Section heading, navigation |
| `type.body` | Kanit | Muli | 400 | Paragraph, explanation |
| `type.data` | Kanit | Muli | 400/500 | ราคา ตัวเลข ตาราง caption |

**Language rule:** ภาษาไทยทั้งหมดใช้ Kanit; ภาษาอังกฤษใช้ Muli งาน production ต้อง embed/package fonts ห้ามปล่อยให้ fallback เป็น final artwork Working assets อยู่ใน `1_icoone/Marketing/Brand Assets/Fonts/` พร้อม OFL

| Level | Print guide | Digital guide | Line height |
|---|---:|---:|---:|
| Display | 30–44 pt | 56–72 px | Thai 1.25–1.35 |
| H1 | 24–32 pt | 40–48 px | Thai 1.35 |
| H2 | 18–22 pt | 28–36 px | Thai 1.45 |
| H3 | 13–16 pt | 20–24 px | Thai 1.5 |
| Body | 9.5–11 pt | 16–18 px | Thai 1.7–1.85 |
| Caption | 6.5–8 pt | 12–14 px | Thai 1.6 |

### Spacing Tokens

ฐาน 8 px digital / 2 mm print: `1×, 2×, 3×, 4×, 6×, 8×, 12×`

- ภายใน component ใช้ 1×–3×
- ระหว่าง module ใช้ 3×–6×
- ระหว่าง editorial sections ใช้ 6×–12×
- ห้ามสร้างระยะใหม่หาก token ที่ใกล้ที่สุดแก้ปัญหาได้

### Border and Shape

- Hairline: 0.5–1 px digital / 0.2–0.35 mm print
- Accent connector: 3–5 px digital / 1–1.5 mm print
- Radius: 0 สำหรับ editorial print; 4–8 px สำหรับ UI ที่ต้องสื่อ interaction
- Shadow: ไม่ใช้ใน print; digital ใช้เฉพาะ elevation ที่มีหน้าที่ ไม่ใช้เพื่อทำให้ดู luxury

---

## 3. Logo Components

### Approved Working Assets

| Component | File | Use |
|---|---|---|
| `Logo/BIB/Positive` | `4_Media/Logo/BIB Logo.png` | White, Ivory และภาพสว่างที่มีพื้นที่สงบ |
| `Logo/BIB/Reversed` | `4_Media/Logo/BIB Logo white.png` | Deep Charcoal หรือภาพมืดที่ contrast ผ่าน |
| `Logo/icoone/LaserMed` | `4_Media/Logo/icoone laser med.png` | Product-specific communication |
| `Logo/icoone/Core` | `4_Media/Logo/icoone.png` | ใช้เมื่อไม่ต้องระบุรุ่นและได้รับอนุมัติ |
| `Logo/icoone/Gold` | `4_Media/Logo/icoone gold.png` | Reserved; ใช้เฉพาะ campaign ที่มี proof สีและ approval |
| `Logo/BIB/Positive-Trimmed` | `1_icoone/Marketing/Brand Assets/Derived/BIB_Logo_trimmed.png` | Production derivative สำหรับ co-brand header; ตัดเฉพาะ transparent canvas ภายนอก ไม่แก้ artwork |
| `Logo/icoone/LaserMed-Trimmed` | `1_icoone/Marketing/Brand Assets/Derived/icoone_LaserMed_trimmed.png` | Production derivative สำหรับ co-brand header; ตัดเฉพาะ transparent canvas ภายนอก ไม่แก้ artwork |

### Co-brand Header

ลำดับมาตรฐานสำหรับ proposal/leaflet:

`BIB logo | vertical taupe connector | product logo`

- Logo ทั้งสองมี optical height ใกล้กัน ไม่จำเป็นต้องกว้างเท่ากัน
- Term Sheet A4 ใช้ logo box เท่ากันที่ประมาณ 35 × 15 mm; BIB สูงไม่เกิน 15 mm และ icoone กว้างไม่เกิน 35 mm/สูงไม่เกิน 13.5 mm เพื่อให้น้ำหนักสายตาใกล้เคียงกัน
- หาก PNG master มี transparent canvas มาก ให้ใช้ approved trimmed derivative แทนการชดเชยด้วยการขยายแบบเดาสายตา ห้ามตัดเข้า artwork หรือ clear space ขั้นต่ำ
- ระยะจากโลโก้ถึง connector อย่างน้อย 1X
- ห้ามรวมเป็นไฟล์โลโก้ใหม่หรือเปลี่ยนสี partner logo ให้เข้ากับ BIB
- Product-led campaign ให้ product logo เด่นกว่า BIB ได้ไม่เกินประมาณ 1.25× ของ optical area

---

## 4. Image System

### Visual Modes

| Mode | Default use | Image rule | Story level |
|---|---|---|---:|
| **Direct Product** | Term sheet, quotation, product specification, proposal summary | รูปผลิตภัณฑ์จริงบน White/Ivory ไม่มีฉาก ไม่มีข้อความซ้อน | 0 |
| **Applied Solution** | Sales deck, case study, training, service model | Product + ผู้ใช้งาน/บริบทจริงที่ช่วยอธิบาย workflow | 1 |
| **Brand Editorial** | Corporate campaign, thought leadership, brand film | Human/environment narrative ที่มี thesis และ proof รองรับ | 2 |

เริ่มจาก **Direct Product** เสมอ แล้วขยับ mode เมื่อวัตถุประสงค์ของชิ้นงานต้องการบริบทเพิ่ม ไม่สร้าง editorial story เพียงเพราะมีพื้นที่ภาพ

### Image Roles

| Role | Purpose | Current assets |
|---|---|---|
| `Image/Hero/Device` | แนะนำ technology ด้วย silhouette ที่จดจำได้ | `icoone device.png` |
| `Image/Detail/Engineering` | แสดง material, handpiece และ interaction | `robo handpieces.png`, `robosolo laser.png` |
| `Image/Evidence/Mechanism` | อธิบายกลไก ไม่ใช้เป็นผลลัพธ์รับรอง | `laser led.png` |
| `Image/Human/Application` | แสดงการใช้งานอย่างเคารพและมีบริบท | `robotwin back.png`, `robotwin neck.png`, `robo twin legs.png`, `men's robosolo.png` |
| `Image/Environment` | สื่อ experience และ service setting | `BIB treatment room.png` |

### Editorial Crop Variants

- **Hero 60/40:** ภาพ 60% + copy 40%; ภาพต้องมี negative space รองรับ headline
- **Object cutout:** device บน Ivory/White; ไม่ใส่ glow หรือ shadow เกินจริง
- **Detail strip:** crop แนวนอน 3:1 สำหรับ mechanism/support module
- **Human moment:** crop ที่เห็นการดูแลและ interaction ไม่แยกร่างกายเป็น problem area

### Image Overlay

- ใช้ solid Ivory/Charcoal field ข้างภาพก่อนใช้ gradient
- หากต้องวาง text บนภาพ ให้ใช้ overlay Charcoal 20–45% และทดสอบ contrast
- ห้ามเปลี่ยนสีผิว ขยายผลลัพธ์ หรือ retouch รูปร่าง

### Product Cutout Rules

- ใช้ไฟล์รุ่นจริงและสัดส่วนจริง; ห้ามสร้างเครื่องใหม่ด้วย AI หรือปรับองค์ประกอบจนผิดจากสินค้า
- แสดงเครื่องครบพอให้จำรุ่นได้ ไม่ crop จนเหลือ silhouette ที่กำกวม
- พื้น White/Ivory เป็นค่าเริ่มต้น; transparent cutout ต้องไม่มี tagline เก่าหรือ metadata ที่ไม่เกี่ยวข้องติดมา
- ไม่มีกริด วงโคจร glow ฉากสปา หรือ pseudo-clinical background ในเอกสาร commercial
- ไม่วาง caption หรือข้อความบนตัวเครื่อง
- หากข้อมูลคือ focal point ภาพเครื่องทำหน้าที่ identification ได้โดยไม่ต้องขยายเป็น hero

### Rights Gate

ภาพทุกไฟล์เริ่มที่สถานะ **WORKING** จนมี metadata: source, owner, consent/license, allowed channels, expiry และ approver งาน public ต้องเป็น **APPROVED PUBLIC** เท่านั้น

---

## 5. Editorial Components

### 5.1 Editorial Hero

**Structure:** English kicker → Thai headline → short thesis → hero image/object

- Kicker: Muli Medium, uppercase, tracking 0.08–0.12 em
- Thai headline: Kanit Light/Regular, ไม่เกิน 2–3 บรรทัด
- Thesis: 40–70 คำ อ่านจบในหนึ่ง breath
- Campaign และ corporate story ห้ามเปิดด้วย feature list หรือส่วนลด
- Commercial document ไม่จำเป็นต้องใช้ Editorial Hero; เปิดด้วยข้อเสนอหรือประโยชน์หลักได้โดยตรง

### 5.1A Commercial Header

**Structure:** Plan/Product label → Thai outcome headline → one-line relevance → product cutout

- Headline ต้องเข้าใจได้โดยไม่อ่านชื่อ Edition
- ตัวเลขหรือเงื่อนไขที่เป็น value หลักใส่ใน headline ได้ เช่น “แบ่งชำระ 10 งวด ดอกเบี้ย 0%”
- English Edition เป็น optional metadata; ไม่ใช้แทนสารหลัก
- Product image ใช้ Direct Product mode เท่านั้น

### 5.2 Solution-Fit Card

แทน component เดิม “Designed for clinic”

| Label | Content |
|---|---|
| `SOLUTION FIT WHEN` | สถานการณ์จริงที่ทำให้แผนนี้เหมาะ |
| `BUSINESS SIGNALS` | traffic/demand, capital, team readiness, time horizon |
| `WHY THIS PATH` | เหตุผลเชิงธุรกิจ 3 ข้อ |

ใช้ภาษาที่อธิบาย situation ไม่ label ประเภทธุรกิจ เช่น “เมื่อมี demand สม่ำเสมอและต้องการรักษาสภาพคล่อง”

### 5.3 Evidence Block

- ตัวเลขเด่น 1–4 ค่า
- ระบุ unit, period และความหมายในจุดเดียวกัน
- Commercial estimate ใช้คำว่า scenario/ประมาณการและแสดง assumptions
- Minimum Guarantee ต้องระบุผู้รับประกันและผู้รับประโยชน์ ห้ามเขียนเพียง “รับประกันรายได้”

### 5.4 Commercial Pathway Module

ลำดับ: `Business intent → Commercial structure → Ownership/status → Support → Next decision`

- เสนอหนึ่ง pathway ต่อหนึ่ง client-facing asset
- เงื่อนไข conversion/ownership ต้องมี trigger, formula และ approval status
- ไม่ใช้ discount badge, countdown หรือ red price strike-through

### 5.5 CTA Module

Primary: **“นัดพูดคุยเพื่อค้นหา Solution ที่เหมาะกับธุรกิจของคุณ”**  
Secondary: **“ร่วมประเมิน demand, capacity และ investment scenario จากข้อมูลจริง”**

---

## 6. Commercial Leaflet Template — A4

### Grid

- 6 columns; outer margin 16–18 mm
- Top brand zone 18–24 mm
- Main narrative zone 55–70 mm
- Commercial data zone 30–38 mm
- Fit/evidence zone 70–90 mm
- CTA/legal zone 32–42 mm

### Required Modules

1. Co-brand header
2. Commercial pathway label
3. Editorial headline and opening
4. Commercial numbers
5. Why this path ×3
6. Solution Fit When
7. Key terms/support
8. Consultative CTA
9. Legal/commercial disclaimer

### Image Use

- ค่าเริ่มต้นคือ device cutout บน White/Ivory เป็น right-side identification anchor ประมาณ 18–28% ของหน้า
- ภาพมนุษย์ใช้เมื่อมีสิทธิ์และเนื้อหาต้องการอธิบาย experience
- Term sheet ไม่ใช้ภาพมนุษย์หรือฉาก narrative; detail images ใช้เฉพาะเมื่อจำเป็นต่อการอธิบายรายการที่เสนอ
- Package accent ใช้กับ top rule, label หรือ key number เท่านั้น ไม่ใช้ย้อมภาพหรือสร้าง mood แยกแผน

---

## 7. Review Checklist

### Brand

- [ ] Thai = Kanit / English = Muli และ font ถูก embed
- [ ] ใช้ working/approved logo master ถูก variant
- [ ] White/Ivory 70% โดยประมาณ และ accent ไม่เกินขอบเขต
- [ ] ภาพมีสถานะ rights/consent ชัดเจน
- [ ] Visual mode ตรงกับวัตถุประสงค์; commercial default = Direct Product

### Content

- [ ] เปิดด้วยบริบทธุรกิจ ไม่จำกัดคำว่า clinic
- [ ] Headline บอก subject/value ได้โดยไม่พึ่งชื่อ Edition หรือคำเปรียบ
- [ ] มี Solution Fit และเหตุผลของคำแนะนำ
- [ ] Claim และ commercial number มี source/approval
- [ ] ROI เป็น scenario ไม่ใช่ guarantee

### Production

- [ ] A4 อ่านจบได้ประมาณหนึ่งนาที
- [ ] ไม่มี overflow และ body ไม่เล็กกว่าขนาดขั้นต่ำ
- [ ] ส่งเฉพาะ commercial pathway ที่คัดให้ผู้รับรายนั้น
- [ ] Final artwork ผ่าน Brand + Commercial + Regulatory/Legal review

---

## 8. Open Production Items

1. ใช้ static legacy Muli files สำหรับ production PDF; เก็บ Mulish variable file เป็น archive เท่านั้น
2. ขอ vector logo masters (SVG/EPS/PDF) สำหรับงานขนาดใหญ่
3. Rename numbered image assets และสร้าง metadata/consent register
4. ยืนยันว่า `icoone device.png` มี embedded tagline “Better Technology of Life” ซึ่งอาจไม่เหมาะกับทุก campaign; ถ้าต้องการ cutout ที่ไม่มีข้อความ ให้ขอ source asset จากเจ้าของไฟล์ ไม่ลบจาก master โดยพลการ
5. ทำ Figma/PowerPoint components จาก tokens และ modules ในเอกสารนี้หลัง Brand Master sign-off
