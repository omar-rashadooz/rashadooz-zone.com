<div align="center">

<img src="logo.png" width="160" alt="RASHADOOZ ZONE logo">

# RASHADOOZ ZONE

**مركزك الأول لأخبار البرمجة والألعاب** 🎮💻

موقع أخبار ثابت (Static) مبني بـ HTML و CSS و JavaScript، ومنشور على GitHub Pages.

[🌐 زور الموقع](https://omar-rashadooz.github.io/rashadooz-zone.com/) · [📸 انستجرام](https://www.instagram.com/rashadooz_zone) · [💬 ديسكورد](https://discord.gg/8DaZQyMmX)

</div>

---

## ✨ المميزات

- فيد أخبار شبه فيسبوك مع صور ومقتطف من كل مقال
- أقسام: **Home** و **Programming** و **Games** و **Contact Us**
- صفحة مستقلة لكل خبر (`post.html?id=N`)
- بحث في عناوين ومحتوى كل الأخبار (بيدعم العربي: توحيد الهمزات والتاء المربوطة وتجاهل التشكيل)
- عداد لايكات لكل خبر
- تاريخ النشر بالأسابيع + الشهر والسنة
- كارت "آخر خبر" في البرمجة وفي الألعاب في الصفحة الرئيسية
- خط **Cairo** وألوان ثلاثة بس: أسود، أحمر، أبيض
- واجهة RTL بالعربي ومتوافقة مع الموبايل

## 📁 هيكل المشروع

```
├── index.html          # الصفحة الرئيسية (Home + الفيد + Contact)
├── post.html           # صفحة الخبر الواحد
├── style.css           # التصميم
├── script.js           # منطق الصفحة الرئيسية (الفيد، البحث، التنقل)
├── post.js             # منطق صفحة الخبر
├── posts.js            # قائمة الأخبار + الدوال المشتركة
├── logo.png            # اللوجو
├── Cairo-Bold.ttf      # الخط
├── Cairo-Black.ttf     # الخط
├── photo_numN.png      # صورة الخبر رقم N
└── subject_numN.txt    # مقال الخبر رقم N
```

## ➕ إضافة خبر جديد

1. ارفع صورة الخبر باسم `photo_numN.png`.
2. ارفع المقال باسم `subject_numN.txt` (نص عادي، `N` هو رقم الخبر).
3. في ملف `posts.js` ضيف سطر جديد **أول القايمة** (الأحدث فوق):

```js
{ id: 14, title: "عنوان الخبر", category: "games", date: "2026-10-22", likes: 120 },
```

| الحقل | المعنى |
|-------|--------|
| `id` | رقم الخبر (فريد، ولازم يطابق رقم الصورة والملف) |
| `title` | العنوان |
| `category` | `programming` أو `games` |
| `date` | تاريخ النشر `سنة-شهر-يوم` |
| `likes` | العدد الأساسي للايكات (بيتضاف عليه رقم عشوائي صغير في كل زيارة) |

بعد الـ commit بتظهر التعديلات على الموقع خلال دقيقة أو اتنين.

## 🚀 التشغيل محليًا

المقالات بتتحمل بـ `fetch`، فلازم سيرفر محلي (فتح `index.html` مباشرة مش هيشتغل):

```bash
python3 -m http.server 8000
# وافتح http://localhost:8000
```

## 🌍 النشر على GitHub Pages

`Settings` ← `Pages` ← **Deploy from a branch** ← اختار `main` و `/ (root)` ← `Save`.

## 📬 التواصل

- البريد: omarmrashad92@gmail.com
- ديسكورد: https://discord.gg/8DaZQyMmX
- انستجرام: [@rashadooz_zone](https://www.instagram.com/rashadooz_zone)

---

<div align="center">© 2026 RASHADOOZ ZONE</div>
