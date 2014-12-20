## Kurulum (Windows)

Sunucunuza MaestroPanel.exe yi indirdikten sonra herhangi bir ayar yapmadan direkt Administrator kullanıcı hakları ile çalıştırıp kuruluma başlayabilirsiniz.
**MaestroPanel.exe** dosyasını çalıştırdığınızda karşınıza ilk olarak MaestroPanel'in hangi dizine kurulacağını belirleyebileceğiniz A1 ekranı gelecektir.

Varsayılan olarak olarak *C:\Program Files\MaestroPanel* klasörü hedef gösterilmiştir. Setup bu dizini gerektiği şekilde oluşturup güvenliğini sağlayarak kuruluma başlayacaktır. 
Dosya yolunun arasında boşluk olması MaestroPanel için sorun değildir.

Kurulum dizinini belirledikten sonra Next butonuna basıp bileşenleri seçebileceğimiz bir sonraki
ekrana geçiş yapabiliriz. 

Ekran A1

Bu ekranın en üstünde önceden tanımlanmış bileşen kombinasyonlarını içeren şablonlar bulunmaktadır. Kurulmasını istediğiniz bileşenleri tek tek seçebileceğiniz gibi şablonları kullanıp ideal seçimlerde yapabilirsiniz.

Ekran A2

#### Şablonlar ve Açıklamaları


**Full Hosting Environment (Agent + Web Management):**

Hem MaestroPanel Agent hemde Web Management Servisi ile alakalı tüm bileşenleri kurar.

**Standart Hosting Environment (Only Agent): **

Sadece MaestroPanel Agent'ı ve paylaşımlı hosting için gerekli olan standart bileşenleri seçer.

**Light Hosting Environment (Only Agent):**

Sadece MaestroPanel Agent'ı ve çok temel olan ihtiyacı karşılayacak paylaşımlı hosting bileşenlerini kurar.

İstenilen bileşenler seçildikten sonra Next butonuna basıp diğer ekrana geçebilirsiniz

Ekran A3

Bu ekranda panel'e erişebilmeniz için gerekli olan kullanıcı adı ve parolayı belirleyebilir, MaestroPanel Agent'ın ve Web Management Servisinin çalışacağı IP adresini belirleyebilir ve varsayılan olarak web sitelerinin hangi dizine açılacağını tanımlayabilirsiniz.

Belirtilen kullanıcı adı ve parola aynı zamanda kurulacak servislerin erişimleri içinde geçerli olacaktır.

Setup, MySQL'in root kullanıcısının parolasını (Eğer seçilmişse), Microsoft SQL'in sa kullanıcısının parolasını Password alanından belirtilen parola ile aynı tanımlayacaktır.

Lisans IP Adresi MaestroPanel Agent'ın çalışacağı ve MaestroPanel Lisansının tanımlı olduğu IP adresidir.

Bu alan normal IP adresi olacağı gibi aynı zamanda domain ismi de olabilir.

***Dikkat!** Lisansın sorunsuz çalışması için, Lisans kontrol panelinden (https://
secure.maestropanel.com) lisans oluştururken buradaki IP ile aynı olmalıdır.*

Örneğin: localhost veya erişilebilir herhangi bir host ismi (panel.maestropanel.net gibi).

Kurulum sihirbazının A2 ekranında MaestroPanel'in desteklediği tüm teknoloji ve yazılımlar mevcuttur. 


**MaestroPanel Web Management Service** dediğimiz panelin merkezi yönetimini sağlayan bağımsız bir bileşende en başta olmak üzere buradan seçip kurabilmemiz mümkün. Bu bileşeni aşağıdaki A4 ekranında görebilirsiniz.

#### MaestroPanel Web Management Service

MaestroPanel Agent'ları yöneten bir Maestro görevi görür. Agent'lara haber gönderebilir, Agent'lar dan bilgi isteyebilir ve tüm sistemi monitör edebilir.
Kurulumda hem MaestroPanel Agent'ı hemde MaestroPanel Web Management Servisini aynı anda seçebilirsiniz. Web Management Servisini seçmediğiniz taktirde Setup bu adımdan sonra hemen kuruluma geçecektir.

Kuruluma Web Management Servisini seçerek devam ederseniz karşınız bir kaç adım daha çıkacaktır. Bunlar sırası ile aşağıdaki gibidir.

