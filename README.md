# ⚡ Mini-Terminal: Interactive Web CLI Engine

HTML5, CSS3 va Vanilla JavaScript yordamida yaratilgan, retro-kiberpank uslubidagi interaktiv terminal (Buyruqlar satri) simulyatori. Ushbu loyiha CLI (Command Line Interface) tizimlarining ishlash mantig'ini hamda JavaScript orqali DOM-ni dinamik manipulyatsiya qilish usullarini mukammal ko'rsatib beradi.

---

## 📝 Loyiha haqida

Dastur Stark Industries kompaniyasining afsonaviy `JARVIS OS` interfeysidan ilhomlangan holda ishlab chiqilgan. Foydalanuvchi maxsus buyruqlarni kiritish orqali tizim bilan real vaqt rejimida muloqot qilishi mumkin. Tizim noto'g'ri kiritilgan buyruqlarni avtomatik aniqlaydi va rangli indikatorlar orqali xatoliklarni qayd etadi.

---

## 📐 Buyruqlar Arxitekturasi va Logika Zanjiri (CLI Execution Flow)

Terminalga buyruq kiritilganda, JavaScript hodisalar filtri matnni tozalaydi va quyidagi algoritm asosida qayta ishlaydi:

1. [ Enter Keydown ] ──► `.toLowerCase().trim()` orqali matn formatlanadi.
2. [ Echo Effect ] ──► Kiritilgan buyruq tarix sifatida ekranga qayta chop etiladi (`print()`).
3. [ Router Engine ] ──► `if-else` mantiqiy silsilasi buyruq kalit so'zini tekshiradi:
   * `help`   ──► Mavjud buyruqlar ro'yxatini chiqarish.
   * `about`  ──► Loyiha va muallif haqida ma'lumot (`.success` klassi bilan).
   * `date`   ──► JavaScript `Date()` obyekti orqali joriy vaqtni generatsiya qilish.
   * `clear`  ──► `innerHTML = ''` yordamida ekranni tozalash.
   * `hack`   ──► Matrix uslubidagi maxfiy animatsion simulyatsiya (`.error` klassi bilan).
4. [ Auto-Scroll ] ──► Yangi element qo'shilgach, oyna avtomatik tubiga tushadi (`scrollTop = scrollHeight`).

---

## ⚡ Asosiy xususiyatlari (Features)

* 📟 **Authentic Matrix UI:** Klassik yashil monoxrom ranglar palitrasi (`#00ff41`) va `Courier New` shrifti yordamida yaratilgan mukammal terminal atmosferasi.
* ⌨️ **Smart Key Listener:** Faqatgina `Enter` tugmasi bosilganda buyruqni ijro etish va kiritish maydonini avtomatik tozalash tizimi.
* 🎛️ **Dinamik DOM Generator:** Har bir buyruq natijasi uchun yangi `<div>` elementi yaratilib, uning turiga qarab dinamik klasslar (`error`, `success`) yuklanishi.
* 🚀 **Autofocus Input:** Sahifa yuklanishi bilanoq kursorning kiritish maydonida (`input`) avtomatik tayyor turishi.
* 🧹 **Buffer Clear Engine:** Oynani tozalash mexanizmi xotirani yuklamasdan terminal buferini lahzada bo'shatadi.

---

## 🛠️ Texnologiyalar (Tech Stack)

* **HTML5** — Terminal chiqish oynasi (`#output`) va buyruq kiritish qatori strukturasi.
* **CSS3 Flexbox** — Ekranni to'liq qoplovchi (`100vh`) va o'suvchi (`flex-grow: 1`) terminal arxitekturasi.
* **Vanilla JavaScript (ES6+)** — String metodlari, Event Listeners va DOM elementlari generatsiyasi.

---

## 🚀 Ishga tushirish (How to Run)

Loyiha hech qanday qo'shimcha resurslar yoki kutubxonalarga bog'lanmagan:

1. Repozitoriyni kompyuterga yuklab oling:
   ```bash
   git clone [https://github.com/orgkamolbek/mini-terminal.git](https://github.com/orgkamolbek/mini-terminal.git)
