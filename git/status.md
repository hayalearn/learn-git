<div dir="rtl" align= "right">

# نبذه عن git status

يتم استخدام الامر `git status`  لتوضيح حالة الملفات التي تم التعديل عليها والتي تمت اضافتها مؤخرًا ولم تتم متابعتها.

## كيفية كتابة الأمر
عند كتابة امر `git status` سوف تظهر هذه الرسالة:

<div dir="rtl" align="left">

```git
$ git status
On branch master
Your branch is up-to-date with 'origin/master'. nothing to commit, working directory clean
```

</div>
وتعني انك لم تقوم بمتابعة وتعديل اي ملف في المشروع الحالي.

## مثال 
### إضافة ملف
في حالة اضافة او تعديل اي ملف في المشروع سوف تختلف رسالة الامر `git status`

عند اضافة ملف README على المشروع الحالي سوف نقوم بإعادة الامر `git status` وستظهر الرسالة الآتية:

<div dir="rtl" align="left">

```git
$ git status
On branch master
Your branch is up-to-date with 'origin/master'. Untracked files:
(use "git add <file>..." to include in what will be committed) README
    nothing added to commit but untracked files present (use "git add" to track)
```

</div>

وتعني انك بحاجة لمتابعة ملف README عن طريق امر `$ git add README`

### تعديل ملف 

بعد إضافة ملف README عن طريق الامر السابق سوف نقوم بإعادة امر `git status` وستظهر الرسالة الآتية:

<div dir="rtl" align="left">

```git
$ git status
On branch master
No commits yet
Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md
```

</div>

وتعني انك بحاجة لتسجيل الملف عن طريق الامر `git commit -m 'your message'` لحفظ التغييرات التي قمت بها على الملف للمشروع.


</div>
