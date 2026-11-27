# NextID-Core

[English](README.md) · [Türkçe](README.tr.md) · [Core kütüphanesi](../README.tr.md)

NextID için ortak açık kaynak kimlik ve erişim yönetimi temeli. Kaynak kişisel fork'tan değil, doğrudan [keycloak/keycloak](https://github.com/keycloak/keycloak) adresinden alınır. Kişisel [muratdelen/NextID-Core](https://github.com/muratdelen/NextID-Core) mimari referanstır: `8ec0daff818713f106ebbd816581fbe6358f2557` sürümü, `5274246ade2f0a4731ee5004cf29eec4ee58b4aa` üst kaynak commit'ine yalnızca senkronizasyon iş akışı ekler. Aynı özgün Keycloak kaynak temelini sabitliyoruz; kişisel iş akışını aktarmıyoruz.

- Üst kaynak commit'i: [`5274246ade2f0a4731ee5004cf29eec4ee58b4aa`](https://github.com/keycloak/keycloak/commit/5274246ade2f0a4731ee5004cf29eec4ee58b4aa)
- Üst kaynak ağaç kimliği: `5fc6d20afdd8a8f94210ad6a6715246b9dc3c010`
- Lisans: Apache-2.0; [özgün lisansı](https://github.com/keycloak/keycloak/blob/5274246ade2f0a4731ee5004cf29eec4ee58b4aa/LICENSE.txt), telif ve bildirimleri koru.
- Kaynak klasörü: `source/`, asıl üst kaynak deposunun kesin commit'ine bağlı Git submodule.

NextOpenSource yerel checkout'undan sonra tüm kaynak kodunu almak için:

```bash
git submodule update --init --recursive Core/NextID-Core/source
git -C Core/NextID-Core/source rev-parse HEAD
```

Bu yapı özgün Git geçmişini ve depo düzenini korur; bağımsız fork'un tamamını NextOpenSource'un kendi geçmişine kopyalamaz. GitHub gitlink ve sabit sürümü saklar; submodule başlatıldığında kod doğrudan Keycloak'tan çekilir. HCC'ye özgü kaynak değişikliği, ürün yerelleştirmesi, kimlik bilgisi veya çalışan senkronizasyon iş akışı eklenmemiştir.

Gelecekteki güncellemelerde üst kaynağı çek, kesin sürümü seçip incele, güvenlik/lisans/derleme ve regresyon kanıtlarını değerlendir; gitlink'i incelenmiş PR ile güncelle. Otomatik senkronizasyon, derleme, dağıtım veya üretime uygunluk iddia edilmez. Bkz. [üst kaynak kaydı](UPSTREAM.md).
