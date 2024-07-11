## مقدمه
در ابتدای کار پس از ساخت ریپو باید برای تقسیم وظایف بردمان را از طریق بخش projects ایجاد می‌کردیم. بعد از آن تسک هارا ایجاد 
کردیم و هر کدام را مرحله به مرحله موازی با انجام کارها جلو بردیم. بعضی از ایتم ها پس از انجام کارهای اولیه به برد اضافه شدند.
![Screenshot from 2024-07-11 15-29-19](https://github.com/MMVahedi/software-lab-report1/assets/79264910/03c5291e-7908-4b3d-b7e8-9fea6e7c685c)


تصویر بالا وصعیت برد بعد از انجام کارهای اولیه و مشخص شدن باقی آیتم ها است که بعضی از ایتم ها به مرحله done رسیده اند. به طور کلی ما چند کار اصلی داشتیم. ایجاد pipline برای استقرار صفحه وب، محافظت از شاخه main، ایجاد gitignore، ساخت قالب اولیه index.html و در انتها اضافه کردن دو ویژگی به آن. در ادامه به ترتیب به این مراحل می پردازیم.
## استقرار
برای اینکار مشابه تصویر زیر ما یک pipline برای استقرار وبسایتمان ایجاد کردیم. سایت هدف در آدرس https://mmvahedi.github.io/software-lab-report1/ قابل دسترس است.
![Screenshot from 2024-07-11 10-21-49](https://github.com/MMVahedi/software-lab-report1/assets/79264910/4c8f0443-9333-41c2-8d12-8ebcc4abbe05)
![Screenshot from 2024-07-11 10-24-22](https://github.com/MMVahedi/software-lab-report1/assets/79264910/f698010c-e279-42b3-b874-0ba97b47f2dd)


با اینکار با هر بار تغییر در شاخه main تغییرات بر روی سایت اعمال می‌شوند.
## محافظت از شاخه main
برای اینکار در تنظیمات github یک قانون برای شاخه main ایجاد میکنیم تا تنها با pull request بتوان آنرا تغییر داد و نیاز به یک تاییدیه هم داشته باشد.
![Screenshot from 2024-07-11 10-50-47](https://github.com/MMVahedi/software-lab-report1/assets/79264910/bdd23349-00c4-4435-935d-eef332f2782b)

نحوه مدیریت شاخه ها هم به این شکل است که ما یک شاخه dev داریم که مرحله قبل از main است. برای ایجاد هر تغییر و یا اضافه کردن ویژگی جدید یک شاخه از شاخه dev گرفته می‌شود و پس از پیاده سازی، با dev ادقام می‌شود. در نهایت برای اعمال تغییرات بر روی سایت، از روی dev به main یک pull request ایجاد میکنیم.

## ایجاد gitignore

برای اضافه کردن فایل .gitignore ابتدا یک برنچ فیچر میسازیم:

![Screenshot 2024-07-11 at 10.59.17 AM.png](https://github.com/MMVahedi/software-lab-report1/assets/70147234/acf65674-85dd-4c30-b3c9-f8248a8339ff)


حال فایل گیت ایگنور را میسازیم و آن را به گیت اد میکنیم:
![Screenshot 2024-07-11 at 11.10.19 AM.png](https://github.com/MMVahedi/software-lab-report1/assets/70147234/adcb06ed-4124-4103-8e95-10b8faff075b)


سپس این برنچ را با dev ادغام میکنیم و درخواست pull request میدهیم تا با main نیز ادغام شود:
![Screenshot 2024-07-11 at 11.14.51 AM.png](https://github.com/MMVahedi/software-lab-report1/assets/70147234/3dd2483c-e7f6-4a9b-b637-8260934d9ba5)
![Screenshot 2024-07-11 at 11.15.49 AM.png](https://github.com/MMVahedi/software-lab-report1/assets/70147234/1086bcc7-d748-44ef-b701-ca5d61907f1d)
![Screenshot 2024-07-11 at 11.24.38 AM.png](https://github.com/MMVahedi/software-lab-report1/assets/70147234/d4577f72-946c-4dd3-b6ad-b5192ade5d5e)
 ## ساخت قالب اولیه 
برای ساخت قالب اولیه و اضافه کردن پایه html به آن اول از همه یک شاخه با نام feature/base ایجاد می‌کنیم تا تغییرات را در آن اعمال کنیم. پس از انجام تغییرات و کامیت کردن آنها، آنها را پوش و بعد با شاخه dev ادغام می‌کنیم.
![Screenshot from 2024-07-11 15-15-34](https://github.com/MMVahedi/software-lab-report1/assets/79264910/81a552f8-5506-41e8-9ba1-5a15aae06aeb)

## اضافه کردن menue
در اینجا یک برنچ برای اضافه کردن فیچر منو میزنیم و سپس داخل ان برنچ که از dev ساخته شده تغییرات را انجام می‌دهیم.
در اینجا دکمه منو را اضافه می‌کنیم که کد آن در زیر آمده است:

![](https://github.com/MMVahedi/software-lab-report1/assets/70147234/4e091acb-b2c5-4927-b2eb-251e25d35dd4)
![](https://github.com/MMVahedi/software-lab-report1/assets/70147234/f839cb93-19e4-4a36-b0e0-6197f3d2f0ca)

همچنین برای زدن روی آن یک لیست نیز تعریف کردیم. سپس دقیقا مانند gitignore این تغییرات را کامیت می‌کنیم و پوش می‌کنیم و سپس با برنچ dev ادغام می‌کنیم. در آخر نیز یک pull request برای مرج شدن با main می‌دهیم:

![](https://github.com/MMVahedi/software-lab-report1/assets/70147234/2a964cc7-163c-481e-bedb-b8c8dda18046)



بعد از ادغام dev با main متوجه یک مشکل در کد شدیم که باعث می‌شد تصویر پسزمینه دوبار نمایش داده شود. برای رفع این مشکل یک شاخه fix/background ایجاد کردیم و تغیرات را در آن اعمال کنیم. چون دو نفر همزمان بر روی این شاخه کار می‌کردیم هنگام push کردن روی آن به یک conflict خوردیم و مجبور شدیم آن را resolve کنیم.
![Screenshot from 2024-07-11 13-57-07](https://github.com/MMVahedi/software-lab-report1/assets/79264910/54232553-d4d2-4374-ad02-f40a7d53809e)
![Screenshot from 2024-07-11 15-24-12](https://github.com/MMVahedi/software-lab-report1/assets/79264910/2a5d5b3b-5b44-4f85-9988-4913e17e0775)
![Screenshot from 2024-07-11 15-24-23](https://github.com/MMVahedi/software-lab-report1/assets/79264910/1a08574e-d5cc-4c9d-b2e9-982e4c7b4e10)



## اضافه کردن contact

<hr/>
در اینجا ما دکمه ی کانتکت در بالا سمت چپ اضافه شده که وقتی روی ان کلیک کنیم یک کانتکت خالی می اید.

پس از زدن دکمه یک متن نوشته میشود.

فرم ساخته میشود و اسم و مسیج و تعداد افرادی که میخواهند بیاید اضافه میشود.

یک دکمه اضافه شده.

تاریخ اضافه شده.

امکان خالی بودن فیلد ها حذف شده و حتما همه باید پر شوند.

اپشن ها ری فرمت شدند و متن دکمه تغیر کرد.


![image](https://github.com/user-attachments/assets/966e9f3f-5e83-4dce-a8f8-ad08871a6401)

![image](https://github.com/user-attachments/assets/983c957c-6c00-4735-8b85-995dc4a9747b)

![image](https://github.com/user-attachments/assets/5d2dff8f-2f3b-41bb-b574-50d3231b6daa)

![image](https://github.com/user-attachments/assets/4f51200a-e254-45ca-9532-3e8181cdad99)

![image](https://github.com/user-attachments/assets/86259f50-c919-46e9-891a-efbe9af45d73)

### گزارش
در انتهای کار هم پس از نوشتن گزارش در README و در شاخه feature/doc، هنگام ادقام آن با dev یه یک conflict دیگر برخوردیم.
![Screenshot from 2024-07-11 22-19-44](https://github.com/user-attachments/assets/6070f9aa-f107-4612-be27-7e02d21e64d7)
![Screenshot from 2024-07-11 22-20-02](https://github.com/user-attachments/assets/154a18db-c06b-4a06-bc11-20b940df6e52)



## پاسخ سوالات

سوال اول - در پوشه‌ی .git همه‌ی اطلاعات مورد نیاز برای اینکه گیت بتواند تغییرات کدبیس ما را مشاهده و شناسایی کند ذخیره شده است. این اطلاعات شامل کامیت‌ها، کامنت‌های مربوط به آنها، برنچ‌ها، تگ‌ها، نام و ایمیل نویسنده، و زمان تغییرات است. برای ایجاد این دایرکتوری کافی است که از دستور git init استفاده کنیم.

 
سوال دوم - منظور از atomic بودن این است که در هر کامیت تنها یک کار به صورت مجزا باید انجام شود و کامیت های مربوط به bugfix، refactoring  یا features  باید از هم جدا شوند. از کامیت کردن تغیرات متعدد به صورت یکجا پرهیز شده و هر کامیت باید تنها یک گام به حالت مورد نظر را در برگیرد. هر کامیت به معنای یک snapshot  از پروژه میباشد پس باید کد را در حالت valid نگه دارد.
برای Atomic pull request تا حد ممکن باید pull requestها به کار های کوچک تر شکسته شده تا review کردن انها در مدت زمان کوتاه تر انجام شود. به عبارتی به جای یک تسک بزرگ کار ها به تعدادی task و issue کوچک تقسیم میشوند که هر یک در قالب یک PR قابل اجراست.


سوال سوم - دستور fetch تغییرات شاخه‌های ریموت را به مخزن محلی منتقل می‌کند بدون اینکه آن‌ها را با شاخه‌های فعال ادغام کند. در واقع این امکان را به ما می‌دهد که تغییرات را ببینیم و در صورت نیاز، آن‌ها را ادغام نماییم.

دستور merge تغییرات یک شاخه را با شاخه‌ی دیگر ادغام می‌کند و یک کامیت جدید ایجاد می‌کند که تغییرات هر دو شاخه را ترکیب می‌کند.

دستور rebase تغییرات یک شاخه را بر روی شاخه‌ی دیگر بازنویسی می‌کند. این دستور به ما اجازه می‌دهد تا تغییرات یک شاخه را به صورت خطی و بدون ایجاد تعارض (conflict) ادغام کنید.

دستور pull یک ترکیب از fetch و merge است. این دستور تغییرات شاخه‌های ریموت را به مخزن محلی ما دانلود و سپس با شاخه فعال ادغام می‌کند.

دستور cherry-pick نیز برای انتقال کامیت‌ها بین برنچ‌ها استفاده می‌شود که این امکان را می‌دهد یک کامیت خاص را انتخاب و انتقال دهید.


سوال چهارم - دستور revert یک commit جدید ایجاد میکند که ما را به commit قبلی برمیگرداند و در تاریخچه موجود ما تغییری اعمال نمی شود.
دستور checkout چند کار متفاوت انجام می دهد یکی از آنها جا به جا شدن بین Branch های مختلف است و دیگری Undo change کردن فایلی که هنوز بر روی stage نرفته و چند کاربرد دیگر که در ویدئو ها بررسی شده.
دستور reset این دستور برای این است که به یک نقطه خاص از تاریخچه ای که داریم بازگردیم که در ویدئو ها بررسی شده است.
دستور Git restore این دستور تمامی تغییرات را تا آخرین کامیتی که انجام شده است عقب میبرد Git switch تنها برای جا به جایی بین برنچ ها انجام میشود.


سوال پنجم - استیج اشاره به یک ناحیه میانی است که در آن تغییرات برای آینده‌ی commit تجمع پیدا کنند. در واقع وقتی فایل‌هایی را "stage" می‌کنیم، به Git اعلام می‌کنیم که قصد داریم این تغییرات را در نسخه بعدی که commit خواهیم کرد، ضمیمه کنیم. این کار با دستور git add انجام می‌شود. 
دستور git stash، این دستور برای ذخیره‌سازی موقت تغییرات فعلی در workspace استفاده می‌شود که هنوز به stage اضافه نشده‌اند یا commit نشده‌اند. یعنی اجازه می‌دهد که پاکسازی موقتی از تغییرات داشته باشیم و به سراغ بقیه کارها برویم بدون اینکه نیاز باشد تغییرات فعلی را commit کنیم. می‌توانیم بعدا این تغییرات را با استفاده از دستور git stash pop بازیابی کنیم تا به کار روی آن‌ها ادامه دهیم.

سوال ششم - مفهوم snapshot در یک پروژه گرفتن یک تصویر از وضعیت کلی پروژه در یک زمان خاص است.به طوری که به دایرکتوری‌ها، فایل‌ها و تاریخچه فایل‌ها دسترسی داشته‌باشیم. همچنین در git به عنوان یک commit ثبت می‌شود‌.

سوال هفتم - مخزن محلی (Local repository) یک نسخه از مخزن است که روی دستگاه شخصی ما قرار دارد و می‌توانید با استفاده از دستورات commit آن را به‌روزرسانی کنیم. اما زمانی که می‌خواهیم با دیگران به صورت مشترک روی کد کار کنیم باید این مخزن را به یک سرور مانند گیتهاب منتقل کنیم که به آن مخزن دور (Remote repository) می‌گویند. این مخزن دور با استفاده از دستور push اطلاعات را از مخزن محلی دریافت می‌کند و با دستور pull اطلاعات را به آن ارسال می‌دارد.
