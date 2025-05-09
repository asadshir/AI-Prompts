I’m looking for a free, open-source AI model that can be run on a regular PC without requiring expensive or high-end hardware, focused specifically on programming tasks. The goal is to use it for code generation and debugging in Pine Script v6 (TradingView). It doesn’t need to work offline — internet access is available. Ideally, the model should be trainable or customizable using online documentation (e.g., Pine Script v6 official docs), so it can learn from and specialize in this narrow domain. Please recommend the most suitable models, tools, or frameworks for this use case, with an emphasis on simplicity, focus, and low resource usage. Please provide your response in Persian (Farsi).

✅ انتخاب نهایی:
🔸 مدل: Phi-2 (ساخته Microsoft)
🔸 ابزار اجرا: Text Generation WebUI
مناسب برای تازه‌کارها چون رابط گرافیکی دارد و نیاز به کدنویسی زیاد ندارد.

می‌توانید با چند کلیک از مدل استفاده کنید.

## راه‌اندازی بهشت کدنویسی

1. **دانلود مدل Phi-2** از مخزن‌های متن‌باز (مثل GitHub یا منابع مشابه).
2. **نصب ابزار Text Generation WebUI** (از مخزن رسمی آن یا مستندات نصب).
3. **پیکربندی مدل Phi-2** در محیط Text Generation WebUI.
4. **بارگذاری مستندات Pine Script v6** به‌عنوان داده‌های آموزشی.
5. **تنظیمات مناسب برای تولید و اشکال‌زدایی کد Pine Script** در ابزار.
6. **اجرای مدل** و استفاده از آن برای تولید کد و اشکال‌زدایی.


## زیرساخت‌های جادوگر هوش مصنوعی

1. **سیستم عامل:** ویندوز، لینوکس یا macOS.
2. **فضای ذخیره‌سازی:** حداقل 10GB فضای خالی برای دانلود مدل و ابزار.
3. **پردازنده:** حداقل 4 هسته CPU.
4. **رم:** حداقل 8GB RAM.
5. **کارت گرافیک (اختیاری):** کارت گرافیک NVIDIA با پشتیبانی از CUDA برای سرعت بیشتر.
6. **نصب Python:** نسخه 3.7 یا بالاتر.
7. **نصب Git:** برای مدیریت مخزن‌های کد.
8. **نصب ابزارهای مورد نیاز:** pip، torch، transformers، webui و دیگر وابستگی‌های لازم.
9. **اتصال به اینترنت:** برای دانلود مدل و مستندات آنلاین.

 جزئیات مرحله 8: نصب وابستگی ها بعد از نصب گیت و کلون کردن پروژه **نصب ابزار Text Generation WebUI**
تست نصب پایتون
python --version
ساخت محیط مجازی:
1. در خط فرمان، ورود به آدرس کلون پروژه:     cd path/to/text-generation-webui
2. دستور ساخت محیط مجازی        python -m venv venv
3. فعال سازی محیط مجازی           venv\Scripts\activate
4. دستور نصب وابستگی ها             pip install -r requirements.txt
