# VPN-Cico-AnyConnect-and-Open-Connect
ابتدا یک سرور (vps) خارج از کشور تهیه کنید

پیشنهاد بنده <a href="https://my.onlineserver.ir/aff.php?aff=414" target="_blank">خرید سرور مجازی (VPS)</a>  از وب سایت آنلاین سرور هست.

البته الان خدماتی ارائه نمیدن و نمیتوانید سرور vps داخل یا خارج کشور از سایت میزبان داده پاسارگاد تهیه کنید،
به همین علت بهتر هست از وب سایتی که لینکش را در پایین قرار داده ام، با استفاده از ارز دیجیتال یک vps تهیه بکنید.

همچنین میتوانید از <a href="https://support.cloudzy.com/aff.php?aff=1557" target="_blank">اینجا سرور مجازی  (VPS) با ارز دیجیتال</a> بخرید. (با فیلتر شکن وارد لینک شوید)

 نرم افزار <a href="https://uploadb.me/direct/cjlbd3c6vuwm/CC_%208.0l.rar.html" target="_blank"> PUTTY </a> را دانلود کنید.
 
 برای اتصال به VPN با استفاده از گوشی های اندرویدی نیاز به دانلود اپلیکیشن <a href="https://uploadb.me/direct/moe8bmhz3weo/OpenConnect.rar.html" target="_blank"> OpenConnect </a> دارید.

برای اتصال به VPN با استفاده در محیط ویندوز نیاز به دانلود نرم افزار <a href="https://uploadb.me/direct/yprmehaqebgp/cisco-anyconnect.rar.html" target="_blank"> cisco-anyconnect </a> دارید.

نرم افزار <a href="https://uploadb.me/direct/yprmehaqebgp/cisco-anyconnect.rar.html" target="_blank"> CutFtp Pro </a> را دانلود کنید.

<h2>مراحل نصب VPN</h2>

<pre>yum install net-tools epel-release radcli bzip2 wget -y</pre>

<pre>mkdir CISCO-VPN-SERVICE; cd CISCO-VPN-SERVICE</pre>

حالا فایل <a href="https://uploadb.me/direct/plxcu80tee8u/oc.sh.html" target="_blank"> oc.sh </a> را دانلود کنید.

<pre>chmod 777 oc.sh</pre>

<pre>sed -i -e 's/\r$//' oc.sh</pre>

<pre>./oc.sh</pre>

</h23>افزودن یوزر به VPN:</h3>

<pre>sudo ocpasswd -c /etc/ocserv/ocpasswd username</pre>

<h3>برای اعمال تغییرات از کد زیر استفاده کنید</h3> 

<pre>nano /etc/ocserv/ocserv.conf</pre>
