<div dir="rtl">

# مشکل چیه ؟

خب مشکل از اونجا شروع میشه که وقتی مترجم عزیز میخواد زیرنویسش رو ذخیره کنه، انکدی(Encode) رو که باید انتخاب کنه درست انتخاب نمی کنه.

برای آشنایی بیشتر با اندکینگ به این لینک رجوع کنید. نتیجه اش اینه که وقتی من و شما که می خواهیم تو سیستم های مختلف زیرنویس رو ببینیم سیستم نمی تونه تخشیص بده که اندک این زیرنویس چیه و در نتیجه چیزای خرچنگ قورباغه ای می بینیم.

برای کسایی که توی لینوکس اومدن این مشکل همیشه وجود داره و برای درست کردنشم هم من اسکریپت پایینو نوشتم.

# نصب
## پیش نیازها:
۱. یه برنامه خیلی ساده به اسم sponge استفاده شده که توی پکیج moreutils قرار داره.چطور توی اوبونتو نصب اش کنم ؟

<div dir="ltr">

`# apt-get install moreutils`
</div>

## نصب خود برنامه

برای نصب این برنامه کافیه دستور زیر رو کپی کنید و توی ترمینالتون اجرا کنید : 
<div dir="ltr">

`git clone https://github.com/GreatBahram/Fix_Persian_Subtitle`
</div>

این دستور اسکرپت رو کپی می کنه توی سیستمتون و تنها کاری که میمونه اینه بهش مجوز اجرا شدن بدیم و یه جایی کپیش کنیم که همیشه تو ترمینال قابل دسترسی باشه: 
<div dir="ltr">

‍`cd Fix_Persian_Subtitile`

`chmod 755 sub-fixer`

`ln -sf $(pwd)/sub-fixer /usr/bin/sub-fixer`
</div>
# نحوه استفاده:

این برنامه رو میشه دوجور استفاده کرد:

*اول اینکه بگیم بهش بگیم فلان زیر نویس رو درست کن: که چک میکنه اگه مشکل داشته باشه،‌ فقط اون زیرنویس رو درست می کنه:‌

<div dir="ltr">

`$ sub-fixer [Name-of-Your-Subtile]` 
 
```
cd Download/Batman-vs-Superman/
sub-fixer batman-1080.srt
```
</div>
*دومین روش همه رو باهم: برای اینکار به دایرکتوری مورد نظر میریم و برنامه رو اجرا می کنیم و به صورت خودکار همه فایل های srt رو چک می کنه اگه هرکدوم مشکلی داشته باشن درستشون می کنه 

<div dir="ltr">

`$ sub-fixer `

```
cd Downloads/Batman-vs-Superman/
ls 
batman-480.srt batman-720.srt batman-1080.srt
sub-fixer
```
</div>


</div>
