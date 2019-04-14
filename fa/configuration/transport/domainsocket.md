---
refcn: chapter_02/transport/domainsocket
refen: configuration/transport/domainsocket
---
# سوکت دامنه حمل و نقل

سوکت دامنه از سوکت دامنه یونیکس استاندارد برای انتقال اطلاعات استفاده می کند. سوکت دامنه کانال tranfer سیستم تعاملی است. این بافر شبکه را مسدود نمیکند و ممکن است کمی سریعتر از ترافون کردن از طریق شبکه loopback محلی باشد.

سوکت دامنه تنها می تواند در سیستم عامل هایی که سوکت دامنه یونیکس را پشتیبانی می کنند، مانند macOS و لینوکس استفاده شود. این در ویندوز موجود نیست

{% hint style='info' %}

هنگام استفاده از سوکت دامنه، IP و پورت مشخص شده در پروکسی ورودی / خروجی نادیده گرفته خواهند شد. تمام ترافیک از طریق سوکت دامنه تونل شده است.

{% endhint %}

## DomainSocketObject

`DomainSocketObject` در `dsSettings` فیلد در `TransportObject` و `StreamSettingsObject`.

```javascript
{
  "path": "/path/to/ds/file"
}
```

> `مسیر`: رشته

یک مسیر فایل کامل معتبر قبل از اجرای V2Ray، فایل در این مسیر نباید وجود داشته باشد.