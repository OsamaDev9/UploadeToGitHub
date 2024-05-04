# رفع الملفات إلى GitHub
خطوات بسيطة لرفع مشروعك على GitHub.

**في البداية قم بالخطوات التالية:**
1- انشئ مستودع على GitHub 
2- قم بالدخول الى مجلد المشروع (على جهازك) الذي تريد رفعه الى مستودع GitHub الذي قمت بإنشائه ثم افتح windows powerShell او Git Bash Here في نفس مسار مجلد المشروع ثم تابع الخطوات التالية**
## الخطوة 1: ربط المشروع بمستودع GitHub

الان قم بربط ملفك أو مشروعك مع مستودع GitHub الذي قمت بإنشائه. باستخدام الأمر التالي:

```shell
git clone https://github.com/OsamaDev9/CallerID.git # رابط المشروع
```
سيتم إنشاء مجلد جديد بنفس إسم المستودع في هذا المثال سيكون اسم المجلد ```CallerID```

## الخطوة 2: فحص الملفات
بعد الانتقال إلى المجلد الرئيسي لمشروعك، يمكنك استخدام الأمر التالي لفحص الملفات:

```shell
ls
```
ستكون النتيجة على سبيل المثال
```shell
CallerID/  InfoNum.php  VI.php      script.js   styles.css
Images/    Os.php       index.html  search.php  visitor_ids.txt
```

## الخطوة 3: الانتقال إلى المجلد الذي تريد رفع الملفات إليه
إنتقل إلى المجلد الذي تريد رفع الملفات إليه (وهو المجلد الذي تم إنشائه عند الربط مع المستودع) باستخدام الأمر التالي:

```shell
cd CallerID
```
في هذه الخطوة قم بنقل الملفات الذي تود رفعها الى هذا المجلد على سبيل المثال هذه الملفات التي نريد رفعها :
```
InfoNum.php  VI.php      script.js   styles.css
Images/    Os.php       index.html  search.php  visitor_ids.txt
```
قم بنقلها او نسخها يدويا الى مجلد ``` CallerID ``` الذي قمنا بالدخول عليه.


## الخطوة 4: فحص الملفات بعد نقلها للمجلد المستهدف

استخدم الأمر التالي لفحص الملفات في المجلد المستهدف:

```shell
git status
```
ستكون النتيجة مشابهه للتالي
```bash
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Images/
        InfoNum.php
        Os.php
        VI.php
        index.html
        script.js
        search.php
        styles.css
        visitor_ids.txt

nothing added to commit but untracked files present (use "git add" to track)
```

## الخطوة 5: رفع الملفات

استخدم الأمر التالي لإضافة جميع الملفات لعملية commit:
```shell
git add *
```
## الخطوة 6: إجراء عملية commit

بعد إضافة الملفات، يمكنك إجراء عملية commit باستخدام الأمر التالي:

```shell
git commit -m "Uploade Done"
```
## الخطوة 7: رفع الملفات إلى GitHub

أخيرًا، قم برفع الملفات إلى مستودع GitHub باستخدام الأمر التالي:

```shell
git push
```

ستظهر رسائل تقدم معلومات حول العملية، وعند الانتهاء بنجاح، ستكون الملفات قد تم رفعها إلى مشروع GitHub الخاص بك.
