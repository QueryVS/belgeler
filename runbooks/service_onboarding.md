# Service Onboarding Runbook

## 1) Amaç

Yeni bir servisin organizasyon standartlarına uygun, güvenli ve işletilebilir şekilde production ortamına alınması.

## 2) Onboarding Kapsamı

Bu runbook aşağıdaki servis tipleri için kullanılabilir:

- API servisleri
- Worker/consumer servisleri
- Event-driven mikroservisler
- İç araç/operasyon servisleri

## 3) Zorunlu Teknik Gereksinimler

### 3.1 Operability

- Health check endpoint
- Readiness/Liveness kontrolü
- Structured logging
- Temel dashboard ve alarm seti

### 3.2 Reliability

- Timeout/retry/circuit breaker stratejisi
- Idempotency ihtiyacı analizi
- Graceful shutdown
- Capacity varsayımları ve limitler

### 3.3 Security

- Secret yönetimi (kod içine gömülü secret yok)
- En az yetki prensibi (least privilege)
- Dependency güvenlik taraması
- Audit log kapsamı

### 3.4 Delivery

- CI pipeline (build + test + scan)
- CD stratejisi (canary/blue-green vb.)
- Rollback prosedürü doğrulaması
- Versiyonlama ve release notları

## 4) Dokümantasyon Gereksinimleri

Servis production'a çıkmadan önce aşağıdaki dokümanlar hazır olmalıdır:

- Servis amacı ve kapsamı
- API kontratı / event şeması
- Bağımlılıklar ve upstream/downstream etkiler
- SLO/SLI tanımı
- Incident iletişim sorumluları

## 5) Onboarding Adımları

1. Mimari ve bağımlılık değerlendirmesi
2. Risk analizi (güvenlik, performans, operasyon)
3. Gözlemlenebilirlik kontrolleri
4. Kademeli yayın planı
5. Game day / failure senaryosu doğrulaması
6. Production açılış ve yakın izleme

## 6) Çıkış Kriterleri (Definition of Ready for Production)

- [ ] SLO/SLI tanımlı ve dashboard mevcut
- [ ] En az bir rollback tatbikatı yapılmış
- [ ] Alarm eşiği ve on-call rotası tanımlanmış
- [ ] Runbook linkleri servis README'sine eklenmiş
- [ ] Güvenlik ve uyumluluk kontrolleri tamamlanmış

## 7) İlk 2 Hafta İzleme Planı

- Günlük hata trendi değerlendirmesi
- Kaynak kullanımı ve autoscaling davranışı
- Alarm gürültüsü (false positive) analizi
- Müşteri etkisi geri bildirimi

## 8) Anti-Patterns

- “Önce çıkalım sonra gözlemleriz” yaklaşımı
- On-call ekip haberdar olmadan production açılışı
- SLO tanımı olmadan başarı ölçmeye çalışma
- Geri dönüş planı olmayan şema/migrasyon değişikliği
