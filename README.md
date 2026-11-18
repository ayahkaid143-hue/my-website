# موقع آية قايد الحيلة

موقع تعريفي عربي ثابت، متجاوب مع الجوال، ومجهز للنشر على GitHub Pages. لا يحتاج تثبيت برامج أو خادم أو قاعدة بيانات.

## النشر من موقع GitHub

1. سجّلي الدخول إلى [GitHub](https://github.com) وأنشئي مستودعًا جديدًا باسم `aya-profile`.
2. اختاري **Public**؛ GitHub Pages لا يجعل الموقع محميًا برابط خاص. لا تضعي في الملفات رقم هاتف أو بريدًا شخصيًا لا تريدين نشره.
3. داخل المستودع اختاري **Add file → Upload files**. ارفعي محتويات هذا المجلد كلها، وتأكدي أن `index.html` في جذر المستودع وليس داخل مجلد إضافي، ثم اضغطي **Commit changes**.
4. افتحي **Settings → Pages**. تحت **Build and deployment** اختاري **Deploy from a branch**، ثم الفرع `main` والمجلد `/(root)`، واضغطي **Save**.
5. انتظري اكتمال النشر. سيظهر رابط الموقع في صفحة **Settings → Pages**، ويكون شكله غالبًا `https://USERNAME.github.io/aya-profile/` مع استبدال `USERNAME` باسم حسابك.

## الرفع من الكمبيوتر عبر Git

بعد إنشاء المستودع العام في GitHub، افتحي الطرفية داخل مجلد الموقع واستبدلي `USERNAME` باسم حسابك:

```bash
git init
git add .
git commit -m "Create Aya's personal website"
git branch -M main
git remote add origin https://github.com/USERNAME/aya-profile.git
git push -u origin main
```

ثم فعّلي Pages من **Settings → Pages** باتباع الخطوة الرابعة أعلاه.

## تحديث المعلومات

- النصوص والأقسام موجودة في `index.html`.
- الألوان والخطوط والتنسيق في `styles.css`.
- تفاعلات القائمة والنسخ في `script.js`.
- الرسوم والأيقونة في `assets/`.

لإضافة بريد أو روابط حسابات اجتماعية، عدّلي قسم التواصل في `index.html` وضعي فقط البيانات التي ترغبين في جعلها علنية.

## ملاحظة الخصوصية

ملف `robots.txt` ووسم `noindex` يطلبان من محركات البحث عدم فهرسة الصفحة، لكنهما لا يضعان كلمة مرور ولا يمنعان أي شخص من فتح الرابط أو إعادة مشاركته. لا ترسلي معلومات خاصة إلى موقع منشور على GitHub Pages.
