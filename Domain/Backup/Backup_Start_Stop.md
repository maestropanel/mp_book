# Yedek Başlatma/Durdurma

MaestroPanel'de planladığınız yedeklemeyi zamanlanmış bir görev olarak başlatabileceğiniz gibi istediğiniz zaman panel üzerinden sizde görevi başlatıp, durdurabilirsiniz.

Bunun için;

**Domainler > domain.com > Yedek > yedekelem planı > Başlat**

menüsünü takip edebilirsiniz.

## Başlatma

Bir yedekleme başlattığınızda Domain'e ait tüm modüllerin yedekleme fonksiyonları çalıştırılarak verilerin son durumları bir yere kopyalanır, sıkıştırılır ve hedef yedekleme alanına (Disk, FTP, UNC Path) gönderilir.

Bu aşamada her bir modül için yedekleme çalışır. Bu modüller hangi sunucdaysa o sunucu üzerindeki geçici alanda sıkıştırılır ve yine o sunucu üzerinden yedekleme alanına taşınır.

## Durdurma

Yedekleme başladıktan sonra çalışan yedekleme oprasyonlarına iptal komutu göndermek ve işlemi durdurmak için kullanabileceğiniz bir fonsiyondur.