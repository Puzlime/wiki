## پازل های Messages

برای ارسال هرگونه پیامی از طرف بات از این پازل ها استفاده می کنیم.


### Forward message

این پازل برای forward پیام ها استفاده می شود.
در قسمت اول(مقابل message) این پازل شئ (object) مربوط به پیام را قرار می دهیم.
در قسمت دوم id مربوط به چت مقصد را قرار می دهیم.(گروه ، شخص خاص، کانال)

![messages-forward](img/messages-forward.png)

### Send message

برای ارسال پیام به صورت متن(text) از این پازل استفاده می کنیم.
در قسمت اول این پازل id چت مورد نظر را قرار می دهیم.
در قسمت دوم (مقابل message) متن مورد نظر خود را قرار می دهید.

![messages-send](img/messages-send.png)

قسمت آخر(options) برای کار های زیر استفاده می شود:

۱- نشان دادن کلید های inline

![messages-send-inline](img/messages-send-inline.png)

۲- نشان دادن کلید های ساده
 
![messages-send-reply](img/messages-send-reply.png)

۳- حذف کلید های ساده

![messages-send-reply2](img/messages-send-reply2.png)

۴- قرار گرفتن در حالت جواب دادن(reply) به یک پیام خاص

![messages-send-reply3](img/messages-send-reply3.png)

### Reply message

این پازل همانند پازل Send message است،
تفاوت این دو پازل در قسمت in reply to message است
که id مربوط به پیامی که می خواهیم به آن جواب دهیم را مقابل آن قرار می دهیم.

![messages-reply](img/messages-reply.png)

### Answer callback query



### Answer inline


## پازل های غیر متعارف

### ChatAction

اگر بات شما برای انجام فعالیتی زمان قابل ملاحظه ای را در بر می گیرد می توانید از این پازل استفاده کنید تا به کاربر اطلاع دهید که بات در حال فعالیت است و متوقف نشده است(به جای اینکه پیام بدهید مثلا "در حال پردازش اطلاعات")
برای نمونه می توانید بات [ImageBot](https://t.me/imagebot) را امتحان کنید.

![messages-send-chatAction](img/messages-send-chatAction.png)

زمانی که بات پردازش خود را انجام می دهد، زیر اسم بات متن sending photo... دیده می شود.
برای اینکار شما کافی است که یکی از متن های زیر را مقابل chatAction قرار دهید: 

1. typing 

2. upload_photo

3. upload_video, record_video

4. upload_audio, record_audio

5. upload_document

6. find_location

7. upload_video_note, record_video_note

### Send Location



### Send Venue



### Send Video Note



### Send Contact


