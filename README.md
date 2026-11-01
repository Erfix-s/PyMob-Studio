# PyMob Studio 🐍📱

اپ اندروید اجرای پایتون با OpenCV/NumPy — نوشتن کد، نصب کتابخانه و پردازش تصویر مستقیم از حافظهٔ گوشی.

## بیلد روی گیت‌هاب (فقط ۳ قدم)
1. فایل `files.zip` را در ریپازیتوری آپلود کنید.
2. فایل `android.yml` را در مسیر `.github/workflows/android.yml` قرار دهید.
3. تب Actions → بعد از اتمام، APK را از Artifacts دانلود کنید.

## استفاده در اپ
- 🖼 انتخاب تصویر از گالری (خواندن مستقیم، بدون کپی)
- `imread()` خواندن تصویر به‌صورت آرایهٔ OpenCV
- `show_image(img)` نمایش خروجی در پنل تصویر
- `save_image(img, "path.png")` ذخیرهٔ خروجی
- تب «کتابخانه‌ها» برای نصب پکیج با pip

## نمونه کد
```python
img  = imread()
gray  = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
edges = cv2.Canny(gray, 100, 200)
show_image(edges)
```

فهرست پکیج‌های قابل نصب: https://chaquo.com/pypi-13.1/
لایسنس: MIT