# MaestroPanel Arayüz

MaestroPanel'in arayüzü ekran genilşiğine duyarlı olarak (Responsive) geliştirilmiştir. Hem cep telefonundan, hem tablet üzerinden hem de masaüstü ekranlara en efektif görüntüyü sağlamaktadır.

Aşağıda MaestroPanel'in Özet (Dashboard) sayfasını ve sabit kontrollerin işlevlerini bulabilirsiniz.

![](https://lh4.googleusercontent.com/JhDFaaPk3dJlE4VJF-BBlIFY1P0XtHAxFfO8rESRMyVqL02_n06I72kl-8V6XRO-9qBdFTGzKWbPjfpWGJRDN42CntfCtsSqV_90uPLoyES7KHTqoZAhkXB2bPJ-CiwgEQ)

MaestroPanel birden fazla tema desteklemektedir. Kullanıcı istese kendi temasını oluşturabilir veya mevcut tema üzerinde HTML yada JavaScript seviyesinde değişiklik yapabilir.

> Not: MaestroPanel'in arayüz kodları açık ve değiştirilmeye müsaittir. Arayüz kodlarına sunucu üzerinde aşağıdaki dizin altından erişebilirsiniz.

**Genel Sayfalar**

```
%MaestroPanelPath%\Web\www\Views\Themes\
```

**Sunucu, Domain ve Reseller Yönetim Sayfaları**
```
%MaestroPanelPath%\Web\www\Views\Areas\themes\
```

**Modül Sayfaları**

```
%MaestroPanelPath%\Web\www\\Views\Themes\{THEME_NAME}\Shared\Extensions
```

> Not: MaestroPanel teması ASP.NET MVC ile birlikte gelen Razor ViewEngine ile geliştirilebilmektedir.

## İlk Giriş

MaestroPanel'e ilk girişinizde karışınıza kullanıcı adı, parola sorusu ile kullanacağınız temanın ne olacağını belirtebileceğiniz bir seçenek kutusu gelir.

Kullanıcı adı ve parola alanına kurulumda belirttiğiniz bilgiler girerek ilk girişi yapabilirsiniz.

![](https://lh4.googleusercontent.com/faavPYkZEehacqsLPCJWSIrUDiU6or3BBcg1rYZ0J0rrU7GLTk0M7q31d7RqZVNtElz6zvlCmEkTgTQ6nnj4R24gbYnbXERAAdaK63hwUs7bPwEsaxqT2jwzywVbanB1sw)

## Sihirbaz Adımları

MaestroPanel'e giriş yaptıktan sonra temel ayarları yapılandırabileceğiniz 5 adımlık bir sihirbaz sizi yönlendirecektir.

#### Adım 1

![](https://lh3.googleusercontent.com/Z8YWA88rrNjZYKY_JYInlG871E04K-Gi821IszFiD8o60AUEi3zkDmQpFZ-xDWigGd7H2tefIB35f3sW-q4LdGFuvLCnnB4NIpDfXJ6c-GzWPBt4m2rnr17dEEl93Aa4cg)

Adım 1'de Profil bilgilerinizi tanımlayabileceğiniz ekrandır. Bu adım yöneticinin kim olduğunu, panel yöneticisinin hangi firma olduğunun tanımlayabileceğiniz ekrandır.

#### Adım 2

![](https://lh4.googleusercontent.com/KnUKtSPIxFKR4zbppgmLvHcIs_LeWBUBzLxo1rAiue2pPC5ru9oDAZ5dUWBYUcmopQ7YH_76Rp1PR_-9ctTe1XSvBOfmGZSEuHhwylWYMxyeKOYY_4VhDsqtmx2gpM7vsw)

İkinci adım yönetici e-posta adresinin, destek e-posta adresinin ve parola güvelik seviyesini tanımlayabileceğiniz ekrandır. (Bu bilgiler Menü > Ayarlar bölümünden de daha sonra düzenlenebilir)

**Yönetici Email**

Panel ile ilgili uyarıların gönderildiği e-posta adresidir.

**Destek Email**

Kullanıcıların herhangi bir sorunda erişebilecekleri e-posta adresidir. Bir hatada kullanıcı bu e-posta adresine yönlendirilir.

>#### Parola Güvenlik Seviyesi

>MaestroPanel üzerinde tanımlacak tüm parolaların zorluk derecesini tanımlar. Her zaman "Yüksek Düzenyli Parola Politikası" seçeneğini seçmeniz önerilir.

>**Düşük Seviye Parola Politikası (Low Level Password Policy)**

>* Minimum 6 karakter uzunluk
* Küçük veya Büyük Harf
* Sayı

>**Orta Seviye Parola Politikası (Medium Level Password Policy)**

>* Minimum 8 karakter uzunluk
* Küçük Harf
* Büyük Harf
* Sayı veya Özel Karakter

>**Yüksek Seviye Parola Politikası (High Level Password Policy)**

>* Minimum 8 karakter uzunluk
* Küçük Harf
* Büyük Harf
* Sayı
* Özel Karakter

## Adım 3

![](https://lh4.googleusercontent.com/znhg9DadYDh6K6ksnthbo0g1q2J8poODeHlT5XgCuSFZScgypkFn4-cEM8Va3TiL1a5aMC--dvvZxgxxiTBeEdnWLuzI_zIw9jqWb-OMHUKM8IaSbmHh-OWw1yLKsHOxNA)

MaestroPanel'de oluşturulacak domain'lerin name server'larının neler olacağını belirtebileceğiniz ekrandır.

Bu alanda tanımlayacağınız bilgiler DNS Template'i üzerinde etki gösterecektir. Daha sonra *Sunucular > Dns Şanlonu* menüsü altından değiştirebilirsiniz.

Bu adımı herhangi bir işlem yapmadan geçtiğinizde Domain'e tanımlı Name Server'lar ns1.domain.com, ns2.domain.com şeklinde oluşturulur.

## Adım 4

![](https://lh5.googleusercontent.com/w9VwGyDw89sAMQb-9zW5XW1tL_uWHlTaOHyN6eVEDz16_EftORCyTG6BH934O7J6ttJCwQ1cKm6U3SBqyh3rbCHFSuhcbg9LuORQI0cfV1-wE2Ytyn8CuGRB1Cctz939DQ)

Bu adım Panel’e lisans eklemenizi ve MaestroPanel Agent'ı Panel’inize bağlamanızı sağlar. 

## Adım 5

![](https://lh5.googleusercontent.com/xvgLlPy4-4m26uEfq0sXQxIhYDmyOhbaR8UhAAji6fAPYu20Go4bjOO-v2EWBfP_t-0tmCLr7WnkMyqx5L5NVRby6i7DtZ5cxYVjY2Z8IWaNFv_0pXO3kDYIcrENWdgejQ)

**Agent Ekleme**

Eğer kurulumu Agent dahil yaptıysanız Maestropanel sunucu üzerinde çalışan Agent’ı algılayacaktır.

## Son

![](https://lh3.googleusercontent.com/k6MiRl9dQDaDfMOxUSci5iDSjtxeStg-h4B0IKWKDanJV30egDYVaksoHpVXdcvAyVAYOQDgGwp0wpUBQezhyqeelfmZihBWbfJRbvlizhTnAHic7QH9gvGkgq00kVG3GQ)

