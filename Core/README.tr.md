# Core — ortak açık kaynak temeli

[English](README.md) · [Türkçe](README.tr.md) · [Deutsch](README.de.md) · [العربية](README.ar.md) · [NextOpenSource](../README.tr.md)

Bu klasör, HCC için üçüncü taraf açık kaynak projelerinden alınan yeniden kullanılabilir bileşenlerin ortak kataloğu ve kaynak kod alanıdır. Yetkilendirilmiş her bileşen `Core/<BileşenKimliği>/` altında sabit bir klasöre sahip olur.

```text
Core/
  README.md
  README.tr.md
  <BileşenKimliği>/               # her üst kaynak bileşeni için ayrı klasör
    README.md                    # köken, amaç, sabit sürüm, kullanım
    README.tr.md                 # eşdeğer Türkçe dokümantasyon
    UPSTREAM.md                  # köken ve inceleme kaydı
    source/                      # yetkili üst kaynak kopyası veya Git submodule
    patches/                     # gerekirse açıkça kayıtlı HCC değişiklikleri
```

## Aktarım ve bakım kuralları

- Aktarımdan önce üst kaynak depo adresini, kesin commit/etiketi, lisans ve zorunlu bildirimleri, bakım durumunu, bağımlılıkları, güvenlik incelemesini, HCC'deki kullanım amacını ve insan onayını kaydet. [Üst kaynak kayıt şablonunu](../templates/UPSTREAM.md) kullan.
- Kaynak kodla birlikte özgün lisans/bildirim dosyalarını, atıfları ve üst kaynak kökenini koru. Doğrulanmış sabit üst kaynak sürümünü tercih et; mevcut Core deposunu çoğaltmak yerine uygun olduğunda ayrı Core deposuna veya submodule referansına başvur. Özgün kaynak ve HCC değişiklikleri izlenebilir olmalıdır.
- Ürüne özgü yerelleştirilmiş verileri, gizli bilgileri, görsel sunum varlıklarını veya tescilli kaynak kodu üst kaynak temeline karıştırma. Ürün uyarlamalarını bağımsız ürün deposunda tut; kaçınılmaz Core yamalarını ayrı belgeleyip incelet.
- Güncellemeleri, lisans uyumunu ve güvenliği geçerli inceleme süreciyle doğrula; NextSecurity test kanıtlarına bağlantı ver. Lisansı veya kökeni belirsiz kodu aktarma; deponun gizli olmasını lisans varlığı kabul etme.
- Projeye özgü değerlendirme ve entegrasyon planları NextOpenSource ve NextRoadmap'in ilgili proje klasörlerinde tutulur. Her projeye kopyalamak yerine bu ortak bileşen kütüphanesini kullan.

## Kayıtlı bileşenler

| Bileşen | Üst kaynak | Sabit sürüm | Lisans | Durum |
|---|---|---|---|---|
| [NextID-Core](NextID-Core/README.tr.md) | [Keycloak](https://github.com/keycloak/keycloak) | [`26.8.2`](https://github.com/keycloak/keycloak/commit/e514445f9dcdabc5bdcf67cab56c1e49655de067) | Apache-2.0 | Değiştirilmemiş tam kaynak kod kopyası; güvenlik/derleme doğrulaması bekliyor |

Yeni bileşenleri ilgili inceleme ve yetkilendirmeden sonra ekle.