Ekran A5

Bu ekran Web Management Servisinin hangi veritabanı motorunu kullanacağını belirler. Servis şuanda Microsoft SQL Server ve SQLite 3 veritabanı motorlarını desteklemektedir. Bunlardan uygun olanını seçip bir sonraki ekrana geçebilirsiniz.

> **Hangi Veritabanı Motorunu Seçmeliyim?**
>
> MaestroPanel olarak iki tür veritabanı tipini ekleme ihtiyacı duyduk. Bunlardan birincisi sunucu bazında bir çok isteğe cevap verebilecek ve network katmanında da çalışabilen SQL Server'lar. Diğeri de daha taşınabilir olması açısından dosya tabanlı veritabanı motorları.

> Bu motorların kullanım tipleri ve alanları farklılık gösterse de Kontrol Panel projelerinde ihtiyaca göre her ikisi de rahatlıkla kullanılabilir.

> Örneğin dağıtık bir yapı oluşturmak istiyorsanız ve 250 üzerinde bir domain barındırabilecek potansiyeliniz varsa kesinlikle SQL Server tipini yani Microsof SQL Server'ı seçmelisiniz.

> MaestroPanel'i Box şeklinde çalıştırıyor ve 250 altında bir domain barındırmayı planlıyorsanız dosya bazlı veritabanı tiplerini seçmenizi öneririz yani SQLite.

> Şu anda Desteklenen Veritabanları

> * Microsoft SQL Server 2008 R2
> * Microsoft SQL Server 20012
> * SQLite 3

> Desteklenmesi Planlanan Veritabanları

> * MySQL
> * SQLCE
> * MS Access
> * PostgreSQL

SQL Motorlarından SQLite'ı seçip ilerlerseniz herhangi bir parametre gerektirmediğinden Setup hemen kuruluma başlayacaktır. Bu adımdan sonra kurulumun bitmesini bekleyebilirsiniz.

Microsoft SQL Server'ı seçtiğinizde ise Setup sizden bu yazılımın çalışması için gerekli olan parametreleri takip eden adımlarda isteyecektir.
Bu adımlarda sırası ile aşağıdaki gibidir.

Ekran 6

**Use an existing SQL Server**

Eğer hali hazırda kurulu olan ve çalışan bir Microsoft SQL sunucunuz var ise bu seçeneği işaretleyip mevcut SQL sunucunuzun erişim bilgilerini girerek kuruluma devam edebilirsiniz.

SQL sunucusuna erişip gerekli olan veritabanını ve kullanıcıyı oluşturarak
kurulumu gerçekleştirecektir.

Burada dikkat edilmesi gereken husus, var olan SQL sunucusuna erişirken tanımlayacağız kullanıcının veritabanı açma, kullanıcı oluşturma gibi haklara sahip olması gerekliliğidir. 

Biz burada "sa" kullanıcısı bilgilerinin girilmesini öneririz.

Ekran 7

A7 ekranındaki diğer bir kırılım ise Setup'ın yeni bir veritabanı üzerinden mi yoksa var olan bir veritabanı üzerinden mi kurulum'a devam edeceğidir.

**Use existing database** seçeneğini işaretlerseniz Setup yeni bir veritabanı açmak yerine sizin belirlediğiniz bir veritabanını sistemde arayıp gerekli olan tablolarını oluşturacaktır.

**Create new database** seçeneğini işaretlerseniz Setup direkt A8 ekranında belirtecek olduğunuz isminde yeni bir veritabanı oluşturup ardından tabloları ve gerekli verileri girecektir.

>Dikkat! Veritabanı ismi belirlerken sistemde daha önce olmayan ve tamamen ASCII karakterlerden oluşan isimler belirlemelisiniz.

Next butonuna bastığınızda Setup veritabanına bağlanarak diğer adıma geçecektir. O nedenle bu adımda kesinlikle veritabanının çalışır durumda ve yerel sunucu tarafından erişilebilir durumda olmasına dikkat edin.

#### Install SQL Server and Create database

A6 ekranında bu seçeneği işaretlerseniz Setup en başta yerel makineye Microsoft SQL Server 2008 R2 Express Edition yazılımını kurup konfigürasyonunu yapacaktır. Daha sonra A8'de belirlenen bilgilerle beraber kullanıma hazır hale getirecektir.