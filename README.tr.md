# NextOpenSource

[English](README.md) · [Türkçe](README.tr.md)

## NextOpenSource nedir?

NextLife'ın tüm HCC projelerine hizmet veren bağımsız açık kaynak ve üst kaynak uyarlama çalışma alanıdır. Yeniden kullanılabilir yazılımları, Core depolarını ve özgün geliştirmeyi karşılaştırır; köken, lisans uyumu, bakım, güvenlik ve uyarlama sınırlarını belgeler.

**Durum:** Özel kuruluş dokümantasyonu çalışma alanı; çalışan servis, konuşlandırılmış ajan, yetki, doğrulanmış proje sonucu veya otomatik kural uygulaması söz konusu değildir.

## Rol ve çalışma standartları

[NextDeveloper](https://github.com/human-centered-computing/nextdeveloper) içindeki **Açık Kaynak Uzmanı** rolü burada yetkilendirilmiş insan, yapay zekâ veya hibrit olarak çalışır. İnsan sorumluluğu, bağımsız inceleme ve insan onayı gereklidir.

- Üst kaynak adresi, sabit commit/etiket, kesin lisans ve bildirimler, bakım durumu ve bağımlılık kanıtını kaydetme.
- Mevcut Core, üst kaynak alternatifleri, eklenti/adaptörler ve özgün geliştirmeyi karşılaştırma; maliyet ve insan faydasını değerlendirme.
- Üst kaynak geçmişi, atıf ve lisansları koruma; Core değişikliklerini yerelleştirilmiş veri, sunum ve özgün ürün değerinden ayırma.
- Yama envanteri, güncelleme stratejisi, sözleşmeler, lisans ve güvenlik kısıtları; bağımsız doğrulamayı NextSecurity'ye yönlendirme.

NextRoadmap onaylı proje analizini, NextOpenSource ayrıntılı üst kaynak değerlendirmeleri ve köken kayıtlarını yönetir. [Core kütüphanesi](Core/README.tr.md), yetkilendirilmiş üst kaynak kodu aktarımlarının ortak alanıdır; her bileşen ayrı klasörde tutulur. Bağımsız Core ve ürün depoları kendi uyarlanmış kaynak kodunun sahibi olarak kalır; bunlar kaydedilir ve bağlantılanır, yinelenen kopyalar oluşturulmaz. Fork, yayın, lisans hakkı verme veya entegrasyon otomatik yetkilendirilmez.

## Proje çalışma alanları ve iş akışı

- Her projenin/modülün sabit kimliği ile kökte tek klasör kullanılır. Yetkilendirilmiş çalışma başladığında klasör oluşturulup burada listelenir; sonraki güncellemelerde aynı klasör kullanılır. Yinelenen veya boş proje klasörleri oluşturulmaz.
- Önce onaylı [NextRoadmap](https://github.com/human-centered-computing/nextroadmap) proje analizi ve ilgili HCC politikaları okunur. [Çalışma kayıt şablonu](templates/WORKSPACE.md) kullanılır.
- Kapsam, rol, sorumlu insan, kesin kaynak sürümü, kanıt, karar, kısıtlar, ölçülebilir kabul ve insan faydası, bağımsız inceleme ve gerekli insan onayı kaydedilir. Kapsamı belirli değişiklikler incelenebilir PR'larla sunulur.
- Gizli bilgiler, kişisel veriler ve hassas kanıtlar olağan Git geçmişinde tutulmaz; yetki dahilinde erişim kontrollü kanıta bağlantı verilir. Kendi çalışmasını onaylama, kapsamı sessizce genişletme ve kanıtsız sonuç iddiası yasaktır.

## Core kütüphanesi

[Core](Core/README.tr.md), yeniden kullanılabilir üçüncü taraf açık kaynak kodlarının ve köken kayıtlarının yetkili aktarımından sonra tutulacağı alandır. Üst kaynak temeli, HCC uyarlamaları, yerelleştirilmiş veri ve ürünün görsel sunumundan ayrı tutulur. Henüz bileşen aktarılmamıştır.

## Projeler

Henüz projeye özel çalışmaya başlanmamıştır.

## Ortak politika

[Mühendislik standartları](https://github.com/human-centered-computing/.github/blob/main/ENGINEERING-STANDARDS.md) · [Yapay zekâ yönetişimi](https://github.com/human-centered-computing/.github/blob/main/AI-GOVERNANCE.md) · [Güvenlik](https://github.com/human-centered-computing/.github/blob/main/SECURITY.md).

İngilizce esas sürümdür. Kök README dosyaları iki dilli standarda uyar. Depo özeldir; gelecekte yayın ve lisanslama uygun inceleme gerektirir. Yayın veya lisans hakkı verildiği anlamına gelmez.
