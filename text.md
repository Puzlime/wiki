# متن

## مثال هایی برای پازل های متن

* "thing #1"
* "12،مارچ،2010"
*""(رشته خالی)
متن می تواند شامل حروف(حروف بزرگ یا حروف کوچک)، اعداد، علائم نقطه گذاری و فضای خالی بین کلمات.(به تمام این ها کاراکتر می گوییم)


# پازل ها

## ایجاد متن

پازل زیر متن hello را می سازد و در متغیری به نام greeting ذخیره می کند.

![text-text](img/text-text.png)

پازل create text with مقدار متغیر greeting و متن جدید "world" را باهم ادغام می کند. برای ساخت "helloworld" توجه کنید که فاصله ای بین آن ها نیست چون در متن اصلی فاصله ای وجود ندارد.

![text-create](img/text-create.png)

برای افزایش تعداد متن های ورودی روی ایکون چرخ دنده کلیک کنید که شکل » را تغییر می دهد به: 

![text-create-modify](img/text-create-modify.png)

ورودی های اضافی با کشیدن از قسمت جعبه ابزار طوسی که در چپ قرار دارد به داخل قسمت join اضافه می شوند.

# ویرایش متن

پازل to ... append text متن داده شده را به متغیر خاصی اضافه می کند. در این حالت مقدار متغیر greeting را از "hello" به "hello,there" تغییر می دهد.

![text-create-modify](img/text-create-modify.png)

# طول متن

پازل length of تعداد حروف، اعداد و غیره را در هر متنی می شمارد. طول متن "we're#1!" 9 می باشد و طول رشته خالی 0 می باشد.

![text-length1](img/text-length1.png)

![text-length2](img/text-length2.png)

# بررسی کردن متن خال

پازل isempty بررسی می کند که آیا متن داده شده خالی است یا نه. در مثال زیر در حالت اول نتیجه درست است و در حالت دوم غلط.

![text-empty1](img/text-empty1.png)

![text-empty2](img/text-empty2.png)

# پیدا کردن متن

این پازل ها می توانند برای این استفاده شوند که آیا قسمتی از متن در متن دیگری وجود دارد،اگر وجود دارد کجای متن ظاهر شده است. برای مثال ظاهر شدن اولین e را در hello می پرسد که نتیجه 2 می شود.

![text-find-first](img/text-find-first.png)

![text-find-last](img/text-find-last.png)
این  مثال در مورد آخرین ظاهر شدن حرف e در hello می پرسد که جواب همچنان ۲ می باشد. 

![text-find-last](img/text-find-last.png)

اگر اولین یا اخرین  حرف انتخاب شود این پازل جواب صفر برمی گرداند چون "hello" دارای حرف "z" نمی باشد.

![text-find-first-last](img/text-find-first-last.png)

# استخراج متن

## استخراج یک کاراکتر

این پازل "b" را به عنوان دومین حرف "abcde" بر می گرداند :

![text-in-text-get1](img/text-in-text-get1.png)

این پازل "d" را به عنوان دومین حرف از آخر "abcde" بر می گرداند :

![text-in-text-get2](img/text-in-text-get2.png)

این پازل "a" را به عنوان اولین حرف "abcde" بر می گرداند :

![text-in-text-get3](img/text-in-text-get3.png)

این پازل "e" را به عنوان آخرین حرف "abcde" بر می گرداند :

![text-in-text-get4](img/text-in-text-get4.png)

این پازل هر 5 حرفی که در "abcde" که احتمال یکسانی داشته باشد را برمی گرداند :

![text-in-text-get5](img/text-in-text-get5.png)

هیچکدام از این پازل ها متنی را که از آن استخراج می کنیم را ویرایش نمی کند.

# استخراج قسمتی از متن

در پازل in text ... get substring اجازه می دهد که قسمتی از متن جدا شود، که شروع آن :

* letter #

* letter # from end

* the first letter

 و پایان آن :
 
 * letter #
 
 * letter # from end
 
 * the last letter

در مثال زیر، "abc" استخراج می شود.

![text-get-substring](img/text-get-substring.png)

## سازگار کردن قالب متن

این پازل مدلی از ورودی متن را بر اساس یکی از موارد زیر ایجاد می کند : 

* UPPER CASE (تمامی حروف بزرگ)

* lower case (تمامی حروف کوچک)

* Title Case (حرف اول بزرگ، بقیه کوچک)

نتیجه پازل زیر "HELLO" می شود.

![text-case](img/text-case.png)

حروفی که در الفبای انگلیسی وجود ندارند تحت تاثیر قرار نمی گیرند. توجه کنید که این پازل روی متن هایی که زبانشان چندین مدل ندارد مانند چینی تاثیر ندارد.

## حذف فاصله 

پازل زیر، از قسمت های زیر فاصله را حذف می کند : 

* شروع متن

* پایان متن

* هر دو قسمت متن

نتیجه پازل زیر "hi  there" است.
(فضای خالی متن تاثیر ندارد.)

![text-trim-spaces](img/text-trim-spaces.png)
