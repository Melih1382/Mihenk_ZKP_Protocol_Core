# Mihenk_ZKP_Protocol_Core
# 🛡️ Mihenk ZKP Protocol Core

**Air-Gapped Sistemler ve Otonom İşlemler İçin Donanım İzolasyonlu Kriptografik Kimlik Doğrulama Katmanı**

Bu mimari; küresel veri aktarımlarında ve otonom sistemlerde mahremiyet (gizlilik), donanım seviyesinde siber güvenlik ve operasyonel otonomi arasındaki boşluğu kapatmayı hedefleyen yeni nesil bir hibrit blokzincir ve ZKP (Sıfır Bilgi İspatı) tasarımıdır.

## 📐 Sistem Mimarisi

Sistem, güvenlik ve otonomiyi üç farklı katmanda izole eden bir yapıya sahiptir:

*(Buraya yükleyeceğin zkp_flow_diagram.png dosyasının görseli gelecek - Şemanı sisteme yükledikten sonra bu kısmı GitHub'da resim eklentisi ile bağlayacağız)*

**1. Donanım Katmanı (Hardware İzolasyonu)**
Fiziksel güvenlik çipleri (TEE/CryptoKit) kullanılarak özel anahtarların (Private Key) cihaz dışına sızması engellenir. Sisteme banka seviyesinde izole ve donanım destekli erişim sağlanır.

**2. Çekirdek Katmanı (ZKP & Escrow)**
Avalanche ağı üzerinde Reentrancy korumalı Escrow (Yediemin) akıllı sözleşmeleri çalışır. ZKP (Sıfır Bilgi Kanıtı) kalkanı sayesinde işlem tutarları ve ticari/operasyonel sırlar ağdaki diğer kullanıcılardan tamamen gizlenir.

**3. Otonom Katman (AI Oracle)**
Python tabanlı geliştirilen Otonom Bot (Oracle), dış sistemlerden gelen verileri 7/24 takip eder. Doğrulama sağlandığı saniye, akıllı sözleşme insan onayı beklemeden tetiklenir ve işlem otonom olarak tamamlanır.

---

### ⚠️ Fikri Mülkiyet ve Akademik Durum
*Bu mimari, ulusal bir akademik araştırma fonu (TÜBİTAK 1001) kapsamında destek başvuru sürecindedir ve Uluslararası Patent (PCT) hazırlıkları sürmektedir. Bu nedenle projenin çekirdek kaynak kodları (Core Source Code) kapalı (Closed-Source) tutulmaktadır.* *Sistem mimarisi, TEE entegrasyonu ve ZKP devre tasarımları hakkında teknik detaylar için iletişime geçebilirsiniz.*
