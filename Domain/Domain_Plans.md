# Domain Planları 

Domain planları, açacağınız domain'lerin hangi sunucudan hangi modülleri kullanacağına, kullanacağı modüllerin limitlenmelerine  karar verdiğiniz şablonlardır. 

Domain planlarında kullandırmak istediğiniz özelliklerin hagi sunucuda çalışacağına karar verebilir, MaestroPanel'in çoklu sunucu desteğin avantajlarını etkili bir biçimde kullanabilirsiniz.

# Yeni Domain Planı

MaestroPanel'in çoklu sunucu özelliğini kullanabilmek için domain planlarından yararlanırız. Domain Planlarında hangi bileşenin hangi sunucu üzerinde çalışacağını belirleyebilir, her servisin kendine özgü olan limitlerini belirleyebilirsiniz.

![](https://lh5.googleusercontent.com/g8LyHQOWMtnq1WDW8YiSXOo-rlu1St1pWYmn1GnAP6AY-A44cqgeAe45YNiVptubOI_Q7GfXdwLmoHspfWcSEfFdNnbPwLgnJn5soQEmSvhi5uwDNjG6BH6zfFAYLPeVOA)

Yeni Domain Planı Oluşturmak İçin;

Sol menüden **Domainler > Domain Planları > Yeni Domain Planı** menüsünü takip ederek ilgili forma ulaşabilirsiniz.

Bu formdaki alanlar aşağıdaki gibidir;

**Plan Adı**

Planı tanımlamak için kullanılan alandır. Domain açarken bu isim görüntülenerek ayırt edilir. Çok uzun olmayan kısa ve öz bir açıklama girmeniz tavsiye edilir. Örneğin: Gold Plan

**Plan Açıklaması**

Plan'ı daha ayrıntılı tanımlayan alandır. Uzun ve açılayıcı bilgiler girilebilir. Örneğin: Gold Plan, 100MB Web Alanı, 10 Email, 1 MySQL, 1 MsSQL

**Takma İsim (Alias - API için)**

API erişimlerinde plan'ı ayırt etmek için kullanılan alandır. Herhangi bir sistemden domain'i hangi plan'a göre oluşturmak istediğinizi programatik olarak bu alanadan ayırabilirsiniz. WHMCS modülünde paketleri eşlemek için bu alan kullanılır.

Kısa tek cümleden oluşan hepsi büyük veya hepsi küçük Türkçe karakter içermeyen bir tanımlama girmeniz önerilir. Örneğin: GOLDPAKET

**Sonlanma Tarihi**

Bu planla açılan domain'in sonlanma tarihini belirler Yıl, Ay, Gün seçeneklerinden birini seçebilirsiniz. 2 değerini girip YIL seçerseniz Domain'i açtığınız tarihten itibaren 2 yıl ekler.

**Modüller**

Modüller alanı Domain Planının hangi özellikleri taşıyacağını belirlediğiniz alandır. MaestroPanel'in dağıtık yapısını burada örnekleyebilirsiniz. Sağ taraftaki sunucular menüsünden hangi sunucuda hangi özelliğin çalışacağnı belirleyebilirsiniz.

Örneğin: DNS özelliğini "Server 2" üzerinde, Web sitesini ve Web sitesinin PHP çalıştırmasını "Server 1" üzerinde belirleyebilirsiniz.

# Domainlere Uygula Özelliği

MaestroPanel, herhangi bir Domain Planını mevcut Domainler üzerine uygulayabileceğiniz bir özelliğe sahiptir. 

Bu özelliğe;

**Domainler > Domain Planları > [Plan Adı] > Domainlere Uygula İkonu**

menüsünden ulaşabilirsiniz.

![](https://lh5.googleusercontent.com/Prb0PQOwCdMgulwYkqlXEWQaNHUXysUwFvrrOFE23dTq18E2Vjf0RHYYZy_BOveQToWUIZ-EhhshnJ48WG42hmjaVV9Lxstzt2_-EV3hT_rLKcFVrpDSXbp2ztgk_WFOKQ)

Domainlere Uygula İkonuna tıkladıktan sonra mevcut domainlerin listesi karşınıza gelecektir. Açılan listede Domain Planını uygulamak istediğiniz domainleri seçip "Uygula" dediğinizde Domain Planına ait özellikler seçil Domainlere eklenecektir.

![](https://lh5.googleusercontent.com/6o-Jaff5JQ26KOaXbuQPtYHpUoywocjDALvZMQTtnV8CUHZdHBsK9qNYMAwRu6LOvhgdDpX_0d2Zp0B3oBQsplH2-jWAiAb-7j90pQgcak8pAZTKC0bk_Z8hXui63k5HMg)

