# دليل إضافة المقالات للمدونة

## كيفية إضافة مقالة جديدة

### الخطوة 1: إنشاء صفحة المقالة
1. انسخ ملف `article.html` وسمه باسم المقالة الجديدة
   ```
   article-2.html
   article-3.html
   article-4.html
   ```

### الخطوة 2: تعديل محتوى المقالة الجديدة
في الملف الجديد، قم بتعديل:

#### أ. العنوان في `<head>`
```html
<title>عنوان المقالة الجديدة | مجموعة السمين للمحاماة</title>
```

#### ب. رابط التنقل (Breadcrumb)
```html
<div class="article-breadcrumb">
    <a href="index.html">الرئيسية</a>
    <i class="fas fa-chevron-left"></i>
    <a href="index.html#blog">المدونة</a>
    <i class="fas fa-chevron-left"></i>
    <span>عنوان المقالة الجديدة</span>
</div>
```

#### ج. عنوان المقالة الرئيسي
```html
<h1 class="article-title">عنوان المقالة الجديدة</h1>
```

#### د. معلومات المقالة
```html
<div class="article-meta">
    <div class="article-meta-item">
        <i class="fas fa-calendar"></i>
        <span>تاريخ النشر</span>
    </div>
    <div class="article-meta-item">
        <i class="fas fa-clock"></i>
        <span>وقت القراءة</span>
    </div>
    <div class="article-meta-item">
        <i class="fas fa-user"></i>
        <div class="article-author">
            <img src="assets/images/lawyers/Ahmedelsmeen.jpg" alt="اسم الكاتب">
            <span>اسم الكاتب</span>
        </div>
    </div>
</div>
```

#### ه. صورة المقالة الرئيسية
```html
<div class="article-image">
    <img src="رابط-الصورة-الجديدة" alt="وصف الصورة">
</div>
```

#### و. محتوى المقالة
```html
<article class="article-body">
    <!-- محتوى المقالة هنا -->
    <h2>عنوان فرعي</h2>
    <p>محتوى الفقرة...</p>
    
    <h3>عنوان فرعي أصغر</h3>
    <ul>
        <li>نقطة أولى</li>
        <li>نقطة ثانية</li>
    </ul>
    
    <blockquote>
        <p>نص الاقتباس</p>
    </blockquote>
</article>
```

#### ز. علامات المقالة
```html
<div class="article-tags">
    <a href="#" class="article-tag">العلامة الأولى</a>
    <a href="#" class="article-tag">العلامة الثانية</a>
    <a href="#" class="article-tag">العلامة الثالثة</a>
</div>
```

### الخطوة 3: إضافة بطاقة المقالة في الصفحة الرئيسية

في ملف `index.html`، ابحث عن قسم المدونة وأضف بطاقة جديدة:

```html
<div class="blog-card" data-aos="fade-up" data-aos-delay="300">
    <div class="blog-image">
        <img src="رابط-صورة-المقالة" alt="عنوان المقالة">
    </div>
    <div class="blog-content">
        <h3>عنوان المقالة الجديدة</h3>
        <span class="blog-date">تاريخ النشر</span>
        <p>ملخص قصير للمقالة في سطرين أو ثلاثة...</p>
        <a href="article-2.html" class="blog-readmore">اقرأ المزيد</a>
    </div>
</div>
```

### الخطوة 4: تحديث المقالات ذات الصلة

في نهاية كل مقالة، قم بتحديث قسم "مقالات ذات صلة":

```html
<div class="related-grid">
    <div class="related-card">
        <img src="رابط-صورة-مقالة-ذات-صلة" alt="عنوان المقالة ذات الصلة">
        <div class="related-card-content">
            <h4>عنوان المقالة ذات الصلة</h4>
            <p>ملخص قصير...</p>
            <a href="رابط-المقالة" class="read-more">اقرأ المزيد</a>
        </div>
    </div>
    <!-- كرر للبطاقات الأخرى -->
</div>
```

## نصائح مهمة

### 1. تسمية الملفات
- استخدم أسماء واضحة: `article-2.html`, `article-3.html`
- أو استخدم أسماء وصفيّة: `contracts-guide.html`, `labor-law-guide.html`

### 2. الصور
- استخدم صور عالية الجودة (600px عرض على الأقل)
- اضغط الصور لتحسين سرعة التحميل
- استخدم أسماء ملفات وصفيّة للصور

### 3. المحتوى
- اكتب عناوين جذابة ومختصرة
- استخدم فقرات قصيرة (3-4 جمل)
- أضف قوائم ونقاط لسهولة القراءة
- استخدم اقتباسات لتمييز النقاط المهمة

### 4. SEO
- استخدم كلمات مفتاحية مناسبة في العناوين
- أضف وصف للصور (alt text)
- استخدم عناوين هرمية (h2, h3, h4)

### 5. الروابط
- تأكد من أن جميع الروابط تعمل
- اختبر الروابط بعد النشر
- استخدم روابط نسبية للملفات المحلية

## مثال سريع لإضافة مقالة جديدة

1. انسخ `article.html` إلى `article-2.html`
2. عدّل العنوان إلى "أهمية العقود في حماية الأعمال"
3. غيّر الصورة إلى صورة مناسبة للعقود
4. اكتب المحتوى الجديد
5. أضف البطاقة في `index.html`
6. اختبر الروابط

## إدارة المحتوى المستقبلية

لإدارة أفضل للمحتوى، يمكنك:
- إنشاء مجلد `articles/` للمقالات
- إنشاء ملف `articles.json` لتخزين بيانات المقالات
- إنشاء نظام إدارة محتوى بسيط
- استخدام GitHub Pages للنشر التلقائي

---

**ملاحظة:** تأكد من اختبار جميع الروابط والصور قبل النشر النهائي! 