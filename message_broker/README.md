# Message Brokers Belgeler

Message broker sistemleri servisler arası asenkron iletişim kurarak gevşek bağlı (loosely coupled) mimariyi destekler.

## Temel kavramlar

- **Producer:** Mesaj üreten servis
- **Consumer:** Mesaj tüketen servis
- **Topic/Queue:** Mesajın taşındığı kanal
- **Consumer Group:** Paralel tüketim yapan mantıksal grup

## Ne zaman kullanılır?

- Senkron çağrının kırılgan olduğu akışlarda
- Yoğun trafiği dengelemek için buffering gerektiğinde
- Event-driven mimari ihtiyacında

## Protokoller (Özet)

| Protokol | Tipik katman | Taşıma |
|---|---|---|
| AMQP | Uygulama | TCP/TLS |
| MQTT | Uygulama | TCP/TLS |
| STOMP | Uygulama | TCP |
| Kafka Protocol | Uygulama/Transport | TCP |

## Operasyon checklist

- [ ] Dead-letter queue stratejisi var
- [ ] Retry/backoff politikası tanımlı
- [ ] Idempotent consumer tasarımı yapıldı
- [ ] Consumer lag alarmları tanımlandı
