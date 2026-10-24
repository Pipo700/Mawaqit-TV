# مواقيت TV
Launcher لشاشات Android TV: ساعة + تاريخ هجري + مواقيت صلاة أوفلاين (طريقة الهيئة المصرية، القاهرة) + عدّاد + تطبيقات مفضلة + إذاعة القرآن.

## بناء الـ APK
### الطريقة 1: GitHub Actions (بدون Android Studio)
1. اعمل Repository جديد على GitHub وارفع محتويات هذا المجلد كلها (بما فيها `.github`).
2. افتح تبويب Actions ← Build APK ← انتظر ~5 دقائق.
3. نزّل `MawaqitTV-apk` من Artifacts، وجواه `app-debug.apk`.

### الطريقة 2: Android Studio
افتح المجلد ← انتظر Gradle Sync ← Build > Build APK(s).
الملف في `app/build/outputs/apk/debug/app-debug.apk`

## التثبيت على الشاشة
adb connect IP_الشاشة:5555
adb install app-debug.apk
ثم اضغط زر Home واختر "مواقيت TV" > Always.
