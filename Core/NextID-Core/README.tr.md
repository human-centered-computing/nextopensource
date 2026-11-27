# NextID-Core

[English](README.md) · [Türkçe](README.tr.md) · [Core kütüphanesi](../README.tr.md)

NextID için ortak açık kaynak kimlik ve erişim yönetimi temeli. Kaynak kişisel fork'tan değil, doğrudan [keycloak/keycloak](https://github.com/keycloak/keycloak) adresinden alınır. Kişisel [muratdelen/NextID-Core](https://github.com/muratdelen/NextID-Core) yalnızca mimari referanstır. Sorumlu insanın talebiyle eski kişisel fork sürümü veya senkronizasyon iş akışı yerine üst kaynağın son kararlı sürümü kullanılır.

- İnceleme anındaki son kararlı üst kaynak sürümü: [26.8.2](https://github.com/keycloak/keycloak/releases/tag/26.8.2) (2026-11-05).
- Üst kaynak commit'i: [`e514445f9dcdabc5bdcf67cab56c1e49655de067`](https://github.com/keycloak/keycloak/commit/e514445f9dcdabc5bdcf67cab56c1e49655de067)
- Üst kaynak ağaç kimliği: `6f439a9bda71c39bf725150cea5d50f149e423f6`
- Lisans: Apache-2.0; [özgün lisansı](https://github.com/keycloak/keycloak/blob/e514445f9dcdabc5bdcf67cab56c1e49655de067/LICENSE.txt), telif ve bildirimleri koru.
- Kaynak klasörü: `source/`, asıl üst kaynak deposunun kesin commit'ine bağlı Git submodule.

NextOpenSource yerel checkout'undan sonra tüm kaynak kodunu almak için:

```bash
git submodule update --init --recursive Core/NextID-Core/source
git -C Core/NextID-Core/source rev-parse HEAD
```

Bu yapı özgün Git geçmişini ve depo düzenini korur; bağımsız fork'un tamamını NextOpenSource'un kendi geçmişine kopyalamaz. GitHub gitlink ve sabit sürümü saklar; submodule başlatıldığında kod doğrudan Keycloak'tan çekilir. HCC'ye özgü kaynak değişikliği, ürün yerelleştirmesi, kimlik bilgisi veya çalışan senkronizasyon iş akışı eklenmemiştir.

Gelecekteki güncellemelerde üst kaynağı çek, kesin sürümü seçip incele, güvenlik/lisans/derleme ve regresyon kanıtlarını değerlendir; gitlink'i incelenmiş PR ile güncelle. Otomatik senkronizasyon, derleme, dağıtım veya üretime uygunluk iddia edilmez. Bkz. [üst kaynak kaydı](UPSTREAM.md).
