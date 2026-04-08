# Change Management & Rollback Runbook

## 1) Amaç

Üretim değişikliklerinin riskini düşürmek, kontrollü yayın yapmak ve sorun anında hızlı rollback sağlayabilmek.

## 2) Değişiklik Sınıflandırma

- **Standard Change:** Düşük riskli, önceden tanımlı
- **Normal Change:** Planlı, teknik inceleme gerektiren
- **Emergency Change:** Incident altında hızlı uygulanması gereken

## 3) Değişiklik Öncesi Checklist

- [ ] İş etkisi ve risk seviyesi tanımlandı
- [ ] Geri dönüş planı (rollback) yazıldı ve test edildi
- [ ] Başarı metrikleri tanımlandı (error rate, latency, saturation)
- [ ] İlgili ekipler bilgilendirildi
- [ ] Değişiklik penceresi (change window) belirlendi

## 4) Yayın Stratejileri

Tercih sırası (risk azaltma odaklı):

1. **Feature flag ile kademeli açma**
2. **Canary release**
3. **Blue/Green deployment**
4. **Big-bang release** (yalnızca zorunluysa)

## 5) Yayın Sırasında İzlenecek Sinyaller

- HTTP 5xx/4xx oranları
- P95/P99 latency
- Queue depth / consumer lag
- DB connection saturation
- CPU/memory trend sapması
- Business KPI sapması (checkout rate vb.)

## 6) Rollback Tetikleyicileri

Aşağıdaki koşullardan biri gerçekleşirse rollback değerlendirmesi başlatılır:

- Hata oranı eşik üzeri ve 5-10 dk içinde düzelmiyor
- Müşteri yolculuğunda kritik adım başarısız
- Veri bütünlüğü riski
- Güvenlik riski

## 7) Rollback Prosedürü

1. Release dondurulur.
2. Değişiklik kapsamı netleştirilir.
3. Son stabil sürüme dönüş uygulanır.
4. Veri migrasyonu varsa geri uyumluluk doğrulanır.
5. Kritik metriklerde iyileşme teyit edilir.
6. İletişim kanallarında durum güncellenir.

## 8) Değişiklik Sonrası Değerlendirme

- Beklenen kazanım gerçekleşti mi?
- Rollback readiness yeterli miydi?
- Alarm eşikleri doğru muydu?
- Runbook güncelleme ihtiyacı var mı?

## 9) Anti-Patterns

- Rollback planı olmadan production deploy
- Tek metrik üzerinden “başarılı yayın” kararı
- Dokümansız emergency change
- İletişim yapılmadan servis davranışını değiştirme
