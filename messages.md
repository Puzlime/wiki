# پازل های Messages

برای ارسال هرگونه پیامی از طرف بات از این پازل ها استفاده می کنیم.


## Forward message

این پازل برای forward پیام ها استفاده می شود.
در قسمت اول(مقابل message) این پازل شئ (object) مربوط به پیام را قرار می دهیم.
در قسمت دوم id مربوط به چت مقصد را قرار می دهیم.(گروه ، شخص خاص، کانال)

![messages-forward](img/messages-forward.png)

## Send message

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

## Reply message

این پازل همانند پازل Send message است،
تفاوت این دو پازل در قسمت in reply to message است
که id مربوط به پیامی که می خواهیم به آن جواب دهیم را مقابل آن قرار می دهیم.

![messages-reply](img/messages-reply.png)

