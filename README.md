# QueryVS Belgeler

QueryVS Belgeler; **Distributed Systems**, **Infrastructure Engineering**, **Software Engineering** ve ilişkili alanlarda Türkçe teknik bilgi üretmek için hazırlanmış yaşayan bir dokümantasyon projesidir.

Bu repo kişisel notlardan evrilmiş olsa da artık hedefi; ekiplerin onboarding, tasarım kararları, operasyonel müdahale ve teknik standartlar için güvenilir bir referans oluşturmaktır.

## 1) Amaç ve Tasarım İlkeleri

Bu proje aşağıdaki ilkelerle yönetilir:

- **Doğruluk:** Belirsiz, doğrulanmamış veya bağlamı eksik içerik yayınlanmaz.
- **İzlenebilirlik:** Her önemli teknik iddia için kaynak veya pratik deneyim bağlamı verilir.
- **Operasyonel değer:** Yalnızca teori değil; runbook, kontrol listesi ve karar çerçevesi üretilir.
- **Sürdürülebilirlik:** Dokümanlar bir kez yazılıp bırakılmaz; sürümleme ve periyodik gözden geçirme yapılır.
- **Okunabilirlik:** Terimler tutarlı, başlık yapısı standart ve metin akışı öğrenme odaklıdır.

## 2) Bilgi Mimarisi (Information Architecture)

### Ana kategoriler

- [Distributed Systems](distributed_systems/README.md)
  - System Design
  - Infrastructure Engineering
  - Linux System Engineering
  - Linux System Management
  - DevOps Engineering
  - Site Reliability Engineering
- [Software Engineering](software_engineering/README.md)
- [Database](database/README.md)
- [Message Broker](message_broker/README.md)
- [Security](security/README.md)
- [Test Engineering](test_engineering/README.md)

### Operasyonel belgeler

- [Runbooks dizini](runbooks/README.md)
  - [Production Incident Response Runbook](runbooks/incident_response.md)
  - [Change Management & Rollback Runbook](runbooks/change_management.md)
  - [Service Onboarding Runbook](runbooks/service_onboarding.md)

### Katkı ve kalite

- [Contributing Guide](CONTRIBUTING.md)

## 3) Kimler İçin?

- Yeni başlayan mühendisler (temel kavram + bağlam kazanımı)
- Mid/Senior mühendisler (tasarım ve uygulama kararları)
- Tech Lead / Staff / Principal mühendisler (mimari yönetişim, standartlaştırma, risk azaltma)
- Operasyon/SRE ekipleri (olay yönetimi ve servis güvenilirliği)

## 4) Doküman Olgunluk Seviyeleri

Dokümanlar aşağıdaki olgunluk seviyeleriyle etiketlenmelidir:

- **Draft:** Konu ana hatları var, teknik doğrulama eksik olabilir.
- **Reviewed:** En az bir teknik gözden geçirme tamamlandı.
- **Production-ready:** Operasyonel kullanım için yeterli; runbook/checklist içeriyor.
- **Deprecated:** Yerine daha güncel yaklaşım geçmiş; sadece tarihsel referans.

## 5) Hızlı Başlangıç

1. İlgi alanınıza göre üstteki kategori dizinlerinden başlayın.
2. Kavramsal başlıkları okuyun, sonra runbook’lara geçin.
3. Bir doküman güncelleyecekseniz önce [CONTRIBUTING.md](CONTRIBUTING.md) dosyasındaki kalite kurallarını uygulayın.

## 6) Yol Haritası

- Eksik başlıklar için minimum bir “basics + anti-patterns + references” standardı getirmek
- Kategori bazında “learning path” bölümleri eklemek
- Dağınık başlıkları bir terim sözlüğüyle normalize etmek
- Her kritik alana en az bir runbook ve bir karar kaydı (ADR) eklemek

## 7) Lisans ve Kullanım

Bu depodaki içerikler açık şekilde paylaşım amacıyla yazılmıştır. Dış kullanımda kaynak gösterimi beklenir.

> Not: Bu repo bir ürün dokümantasyon portalı değil, bir mühendislik bilgi tabanıdır. Bu nedenle içerikler “nasıl düşünülür”, “nasıl tasarlanır” ve “nasıl işletilir” ekseninde ilerler.
