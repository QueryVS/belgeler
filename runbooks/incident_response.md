# Production Incident Response Runbook

## 1) Amaç

Production incident durumlarında MTTR'ı düşürmek, müşteri etkisini sınırlandırmak ve iletişimi standardize etmek.

## 2) Tetikleme Kriterleri

Aşağıdaki durumlardan biri varsa bu runbook aktif edilir:

- Kritik servis hata oranı (5xx) eşik üstünde
- P95/P99 gecikme ciddi sapma gösteriyor
- Veri kaybı / veri tutarsızlığı riski
- Güvenlik ihlali şüphesi
- Çoklu müşteri etkisi veya gelir etkisi

## 3) Roller ve Sorumluluklar

- **Incident Commander (IC):** Olay yönetimi, karar koordinasyonu
- **Ops Lead:** Sistem sağlığı, rollback/failover aksiyonu
- **Comms Owner:** İç/dış iletişim, status update
- **Subject Matter Expert (SME):** Derin teknik analiz
- **Scribe:** Zaman çizelgesi ve karar kaydı

## 4) İlk 15 Dakika (Golden Path)

1. Incident seviyesi belirlenir (SEV1/SEV2/SEV3).
2. War room açılır (chat + konferans).
3. IC atanır, roller netleştirilir.
4. Müşteri etkisi ve etki alanı çıkarılır.
5. En düşük riskli mitigasyon başlatılır:
   - Trafik azaltma
   - Feature flag kapatma
   - Rollback
   - Read-only moda geçiş
6. İlk status mesajı yayınlanır (maks. 15 dk içinde).

## 5) Teknik Teşhis Akışı

- Alarm kaynağı doğrula (false positive kontrolü)
- Son deploy / config değişimi kontrolü
- Bağımlı servislerin sağlık durumu
- Altyapı katmanı kontrolü (CPU, memory, IO, network)
- Veri katmanı kontrolü (replication lag, lock, saturation)
- Güvenlik sinyalleri (anormal erişim, rate spike)

## 6) Eskalasyon Kuralları

- 15 dakika içinde stabilize edilemiyorsa bir üst teknik seviye devreye alınır.
- Güvenlik etkisi varsa Security ekibi eşzamanlı dahil edilir.
- Müşteri etkisi yüksekse yönetim ve destek ekipleri bilgilendirilir.

## 7) İletişim Şablonu

- **Durum:** Investigating / Identified / Monitoring / Resolved
- **Etki:** Hangi müşteri grubu, hangi bölge, hangi fonksiyon
- **Aksiyon:** Yapılan mitigasyon
- **Sonraki güncelleme:** Kesin zaman bilgisi

Örnek: “Ödeme API’sinde artan 5xx oranını inceliyoruz. Geçici olarak trafik %30 azaltıldı. Sonraki güncelleme 20 dakika içinde paylaşılacak.”

## 8) Olay Kapatma Kriterleri

- Metri̇kler normal banda döndü
- En az 30-60 dk stabil gözlem tamamlandı
- Müşteri etkisi sona erdi
- Geçici çözüm değil, kalıcı aksiyon planı kaydedildi

## 9) Postmortem (24-72 saat)

Postmortem en az şu başlıkları içermelidir:

- Özet ve müşteri etkisi
- Zaman çizelgesi
- Root cause ve katkı sağlayan faktörler
- Neden erken yakalanamadı?
- Düzeltici / önleyici aksiyonlar (DÖF)
- Sahiplik ve teslim tarihleri

## 10) Anti-Patterns

- IC rolü netleşmeden paralel kaotik müdahale
- Kanıtsız root cause ilanı
- Status iletişimini geciktirmek
- Olay kapanmadan “tamamen düzeldi” beyanı
