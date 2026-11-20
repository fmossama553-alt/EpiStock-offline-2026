# LEONI Epissure Manager

تطبيق ويب للهاتف لمتابعة **نقص الـÉpissures** فقط. بدون أي framework وبدون build: ملفات HTML/JS عادية.

> نموذج أولي مستقل، غير مرتبط بأنظمة LEONI الداخلية.

## الملفات
- `index.html` : التطبيق كامل (واجهة + منطق + 3 لغات FR/AR/EN)
- `manifest.json` + `icon.svg` + `sw.js` : باش يتركّب كتطبيق (PWA)

## النشر على GitHub Pages
1. Settings ← Pages
2. Source: **Deploy from a branch** ← Branch: `main` / `(root)` ← Save
3. بعد دقيقة يظهر الرابط: `https://USERNAME.github.io/REPO/`

## التركيب على أندرويد
Chrome ← فتح الرابط ← ⋮ ← **Ajouter à l'écran d'accueil**

## الميزات
- خطوط الإنتاج (إضافة / حذف)
- لكل Épissure: مرجع، كمية مطلوبة، متوفرة، والناقصة تتحسب وحدها
- الكابلات المكوّنة (CB-xxxx) وحالتها: متوفر / في Magasin (بدون كمية). كليك على الكابل يبدّل الحالة
- البحث باسم Épissure يعرض كل الخطوط اللي تستعملها مع الكمية الناقصة، والبحث يخدم بالخط والكابل زادة
- فلترة بالحالة والخدمة (Préparation / Magasin)
- الحالات: En attente ← En préparation ← Disponible ← Livré
- سجل يومي

## التخزين
حاليًا في `localStorage` (كل هاتف عنده نسخته). لقاعدة بيانات مشتركة: Firebase أو Supabase.
