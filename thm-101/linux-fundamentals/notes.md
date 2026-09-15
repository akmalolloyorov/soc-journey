# Cron va Crontab — tushuntirish

## 🎯 Nima uchun kerak?

Tizim yoqilgandan keyin (yoki muntazam ravishda) avtomatik bajariladigan vazifalarni sozlash uchun. Masalan: fayllarni backup qilish, dasturlarni ishga tushirish, buyruqlarni jadval bo'yicha bajarish.

## ⚙️ Cron nima?

**Cron** — bu tizim yuklanganda ishga tushadigan process (background'da doim ishlaydi). U **crontab** fayllarini o'qib, unda yozilgan vazifalarni belgilangan vaqtda bajaradi.

**Crontab** — cron uchun maxsus formatdagi fayl, har bir qator alohida vazifa.

## 📋 6 ta asosiy qiymat

| Qiymat | Nima uchun |
|--------|-----------|
| MIN | Necha minutda ishga tushsin |
| HOUR | Necha soatda |
| DOM | Oyning qaysi kunida (Day of Month) |
| MON | Yilning qaysi oyida |
| DOW | Haftaning qaysi kunida (Day of Week) |
| CMD | Bajariladigan buyruqning o'zi |

## 💡 Misol

Har 12 soatda `cmnatic` foydalanuvchisining `Documents` papkasini backup qilish uchun quyidagi qator yoziladi:

```bash
0 */12 * * * cp -R /home/cmnatic/Documents /var/backups/
```

**Izoh:**
- `0` — 0-minutda
- `*/12` — har 12 soatda bir marta
- `* * *` — oy, kun, hafta kuni muhim emas (wildcard)
- oxiri — bajariladigan buyruq

## ⭐ Wildcard (`*`) nima uchun?

Agar biror qiymat muhim bo'lmasa (masalan, "qaysi oy" farqi yo'q), o'sha joyga `*` qo'yiladi — "istalgan vaqt/qiymat" degani.

## 🛠️ Foydali resurslar
- **Crontab Generator** — vizual interfeys orqali formatlashni avtomatik yaratadi
- **Cron Guru** — sintaksisni tekshirish/tushuntirish uchun

## 📝 Tahrirlash

```bash
crontab -e
```
Bu buyruq crontab faylini ochadi (odatda Nano editor bilan), o'zgarishlar shu yerda kiritiladi.

## Task 1 — Automation (Amaliy mashq)

Cron qanday ishlashini tushunish uchun eng yaxshi yo'l — uni amalda sinab ko'rish. Quyidagi qadamlarni ketma-ket bajaring:

**1-qadam:** Crontab editorni oching:
```bash
crontab -e
```

**2-qadam:** Quyidagi qatorni qo'shing — bu har daqiqada joriy vaqtni faylga yozadi:
```bash
* * * * * date >> /home/Admin/Documents/cron-test.log
```

**3-qadam:** Saqlab chiqing (`Ctrl+O` → `Enter` → `Ctrl+X`), so'ng tekshiring:
```bash
crontab -l
```

**4-qadam:** Bir necha daqiqa kutib, natijani ko'ring:
```bash
cat /home/Admin/Documents/cron-test.log
```

Agar hammasi to'g'ri ishlagan bo'lsa, quyidagidek natija chiqadi — har daqiqada aniq bitta yangi qator qo'shilib boradi:

![Cron job natijasi — har daqiqada log yozilishi](screenshots/cron-test-log.png)

### Qo'shimcha mashq: turli vaqt formatlarini sinab ko'ring

Cron formatini yaxshiroq o'zlashtirish uchun quyidagi misollarni ham o'zingiz yozib ko'ring:

- `0 */12 * * *` — har 12 soatda ishga tushadi
- `45 23 1,15 2,4,6,8,10,12 *` — oyning 1- va 15-kunlarida, belgilangan oylarda (fevral, aprel, iyun, avgust, oktyabr, dekabr), soat 23:45da ishga tushadi
- `0 8 * * 1,3,5` — dushanba, chorshanba va juma kunlari soat 8:00da ishga tushadi

Har birini `crontab -e` orqali kiritib, `crontab -l` bilan tekshirib boring — shu tariqa format qanday o'zgarishini his qilasiz.
