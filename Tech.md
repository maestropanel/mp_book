## Teknoloji

MaestroPanel Controller ve Agent olmak üzere 2 bölümden oluşmaktadır;

Controller denilen bölüm basitçe panel işlemlerinin yapılmasını sağlayan Web Uygulamasından oluşmaktadır. Agent bölümü ise daha çok sunucu üzerinde çalışan, controller'dan gelen emirleri sunucuda uygulayan bir işletim sistemi servisidir.

![](https://lh4.googleusercontent.com/tWaXl67gdJc7GzBa18p6IJP1nBBpCyEIcA9w6oac7Tn87QEUecYRvR4Grlxbt_P9ekugqLwC7hfED9COPcBFtrER7K74-mjM-JP6OGXlWpytLOfXiK1f19YtgpVPu81lMw)

MaestroPanel **.Net Framework 4.0** ile geliştirilmiştir. Fakat içinde .Net 2.0 ve 3.5 sürümler ile çalışan bileşenlerde mevcuttur.

Controller'ın Front-End tarafında **ASP.NET MVC**, **Jquery**, **Foundation Zurb** ile hazırlanmış Template desteği olan bir arayüz vardır. Güncel arayüz de **Razor ViewEngine** kullanmaktadır.
Yine Controller **MsSQL** ve **SQLite** olmak üzere iki veritabanı üzerinde çalışabilmektedir. Veritabanı ile haberleşmesi için ise **Nhibernate** kullanılmıştır. Bu ORM aracını daha efektif kullanabilmek için ise **FluentHibernate**'den yararlanılmıştır.

Back-End tarafta ise Self-Hosted çalışan bir **WCF** servisi HTTP üzerinden SOAP şeması üzerinden Controller emirlerini dinleyebilmektedir. MaestroPanel'in modüler yapısının altında ise **MEF** dediğimiz framework yatmaktadır. Back-End tarafın **Linux** üzerinde çalışması için ise **Mono** Framework'ü kullanılmıştır.

Arada Kullandığımız;

Log hesaplamalarında ve büyük Text dosya analizlerinde Perl, C++, LogParser araçlarından yararlandık.

Bazı Self-Hosted çalışan Micro Servislerde ise Go Programlama dilindan faydalandık.