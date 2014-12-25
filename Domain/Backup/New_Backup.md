# Yeni Yedek

MaestroPanel'de Domain seviyesinde yedekleme yapabilirsiniz. Yedekleme sırasında Domain'in sahip olduğ tüm özellikleri, limitleri ve konfigürasyonu yedekler. Bu konfigürasyonun içinde FTP parolaları, Email hesaplarının parolaları ve Domain ile ilgili tüm parolalar şifrelenmiş bir şekilde tutulur ve yedeklenir.Yani MaestroPanel üzerinden yedek aldığınızda andaki konfigürasyonda yedeklenir ve geri döndüğünüzde o andaki parolalarla beraber döner.

MaestroPanel dosya sıkıştırma formatı olarak açık kaynaklı [7-Zip](http://www.7-zip.org/) formatını kullanır. Yedeklenen dosyalar bu format ile sıkıştırılıp depolama alanına kopyalanır ve yine geri yüklenmek istediğinde bu format açılarak ilgili yerlere geri yüklenir.

Yedekleme yapabilmek için;

**Domainler > domain.com > Yedekler > Yeni Yedekleme**

menüsünü takip edebilirsiniz.

![](https://lh3.googleusercontent.com/8U2p30WYYOZJpM0XlEGMXzBTiR9gDShalAFk5A1fuB4gN6u6fTsdUKpBaLWtFpbUdJVpe1E2aYkm9bAQ5GiKiKVg_8rJWqkm8JArfxXQWwSVJh3S87NGvFIE_Y0h0vTIYg)


**Hedef**

Yedeklemenin oluşturduğu dosyaları hangi depolama alanına aktarılacağını belirler. Hedef Yerel Disk, Uzak FTP veya  SMB Protokolü üzerinden bir UNC path olabilir.

**Açıklama**

Yedekleme ile ilgili bilgi girebileceğiniz zorunlu olmayan bir alandır. Yedekleme ile ilgil açıklayı bir cümle girmeniz tavsiye edilir. Örnek: "Günlük Yedekleme"

**Sadece Ayarların Yedeğini Al**

Yedekleme'nin sadece Domain'in konfigürasyonunun alınacağını, sahil oldukları özelliklerin verilerinin (Web site dosyaları, Veritabanı dosyaları) yedeklenmeyeceğini belirler.
Opsiyonel olarak kullanılabilmektedir.

Yedekler MaestroPanel Web Management Servisinde tutulur ve dizini aşağıdaki gibidir;


```
%MaestroPanelPath%\Web\Config\Backup
```

**Ayarların ve Verilerin Yedeğini Al**

Bu seçenek yedeklemenin hem konfigürasyon hemde Domain'in sahip olduğu özellikler kapsamında yapılacağını belirtir. Yedeklenen veriler hedef alanında seçilen depolama alanına kaydedilir. Konfigürasyon dosyası tekrar dan yukarıdaki belirtilen alana kaydedilir.

**Yedekleme Tamamlandığında Email Gönder**

MaestroPanel yedekleme tamamlandığında yedeklemenin başarılı veya başarısız olduğunu ve yedeklemenin ayrıntısını (Yedekleme Loglarını) belirtilen eposta adresine gönderir.

![](https://lh6.googleusercontent.com/jw35bfxifFOK_f4B-Nne5tfsLbcpwQ4U_APHPhMFvVU0QsLArbBvYyYFjxq7-CacUj52u53ImoqDUHFfCn626mGFTnpXPGeulHUXPUcLzXknccWArubF-3aXbX5vNIfmdg)

M
























S