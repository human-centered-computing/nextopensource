# NextID-Core

[English](README.md) · [Türkçe](README.tr.md) · [Deutsch](README.de.md) · [العربية](README.ar.md)

NextID için ortak açık kaynak kimlik ve erişim yönetimi temeli. Özgün kaynak [keycloak/keycloak](https://github.com/keycloak/keycloak) adresinden gelir; kişisel fork yalnızca yapısal referanstır. Özgün üst kaynak dosyalarında kasıtlı değişiklik yapılmamıştır.

- Üst kaynak sürümü: [26.8.2](https://github.com/keycloak/keycloak/releases/tag/26.8.2) (2026-11-05).
- Sabit commit: [`e514445f9dcdabc5bdcf67cab56c1e49655de067`](https://github.com/keycloak/keycloak/commit/e514445f9dcdabc5bdcf67cab56c1e49655de067)
- Kaynak ağaç kimliği: `6f439a9bda71c39bf725150cea5d50f149e423f6`
- Lisans: Apache-2.0; özgün lisans, atıflar ve bildirimler kaynakta korunur.
- Kaynak: [source/](source/), özgün Git ağacının normal dosyalar olarak birebir tam kopyası.

NextOpenSource normal şekilde klonlandığında kaynak ağacının tamamı gelir; submodule başlatmak gerekmez. NextID bu sabit kaynak sürümünü derleme girdisi olarak kullanabilir. Yerelleştirilmiş veri, temalar, eklentiler, Dockerfile ve ürün yapılandırması kendi bağımsız ürün deposunda kalır.

Mevcut kişisel NextID, Core konteyner imajı üzerine NextLog dinleyicisi eklentisini ekler. Gelecekteki HCC teslimat modeli özgün Keycloak kaynak kodunu, incelenmiş Core derleme çıktısını ve özelleştirilmiş NextID ürün imajını ayırır. Bu kaynak kaydı derleme veya imaj yayını yetkisi vermez. Tekrarlanabilir derleme için kesin NextOpenSource commit'ini ve imaj özetini kaydet; değişken `latest` etiketine güvenme. Depo herkese açıktır; Dockerfile'a kimlik bilgisi yazma.

Üst kaynak kopyası yalnızca incelenmiş PR ile güncellenir; kesin ağaç özeti doğrulanır, lisans ve bildirimler korunur; üretim öncesi NextSecurity değerlendirmesi, derleme ve regresyon testi yapılır. Otomatik güncelleme veya yayın etkin değildir.
