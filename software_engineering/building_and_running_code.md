# Building and Running Code

## Build stratejisi

- Deterministic build (aynı input -> aynı output)
- Versiyon kilitleme (lockfile)
- Repeatable CI pipeline

## Çalıştırma ortamı

- Development / Staging / Production ayrımı
- Ortam bazlı config ve secret yönetimi
- Runtime health check'leri

## Dağıtım önerileri

- Küçük ve sık release
- Canary veya kademeli geçiş
- Rollback hazır olmadan deploy yapma

## Kontrol listesi

- [ ] Build cache ve artifact stratejisi tanımlı
- [ ] CI içinde test + güvenlik taraması var
- [ ] Runtime gözlemlenebilirlik açık
