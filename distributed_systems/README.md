# Dağıtık Sistemler

Dağıtık sistemler; birden fazla bağımsız düğümün tek bir sistem gibi çalıştığı, ağ gecikmesi ve kısmi hata gibi gerçek dünya kısıtlarını doğrudan yöneten sistemlerdir.

## Bu kategorinin amacı

- Dağıtık sistemlerde temel kavramları netleştirmek
- Tasarım kararlarında trade-off düşüncesini yerleştirmek
- Operasyonel gerçeklik (incident, kapasite, hata toleransı) ile mimariyi birleştirmek

## Alt Başlıklar

- [System Design](system_design/README.md)
- [Infrastructure Engineering](infrastructure_engineering/README.md)
- [Linux System Engineering](linux_system_engineering/README.md)
- [Linux System Management](linux_system_management/README.md)
- [DevOps Engineering](devops_engineering/README.md)
- [Site Reliability Engineering](site_reliability_engineer/README.md)

## Temel Prensipler

1. **Her şey fail eder:** Network partition, node kaybı, dependency timeout normaldir.
2. **Latency bir özelliktir:** Uçtan uca gecikme, yalnızca performans değil, ürün deneyimidir.
3. **Tutarlılık bilinçli seçilir:** Strong consistency yüksek doğruluk sağlar; maliyeti vardır.
4. **Observability zorunludur:** Metrik, log, trace olmadan dağıtık sistem yönetilemez.
5. **Operasyon tasarımın parçasıdır:** Runbook, rollback ve capacity planı tasarım çıktısıdır.

## Öğrenme Rotası (Öneri)

1. Terminoloji + teoremler
2. Veri modelleme ve bölümlendirme stratejileri
3. Servis iletişim desenleri (sync/async)
4. Dayanıklılık kalıpları (retry, circuit breaker, backpressure)
5. Operasyon (SLO, incident response, capacity)

## Sık Yapılan Hatalar

- CAP/BASE kavramlarını bağlamsız ezberlemek
- Global transaction beklentisiyle mikroservis tasarlamak
- Gözlemlenebilirlik olmadan ölçeklendirmeye çalışmak
- “Küçük sistemde gerek yok” diyerek hata toleransını ertelemek
