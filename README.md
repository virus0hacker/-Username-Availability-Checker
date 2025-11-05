# -Username-Availability-Checker

Author: ml-ftt
Language: Python
Interface: GUI (Tkinter)

🔍 Overview

أداة سهلة الاستخدام للتحقق من توافر أسماء المستخدمين عبر أشهر المنصات الاجتماعية:

Snapchat

Twitter / X

Instagram

Telegram

(ملاحظة: Discord لا يوفّر واجهة عامة للتحقق من الأسماء، ويُدرج كـ "غير قابل للفحص المباشر")


⚙️ Features  :

✅ Quick cross-platform username check
✅ Simple and elegant dark green graphical user interface (GUI)
✅ Color-coded results display (Available/Used/Unknown)
✅ Batch input of multiple usernames
✅ Export results in CSV or JSON format
✅ Works without requiring any account or login
✅ فحص سريع لأسماء المستخدمين عبر منصات متعددة
✅ واجهة رسومية (GUI) بسيطة وأنيقة باللون الأخضر الداكن
✅ عرض النتائج بالألوان (متاح / مستخدم / غير معروف)
✅ إمكانية إدخال قائمة أسماء متعددة دفعة واحدة
✅ تصدير النتائج بصيغة CSV أو JSON
✅ يعمل دون الحاجة إلى أي حساب أو تسجيل دخول


💻 Installation :

pip install requests
python username_availability_checker.py


How it works :

This script sends HTTP requests to public user pages on each platform and infers from the status codes and page text whether a name is in use.

Status Color Meaning
✅ 200 or Redirect 🔴 Taken Name is in use
⚙️ 404 or "not found" text 🟢 Available Name is available
⚠️ Any other status ⚪ Unknown Unconfirmed

السكربت يقوم بإرسال طلبات HTTP إلى صفحات المستخدمين العامة لكل منصة،
ويستنتج من رموز الاستجابة (Status Codes) ونص الصفحة ما إذا كان الاسم مستخدمًا أم لا.

الحالة	اللون	المعنى
✅ 200 أو Redirect	🔴 Taken	الاسم مستخدم
⚙️ 404 أو نص "not found"	🟢 Available	الاسم متاح
⚠️ أي حالة أخرى	⚪ Unknown	غير مؤكد


🔒 Privacy & Safety :

No sensitive data is transmitted, and no accounts are accessed.

All scans are performed locally on the user's device.

لا يتم إرسال أي بيانات حساسة أو الدخول إلى الحسابات.

جميع عمليات الفحص تتم محليًا في جهاز المستخدم.

📦 Output :

Easily save results:

CSV file: Suitable for analysis in Excel or Google Sheets

JSON file: For programmatic use or data storage

يمكن حفظ النتائج بسهولة:

ملف CSV: مناسب للتحليل في Excel أو Google Sheets

ملف JSON: للاستخدام البرمجي أو حفظ البيانات

Username: example_user
Twitter: taken
Instagram: available
Telegram: taken
Snapchat: available
Discord: unknown


🏷️ License

MIT License — free for personal & research use.
