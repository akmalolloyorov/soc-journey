# Windows Desktop — Umumiy Ko'rinish (GUI)

## 🖥️ Windows Desktop nima?

**Windows Desktop** (grafik foydalanuvchi interfeysi, ya'ni **GUI**) — bu Windows 10 mashinasiga tizimga kirgandan keyin sizni kutib oladigan asosiy ekran.

Odatda, avval **login ekrani**dan o'tish kerak bo'ladi — bu yerda haqiqiy hisob ma'lumotlari (username va parol) kiritiladi. Bu hisob — o'sha tizimdagi mavjud Windows account yoki, agar mashina domenga ulangan bo'lsa, **Active Directory** muhitidagi hisob bo'lishi mumkin.

## 🧩 GUI'ning asosiy qismlari

Windows Desktop quyidagi komponentlardan tashkil topgan:

1. **The Desktop** — ish stoli
2. **Start Menu** — boshlash menyusi
3. **Search Box (Cortana)** — qidiruv paneli
4. **Task View** — ochiq oynalar ko'rinishi
5. **Taskbar** — vazifalar paneli
6. **Toolbars** — asboblar paneli
7. **Notification Area** — bildirishnomalar hududi

---

## 🖱️ The Desktop (Ish stoli)

Desktop — bu dasturlar, papkalar, fayllarga tezkor kirish uchun yorliqlar (shortcut) joylashadigan joy. Bu belgilar (ikonkalar) alifbo bo'yicha papkalarga tartibli joylashtirilgan yoki tartibsiz sochilgan holda bo'lishi mumkin — ikkala holatda ham, ularning maqsadi **tez kirish** imkonini berish.

### Sozlash imkoniyatlari

Desktop bo'sh joyiga o'ng tugma bilan bosilganda, kontekst menyu chiqadi. Bu menyu orqali quyidagilarni o'zgartirish mumkin:
- Desktop ikonkalarining o'lchami
- Ularni qanday joylashtirish kerakligi
- Nusxa ko'chirish/joylashtirish (copy/paste)
- Yangi element yaratish (papka, shortcut, matn hujjati)

**Display settings** orqali:
- Ekran ruxsati (resolution) va orientatsiyasini o'zgartirish
- Bir nechta monitor bo'lsa, multi-screen sozlamalarini boshqarish

> 📌 **Eslatma:** Remote Desktop sessiyasida ba'zi display sozlamalari o'chirilgan (disabled) bo'ladi.

**Personalize** orqali:
- Fon rasmini (wallpaper) o'zgartirish
- Shriftlar, mavzular (themes), rang sxemasini sozlash

---

## 🪟 The Start Menu

Avvalgi Windows versiyalarida ekranning chap pastki burchagida "Start" so'zi ko'rinardi. Zamonaviy versiyalarda (Windows 10 kabi) bu so'z ko'rinmaydi, o'rniga **Windows logotipi** chiqadi. Ko'rinishi o'zgargan bo'lsa-da, vazifasi bir xil qolgan — eng ko'p ishlatiladigan ilova, fayl va vositalarga tezkor kirish.

Windows logotipiga bosilganda, Start Menu ochiladi. U bir nechta bo'limdan iborat:

### 1-bo'lim — Hisob va tizim amallari
Bu yerda hisobga oid qisqa yo'llar joylashgan: hisobni o'zgartirish, ekranni bloklash, tizimdan chiqish. Shuningdek:
- **Hujjatlar (Documents)** va **Rasmlar (Pictures)** papkalariga yorliqlar
- **Sozlamalar (Settings)** — tishli g'ildirak belgisi orqali
- **Quvvat (Power)** belgisi — Remote Desktop'dan uzilish, kompyuterni o'chirish yoki qayta ishga tushirish

Bu bo'limni kengaytirish uchun yuqoridagi "gamburger" ko'rinishidagi belgiga bosiladi.

### 2-bo'lim — Ilovalar ro'yxati
- Yuqori qismda **yaqinda qo'shilgan** ilovalar/dasturlar ko'rsatiladi
- Pastda **o'rnatilgan barcha ilovalar** alifbo tartibida, har bir harf o'z bo'limiga ega bo'lgan holda ko'rsatiladi

> 📌 **Eslatma:** Ba'zi VM'larda Google Chrome endi "Recently Added" bo'limida ko'rinmaydi.

Agar o'rnatilgan dasturlar ro'yxati juda uzun bo'lsa, harflar ustiga bosib, alifbo panjarasi (alphabet grid) orqali kerakli bo'limga to'g'ridan-to'g'ri o'tish mumkin.

### 3-bo'lim — Tile'lar (Ilovalar kartochkalari)
Start Menu'ning o'ng tomonida maxsus ilova/dastur yoki vositalar uchun belgilar joylashgan — bular **tile** deb ataladi. Ba'zilari standart holatda qo'shilgan bo'ladi.

Tile ustiga o'ng tugma bilan bosilsa, qo'shimcha amallar menyusi chiqadi:
- O'lchamini o'zgartirish
- Start Menu'dan olib tashlash (unpin)
- Xususiyatlarini (Properties) ko'rish

Dasturni Start Menu'ga qo'shish uchun: dastur ustiga o'ng tugma bosib, **"Pin to Start"** tanlanadi.

---

## 📊 The Taskbar (Vazifalar paneli)

Ba'zi komponentlar standart holatda yoqilgan va ko'rinadi. Masalan, **Toolbar** — bu demonstratsiya maqsadida alohida yoqilishi mumkin bo'lgan komponent.

Taskbar'ga o'ng tugma bilan bosilsa, kontekst menyu chiqadi — bu orqali qaysi komponentlarni yoqish/o'chirishni sozlash mumkin.

Ochilgan/ishga tushirilgan har qanday dastur, papka yoki fayl — taskbar'da ko'rinadi. Belgi ustiga sichqonchani olib borilsa, **preview thumbnail** va tooltip chiqadi — bu, masalan, bir nechta Google Chrome oynasi ochiq bo'lsa, kerakli oynani topishda foydali.

Element yopilganda, u taskbar'dan yo'qoladi — **agar aniq pin qilinmagan bo'lsa**.

---

## 🔔 The Notification Area (Bildirishnomalar hududi)

Odatda ekranning **pastki o'ng burchagida** joylashgan — bu yerda sana va vaqt ko'rsatiladi. Bundan tashqari, bu yerda quyidagilar ham bo'lishi mumkin:
- Ovoz balandligi belgisi
- Tarmoq/wireless belgisi
- va boshqa tizim belgilari

Belgilarni qo'shish yoki olib tashlash **Taskbar settings** orqali, **Notification Area** bo'limida amalga oshiriladi.

---

## 💡 Foydali maslahat

Istalgan papka, fayl, dastur yoki belgi ustiga **o'ng tugma bilan bosish** orqali qo'shimcha ma'lumot yoki amallarni ko'rish mumkin — bu Windows'da eng ko'p ishlatiladigan interaktsiya usullaridan biri.
