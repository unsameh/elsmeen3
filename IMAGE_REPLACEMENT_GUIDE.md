# 🖼️ دليل استبدال الصور بالصور المحلية | Image Replacement Guide

## 📁 **الخطوة 1: إعداد المجلدات** | Step 1: Setup Folders

تم إنشاء المجلدات التالية لك:
```
website/
├── assets/
│   └── images/
│       ├── lawyers/     (صور المحامون)
│       └── logo/        (الشعار)
```

## 🖼️ **الخطوة 2: تحضير الصور** | Step 2: Prepare Images

### **للشعار | For Logo:**
- ضع صورة الشعار في `assets/images/logo/`
- الحجم الموصى به: 200×200 بكسل أو أكبر
- الصيغ المدعومة: JPG, PNG, WebP
- اسم الملف المقترح: `logo.png` أو `logo.jpg`

### **لصور المحامون | For Lawyer Photos:**
- ضع صور المحامون في `assets/images/lawyers/`
- الحجم الموصى به: 400×400 بكسل (مربع)
- الصيغ المدعومة: JPG, PNG, WebP
- أسماء الملفات المقترحة: `lawyer1.jpg`, `lawyer2.jpg`, إلخ...

## 🔄 **الخطوة 3: استبدال الروابط** | Step 3: Replace Links

### **في ملف index.html:**

#### **استبدال الشعار | Replace Logo:**
```html
<!-- من | From: -->
<img src="https://images.unsplash.com/photo-1589829545856-d10d557cf95f?w=50&h=50&fit=crop&crop=face" alt="مكتب المحاماة الحديث" class="logo-image">

<!-- إلى | To: -->
<img src="assets/images/logo/logo.png" alt="مكتب المحاماة الحديث" class="logo-image">
```

#### **استبدال صور المحامون | Replace Lawyer Photos:**
```html
<!-- من | From: -->
<img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=200&h=200&fit=crop&crop=face" alt="أحمد محمد علي">

<!-- إلى | To: -->
<img src="assets/images/lawyers/lawyer1.jpg" alt="أحمد محمد علي">
```

## 📋 **قائمة كاملة بالاستبدالات** | Complete Replacement List

### **الشعار | Logo (2 مرات | times):**
1. في الهيدر | In header: `assets/images/logo/logo.png`
2. في الفوتر | In footer: `assets/images/logo/logo.png`

### **صور المحامون | Lawyer Photos (10 مرات | times):**
1. أحمد محمد علي: `assets/images/lawyers/lawyer1.jpg`
2. فاطمة أحمد حسن: `assets/images/lawyers/lawyer2.jpg`
3. محمد عبدالله سالم: `assets/images/lawyers/lawyer3.jpg`
4. سارة خالد محمد: `assets/images/lawyers/lawyer4.jpg`
5. علي حسن أحمد: `assets/images/lawyers/lawyer5.jpg`
6. نورا محمد علي: `assets/images/lawyers/lawyer6.jpg`
7. يوسف أحمد حسن: `assets/images/lawyers/lawyer7.jpg`
8. ليلى عبدالله محمد: `assets/images/lawyers/lawyer8.jpg`
9. خالد محمد علي: `assets/images/lawyers/lawyer9.jpg`
10. مريم أحمد حسن: `assets/images/lawyers/lawyer10.jpg`

## 🛠️ **الخطوة 4: خطوات التنفيذ** | Step 4: Implementation Steps

### **1. نسخ الصور | Copy Images:**
```bash
# انسخ شعارك إلى مجلد الشعار
copy "C:\path\to\your\logo.png" "assets\images\logo\logo.png"

# انسخ صور المحامون إلى مجلد المحامون
copy "C:\path\to\lawyer1.jpg" "assets\images\lawyers\lawyer1.jpg"
copy "C:\path\to\lawyer2.jpg" "assets\images\lawyers\lawyer2.jpg"
# ... وهكذا لجميع الصور
```

### **2. تعديل ملف HTML | Edit HTML File:**
- افتح ملف `index.html`
- ابحث عن جميع روابط الصور
- استبدل كل رابط بالمسار المحلي المناسب

### **3. اختبار الموقع | Test Website:**
- افتح `index.html` في المتصفح
- تأكد من ظهور جميع الصور بشكل صحيح

## 💡 **نصائح مهمة** | Important Tips

### **لتحسين الأداء | For Performance:**
- **ضغط الصور | Compress images** قبل استخدامها
- **استخدم صيغة WebP** للحصول على أحجام أصغر
- **احتفظ بنسخة احتياطية** من الصور الأصلية

### **لتحسين SEO | For SEO:**
- **أضف alt text** وصفي لكل صورة
- **استخدم أسماء ملفات منطقية** مثل `ahmed-lawyer.jpg`

### **للتوافق | For Compatibility:**
- **اختبر على متصفحات مختلفة**
- **تأكد من عمل الموقع بدون اتصال بالإنترنت**

## 🔧 **أدوات مفيدة** | Useful Tools

### **لضغط الصور | For Image Compression:**
- [TinyPNG](https://tinypng.com/) - ضغط PNG و JPG
- [Squoosh](https://squoosh.app/) - أداة Google لضغط الصور
- [ImageOptim](https://imageoptim.com/) - لـ Mac

### **لتحويل الصيغ | For Format Conversion:**
- [Convertio](https://convertio.co/) - تحويل بين صيغ الصور
- [CloudConvert](https://cloudconvert.com/) - تحويل سحابي

## ❓ **استكشاف الأخطاء** | Troubleshooting

### **إذا لم تظهر الصور | If Images Don't Show:**
1. **تحقق من المسار | Check path** - تأكد من صحة المسار
2. **تحقق من اسم الملف | Check filename** - تأكد من تطابق اسم الملف
3. **تحقق من الصيغة | Check format** - تأكد من دعم المتصفح للصيغة

### **إذا كانت الصور كبيرة | If Images Are Too Large:**
1. **أعد تحجيم الصور | Resize images** إلى الحجم المطلوب
2. **اضغط الصور | Compress images** لتقليل الحجم
3. **استخدم صيغة WebP** للحصول على جودة أفضل وحجم أصغر

## 📞 **المساعدة** | Help

إذا واجهت أي مشاكل:
1. تحقق من أن جميع الملفات في المكان الصحيح
2. تأكد من صحة أسماء الملفات والمسارات
3. اختبر الموقع في متصفح مختلف

---

**ملاحظة | Note:** هذا الدليل يساعدك على استبدال الصور عبر الإنترنت بالصور المحلية الخاصة بك. تأكد من أن لديك حقوق استخدام الصور التي تضعها في الموقع. 