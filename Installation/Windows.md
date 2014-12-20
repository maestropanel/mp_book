## Kurulum (Windows)

Sunucunuza MaestroPanel.exe yi indirdikten sonra herhangi bir ayar yapmadan direkt Administrator kullanıcı hakları ile çalıştırıp kuruluma başlayabilirsiniz.

**MaestroPanel.exe** dosyasını çalıştırdığınızda karşınıza ilk olarak MaestroPanel'in hangi dizine kurulacağını belirleyebileceğiniz A1 ekranı gelecektir.

Varsayılan olarak olarak *C:\Program Files\MaestroPanel* klasörü hedef gösterilmiştir. Setup bu dizini gerektiği şekilde oluşturup güvenliğini sağlayarak kuruluma başlayacaktır. 
Dosya yolunun arasında boşluk olması MaestroPanel için sorun değildir.

**Ekran A1**

![](https://lh5.googleusercontent.com/U84mrBBvxADgi2yzI5jLZSm8k2iEJ57UxwWf302yd7HC25QYiXblLfCb2taddfx-T7R63eJNFTuRp8xGnmF4rCxmfrsEzJQ69faLFa4IZjspmmjBRWyaDJ0RtpH5sHaEUQ)

Kurulum dizinini belirledikten sonra **Next** butonuna basıp bileşenleri seçebileceğimiz bir sonraki ekrana geçiş yapabiliriz. 

**Ekran A2**

![](https://lh5.googleusercontent.com/6Z6uQbwZ5LAXSDZ3k8pSaYkRbIeG0-LKDtKsSUNcD-454QlyFP9FvLB1f41gypsHlfNjm0xQurHwK8ASzYQrlZ0iI7gC6nLfzblWI-TONp07ORj2O9m_6x8CpgFlS59vHA)

Bu ekranın en üstünde önceden tanımlanmış bileşen kombinasyonlarını içeren şablonlar bulunmaktadır. Kurulmasını istediğiniz bileşenleri tek tek seçebileceğiniz gibi şablonları kullanıp ideal seçimlerde yapabilirsiniz.

> **Full Hosting Environment (Agent + Web Management):**

> Hem MaestroPanel Agent hemde Web Management Servisi ile alakalı tüm bileşenleri kurar.

> **Standart Hosting Environment (Only Agent): **

> Sadece MaestroPanel Agent'ı ve paylaşımlı hosting için gerekli olan standart bileşenleri seçer.

> **Light Hosting Environment (Only Agent):**

> Sadece MaestroPanel Agent'ı ve çok temel olan ihtiyacı karşılayacak paylaşımlı hosting bileşenlerini kurar.

İstenilen bileşenler seçildikten sonra **Next** butonuna basıp diğer ekrana geçebilirsiniz

**Ekran A3**

![](https://lh4.googleusercontent.com/3TZiefzYXWPBuxQSCaqml6mrou2GxepKnh0XomrczXUO62TVSsirPSF8vPemQSK6pqocZqOfWVpcXBFfuWTCZZ8DYuHuBnWTFt8-T6krssrBKD13EHqdZ6185flJJetw3w)

Bu ekranda panel'e erişebilmeniz için gerekli olan kullanıcı adı ve parolayı belirleyebilir, MaestroPanel Agent'ın ve Web Management Servisinin çalışacağı IP adresini belirleyebilir ve varsayılan olarak web sitelerinin hangi dizine açılacağını tanımlayabilirsiniz.

Belirtilen kullanıcı adı ve parola aynı zamanda kurulacak servislerin erişimleri içinde geçerli olacaktır.

Setup, MySQL'in root kullanıcısının parolasını (Eğer seçilmişse), Microsoft SQL'in sa kullanıcısının parolasını Password alanından belirtilen parola ile aynı tanımlayacaktır.

Lisans IP Adresi MaestroPanel Agent'ın çalışacağı ve MaestroPanel Lisansının tanımlı olduğu IP adresidir.

Bu alan normal IP adresi olacağı gibi aynı zamanda domain ismi de olabilir.

Kurulum sihirbazının A2 ekranında MaestroPanel'in desteklediği tüm teknoloji ve yazılımlar mevcuttur. 

**MaestroPanel Web Management Service** dediğimiz panelin merkezi yönetimini sağlayan bağımsız bir bileşende en başta olmak üzere buradan seçip kurabilmemiz mümkün. Bu bileşeni aşağıdaki A4 ekranında görebilirsiniz.

**Ekran A4**

![](https://lh3.googleusercontent.com/6WUFJ1mBinszxK4FIV0EWnBQvpr9VY_oN-a7hQHGx8TclwoWtYPV7jFKhdBqP0t-nnA6qfs4Z1IKb7IfqcU3XNiSdEWvqoJX9U8a1TT3mZjqsYaCoakn1U7nG9LfEwN-QQ)

### MaestroPanel Web Management Service

MaestroPanel Agent'ları yöneten bir Maestro görevi görür. Agent'lara haber gönderebilir, Agent'lar dan bilgi isteyebilir ve tüm sistemi monitör edebilir.

Kurulumda hem MaestroPanel Agent'ı hemde MaestroPanel Web Management Servisini aynı anda seçebilirsiniz. Web Management Servisini seçmediğiniz taktirde Setup bu adımdan sonra hemen kuruluma geçecektir.

Kuruluma Web Management Servisini seçerek devam ederseniz karşınız bir kaç adım daha çıkacaktır. Bunlar sırası ile aşağıdaki gibidir.

**Ekran A5**

![](https://lh6.googleusercontent.com/HMqxq5sh4zZArcLWuG3z0qBac-8Pj-d8i_cqKbPad4R0Nnz6NbzqwWLkuRPflw6Fe7tisTpJTjFqNYpz-Pb2lm7uMs7ryK1F9HLD8U8nF3qVKySAGeK4bgVVx1brT-YsVA)

Bu ekran Web Management Servisinin hangi veritabanı motorunu kullanacağını belirler. 

Servis şuanda **Microsoft SQL Server** ve **SQLite 3** veritabanı motorlarını desteklemektedir. Bunlardan uygun olanını seçip bir sonraki ekrana geçebilirsiniz.

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

**Ekran 6**

![](https://lh6.googleusercontent.com/binDIAR8j2swc3pHsFBI_95Uka51jSRXdVP_QuBIyp1akAFyG9SLgCr931GeuOWerBRZJtBgdn_I7HYFQERvw9TAwhVZdYvSga9oo8MXP9Drc5vpnhyxBedZ8fpP_OE5Tw)

**Use an existing SQL Server**

Eğer hali hazırda kurulu olan ve çalışan bir Microsoft SQL sunucunuz var ise bu seçeneği işaretleyip mevcut SQL sunucunuzun erişim bilgilerini girerek kuruluma devam edebilirsiniz.

SQL sunucusuna erişip gerekli olan veritabanını ve kullanıcıyı oluşturarak
kurulumu gerçekleştirecektir.

Burada dikkat edilmesi gereken husus, var olan SQL sunucusuna erişirken tanımlayacağız kullanıcının veritabanı açma, kullanıcı oluşturma gibi haklara sahip olması gerekliliğidir. 

Biz burada "sa" kullanıcısı bilgilerinin girilmesini öneririz.

**Ekran A7**

![](https://lh3.googleusercontent.com/JrzItszfEPu8P-Wy7-5ZZHNVesz40txK3LxSPLEhzd6zEj898KsMHoBXpcr1BwD0dK3XAygcZkojhT6YkUCXXi2a8jZ6ExUUo_7opaqGQmQoj_9iw15p6xMfR-E0jctJ_Q)

A7 ekranındaki diğer bir kırılım ise Setup'ın yeni bir veritabanı üzerinden mi yoksa var olan bir veritabanı üzerinden mi kurulum'a devam edeceğidir.

**Use existing database** seçeneğini işaretlerseniz Setup yeni bir veritabanı açmak yerine sizin belirlediğiniz bir veritabanını sistemde arayıp gerekli olan tablolarını oluşturacaktır.

**Create new database** seçeneğini işaretlerseniz Setup direkt A8 ekranında belirtecek olduğunuz isminde yeni bir veritabanı oluşturup ardından tabloları ve gerekli verileri girecektir.

>Dikkat! Veritabanı ismi belirlerken sistemde daha önce olmayan ve tamamen ASCII karakterlerden oluşan isimler belirlemelisiniz.

Next butonuna bastığınızda Setup veritabanına bağlanarak diğer adıma geçecektir. O nedenle bu adımda kesinlikle veritabanının çalışır durumda ve yerel sunucu tarafından erişilebilir durumda olmasına dikkat edin.

#### Install SQL Server and Create database

A6 ekranında bu seçeneği işaretlerseniz Setup en başta yerel makineye Microsoft SQL Server 2008 R2 Express Edition yazılımını kurup konfigürasyonunu yapacaktır. Daha sonra A8'de belirlenen bilgilerle beraber kullanıma hazır hale getirecektir.

**Ekran 8**

![](https://lh3.googleusercontent.com/WnpeFyGl2aamtmTcCODoHRSqpJ7kb7QdRD8R7IqKsTP7TpcSXEJSH6U97rGVohRtikxm-rawJJYEc_KADsPFaZm6hGrbhfMhvhCDM6ec3KFL6DwYe85xi5Km48P0uxP3bQ)

Bu ekranda MaestroPanel'in veritabanı ve bu veritabanına erişirken kullanılacak kullanıcı tanımlamalarını yapabilirsiniz. Veritabanı adı ve kullanıcı adı belirlerken Türkçe karakter ve özel karakterleri kullanmamaya dikkat edin. Parola için bu geçerli değildir.

Bu adımı tamamladıktan sonra artık seçili olan bileşenler aşağıdaki A9 ekranında görüldüğü gibi sunucu üzerine otomatik olarak kurulmaya hazır hale gelecektir.

**Ekran A9**

![](https://lh5.googleusercontent.com/BTikU_G9_nZP_mXYcZdmGWVsXc9EqKSmdo7XTGzKVZ6SXrcmuDxEQl4GtxeJDJFw3yYWyzS4G5g0G_WQnajr_6R9q6IT5_4SYv9cte0FLdnBlfSukMzjaWVx33qvQkIUww)

Install butonuna basıldıktan sonra Setup "Preparing to Install" aşamasına geçer. 

Öncelikle modüllerin gereksinim duyduğu Framework ve Runtime'ları eğer sunucuya daha önce kurulmamışsa bu adımda kurulur ve çeşitli sunucu değişkenlerini aktif edilir.  Örneğin MaestroPanelPath

**Ekran 10**

![](https://lh6.googleusercontent.com/c8vd2euyezz76r-Fx-AEQ0o9C6_eZa52qv2MTfIth1aRP2bwalJDrTF2J07YXNEglxc4w8lgWRdfhV8iyCYjKcpaHadSaMcQmkRff5ZyavjCaKQFU88OnV7gieuIdY0k5g)

Peraparing to Install sırasında Setup sunucu üzerinde aşağıdaki bileşenlerin olup olmadığını kontrol eder.

* .Net Framework 4.5 (Server 2012 kurulumunda)
* .Net Framework 4.0
* .Net Framework 3.5
* IIS 7.5 (IIS 7.5 bağımlı modül seçilmişse)
* Microsoft Visual C++ Redistributable
* Microsoft DNS (DNS Bağımlı modül seçilmişse)
* %MaestroPanelPath% isminde sunucu değişkeni (System Environment)
* Microsoft SQL Server Native Client

Eğer yukarıdaki bileşenlerden herhangi biri yok ise Setup sunucuya otomatik olarak kurar ve **A11** ekranında olduğu gibi gerekirse sistemin yeniden başlatılmasını ister.

**Ekran A11**

![](https://lh4.googleusercontent.com/Tg-kHcuTyvD4tYHkPTPCiuuwJNaGxz8AdtY9YcdQFPJIBQEc-a_8KKaf8AoUF3kRE5mZQUTCpo4zDjawQV7xy17OhN85h8SjBwtqJFXl-AEDKpIouSRbWY6ihqtQsAuUaQ)

Burada Yes, restart the computer now seçeneğini işaretleyip Finish butonuna bastıktan sonra sunucu derhal yeniden başlatılır. Tekrar sunucuya giriş yaptığınızda Setup kaldığınız yerden kuruluma devam eder.

No, I will restart the computer later seçeneğini işaretlemeniz durumunda, sunucu hemen yeniden başlatılmaz fakat Setup'ı sunucu yeniden başlatılana kadar da çalıştırmanıza izin verilmez.

Bu adımdan sonra sunucuya ilk girişinizde Setup otomatik olarak kaldığı yerden başlar ve tüm bileşenleri sizin için kurup optimize ederek kurulumu tamamlar.

