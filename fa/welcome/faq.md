---
refcn: chapter_00/faq
refen: welcome/faq
---
# سوالات متداول (FAQ)

## استفاده از V2Ray

### نحوه ارتقاء V2Ray

* آخرین بسته را دانلود کنید یا
* اجرای مجدد اسکریپت نصب (فقط لینوکس)

### سقوط V2Ray

* اگر از لینوکس با systemd استفاده می کنید، می توانید با استفاده از دستور `journalctl -u v2ray`.
* به طور کلی شما می توانید دستور `v2ray -config =<config-file> -test` را اجرا کنید تا اطلاعات خطا ببینید.

### Backward Compatibility

* For configuration file (e.g., JSON), backward compatibility applies to at least one major releases. For example, V2Ray 4.x supports config files from V2Ray 3.x.
* For Protobuf based communication protocols, such as [Api](../api.md), backward compatibility applies to at least one major releases.
* For binary based commnunication protocols, such as Shadowsocks and VMess, it is always backward compatible when server version is not older than clients. When client version is newer, backward compatibility applies to at least 12 minor releases.

## خطاهای V2Ray

### Socks: Unknown Socks version: 67

علل احتمالی

* You are using socks inbound in V2Ray, but your browser is configured to use HTTP proxy.

راه حل

* Add a HTTP inbound in V2Ray, and then update your browser proxy settings to use this proxy.

## مجوز این پروژه

پروژه V از مجوز زیر استفاده می کند.

### V2Ray

کد منبع و انتشار رسمی تحت مجوز MIT، از جمله کد منبع و انتشار در مخزن زیر مجوز.

* [v2ray/v2ray-core](https://www.github.com/v2ray/v2ray-core/)
* [v2ray/ext](https://www.github.com/v2ray/ext)

### V2Ray.Com

وب سایت رسمی، [v2ray.com](https://www.v2ray.com/)، تحت [Creative Commons Attribution 4.0 مجوز بین المللی](https://creativecommons.org/licenses/by/4.0/)مجاز است.

* Including all visible text and pictures on the website.
* Including <a href="https://www.v2ray.com/resources/v2ray_1024.png" target="_blank">Project V logo</a>.
* Including all source code that is used for generating the website, i.e., [v2ray/manual](https://www.github.com/v2ray/manual).

### Screenshot and other files {#screenshots}

تمام پرونده های شخص ثالث ذکر شده در زیر به خالق آنها تعلق دارند. هر شخصی که فایل را ایجاد می کند فایل دارد

* Including all screenshots of Project V.
* Including all configuration files that are used to run Project V.
* Including all logs generated by Project V during runtime.

### Other content {#other}

تمام محتویاتی که در بالا ذکر نشده اند، به صورت مورد صدور مجوز خواهند بود.