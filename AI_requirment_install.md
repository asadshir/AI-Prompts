00-  https://visualstudio.microsoft.com/visual-cpp-build-tools/
✅ مواردی که باید حتماً انتخاب کنی:
این‌ها ضروری هستن برای اینکه نصب torch و سایر ابزارها بدون خطا انجام بشه:
✔ MSVC v143 - VS 2022 C++ x64/x86 build tools
✔ Windows 11 SDK (10.0.22621.0) ← این نسخه از SDK رایج‌ترین نسخه پایدار برای ویندوز 11 هست.
✔ C++ CMake tools for Windows
🟡 موارد اختیاری (فقط اگر فضای کافی داری و آینده‌نگر هستی):
اگر فضای کافی داری (که گفتی داری)، این‌ها می‌تونن در آینده مفید باشن:
⭕ vcpkg package manager ← ابزار قدرتمندی برای مدیریت پکیج‌های C++
⭕ C++ AddressSanitizer ← مفید برای بررسی خطاهای حافظه، اگر بخوای در آینده کدنویسی C++ انجام بدی
⭕ C++/CLI support for v143 build tools (Latest) ← اگر روزی بخوای C++ رو با .NET ترکیب کنی
⭕ C++ Clang tools for Windows (19.1.1 - x64/x86) ← اگر بخوای از کامپایلر Clang استفاده کنی

0- notepasd++
1- Python
2- Git
3- Github desktop



گزارش هوش مصنوعی از مراحل کار
حتماً! در ادامه، یک **خلاصه تیتر‌وار و کامل** از تمام مراحل پروژه‌ی راه‌اندازی مدل هوش مصنوعی سبک و آزاد برای برنامه‌نویسی مخصوصاً Pine Script در ویندوز (با تأکید بر سادگی، منابع کم، و قابلیت شخصی‌سازی) از ابتدا تا اینجا آورده‌ام — بدون حذف هیچ مورد ضروری:

---

### ✅ خلاصه مراحل انجام‌شده تا کنون:

1. **نصب پایتون (Python)**

   * دانلود از سایت رسمی:
     🔗 [https://www.python.org/downloads/windows/](https://www.python.org/downloads/windows/)
   * نسخه پیشنهادی: Python 3.10 یا بالاتر (ترجیحاً 3.10 تا 3.11 برای سازگاری بهتر)
   * تیک گزینه‌ی **Add Python to PATH** در ابتدای نصب ✅
   * تست نصب در CMD:

     ```bash
     python --version
     ```

2. **نصب Git**

   * دانلود از سایت رسمی گیت:
     🔗 [https://git-scm.com/download/win](https://git-scm.com/download/win)
   * تفاوت با GitHub Desktop: Git ابزاری خط فرمانی است و برای clone و version control ضروری است.
   * طی نصب، تنظیمات پیشنهادی:

     * Editor: می‌تونی پیش‌فرض (Vim) رو نگه داری یا مثلاً Notepad++ رو انتخاب کنی.
     * Branch name: بهتره "Let Git decide" رو رها کنی یا مستقیماً `main` رو انتخاب کنی (برای آینده بهتره).
     * PATH: گزینه دوم (پیش‌فرض) مناسب است.
     * SSH: گزینه پیش‌فرض Git.
     * HTTPS transport backend: پیش‌فرض (curl).
     * Line endings: پیش‌فرض (Checkout Windows-style, commit Unix-style).
     * Terminal emulator: Use MinTTY (پیش‌فرض) خوبه.
     * Git Pull behavior: Merge (پیش‌فرض) خوبه.
     * Credential helper: انتخاب پیش‌فرض مناسب است.
     * Additional options:

       * ✅ Enable file system caching
       * ✅ Enable symbolic links (اختیاری ولی مفید)

3. **ری‌استارت سیستم پس از نصب Git**

   * پس از ری‌استارت، تست دستور گیت در خط فرمان:

     ```bash
     git --version
     ```

4. **ساخت مسیر مناسب برای پروژه**

   * در درایو E پوشه‌ای ساختی به نام:

     ```
     E:\AI\webui
     ```

5. **کلون کردن مخزن Web UI مدل سبک و کاربردی**

   * دستور:

     ```bash
     git clone https://github.com/oobabooga/text-generation-webui.git
     ```
   * در مسیر `E:\AI\webui`

6. **ورود به پوشه کلون‌شده و نصب وابستگی‌ها**

   * ورود:

     ```bash
     cd text-generation-webui
     ```
   * نصب وابستگی‌ها:

     ```bash
     python launch.py
     ```

7. **ارور در نصب برخی پکیج‌ها مانند numpy و pillow-avif-plugin**

   * دلیل اصلی: عدم وجود ابزار کامپایل C/C++ در سیستم ویندوز (برای ساخت برخی پکیج‌ها لازم است).

8. **تصمیم برای نصب ابزار Visual Studio Build Tools**

   * دانلود از این لینک:
     🔗 [https://visualstudio.microsoft.com/visual-cpp-build-tools/](https://visualstudio.microsoft.com/visual-cpp-build-tools/)
   * در بخش نصب:

     * انتخاب Workload: ✅ **Desktop development with C++**
     * در Installation details، گزینه‌های پیش‌فرض کافی هستند اما:

       * ✅ MSVC v143 - VS 2022 C++ x64/x86 build tools
       * ✅ Windows 11 SDK (10.0.22621.0) (یا نسخه‌ای نزدیک)
       * ❗ انتخاب دقیق با توجه به نسخه ویندوز

9. **در حال حاضر: نصب Visual Studio Build Tools در حال انجام است (حجم تقریبی: 17 گیگ)**

---

اگر موافق باشی، پس از پایان نصب Build Tools و ری‌استارت سیستم، مرحله بعدی نصب مجدد پکیج‌هایی است که خطا داده بودند (مثل `pillow-avif-plugin` و `numpy`) و سپس راه‌اندازی مدل مورد نظر.

آیا دوست داری بعد از نصب، دقیق بگم چه دستوراتی بزنی تا پکیج‌های خطادار با موفقیت نصب بشن؟

