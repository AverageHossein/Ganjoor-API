<h1 align="center">
	<img width="200" src="static/ganjoor.jpg" alt="Aur">
	<br>
	<br>
</h1>

<div dir="rtl">
	<h1>API ارتباط با سایت گنجور توسعه داده شده توسط فریمورک فلسک</h1>
</div>
<div dir="rtl">
	<h3>نصب روی سرور شخصی</h3>
</div>

ابتدا دیتابیس <a href='https://github.com/ganjoor/ganjoor-db'>گنجور </a> رو clone کنید:


<div dir="rtl">
	ابتدا دستور زیر را در خط فرمان وارد کنید:
</div>

`sudo pip install -r requirements.txt`
<br />

<div dir="rtl">
	سپس وارد دایرکتوری اصلی شده و دستور زیر را وارد کنید:
</div>

`flask run`
<br />

<div dir="rtl">
	<h3>نحوه استفاده از API</h3>
</div>

<div dir="rtl">
	<h4>لیست شاعران به همراه ID هایشان</h4>
	هر شاعر دارای یه ID هست، برای اینکه بایوگرافی شاعر رو در بیارید به این ID نیاز دارید.

</div>


`http://host/poets`
<br />



<div dir="rtl">
	<h4>بیوگرافی شاعر مدنظر</h4>
	کافیه به جای <code>POETId</code> در ریکوئست پایین Id شاعر مدنظر رو که از ریکوئست بالابرداشتید وارد کنید.

</div>


`http://host/poet?id=POETID`
<br />


<div dir="rtl">
	<h4>انتخاب شعر به صورت تصادفی</h4>
</div>

`http://host/random`
<br />


<div dir="rtl">
	<h3>گلاسری شاعران</h3>
</div>

<div dir="rtl">
برای اینکه بتونید یک شعر تصادفی از یک شاعر خاص داشته باشید، می‌تونید به گلاسری زیر ریکوئست بزنید تا نوشتار انگلیسی نام‌ شاعر‌ها رو ببینید.

</div>


`http://host/glossary`
<br />



<div dir="rtl">
	<h4>انتخاب شعر تصادفی از شاعری خاص</h4>
	حالا کافیه اسم شاعری که از glossary بالا انتخاب کردید رو اینجا وارد کنید، برای مثال حافظ:

</div>

`http://host/random/hafez`
<br />

