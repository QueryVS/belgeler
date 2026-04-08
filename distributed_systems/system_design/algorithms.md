# System Design Algorithms

Bu doküman, dağıtık sistem tasarımında en sık kullanılan algoritma ailelerini özetler.

## 1) Leader Election

### Bully Algorithm
- En yüksek kimliğe sahip node lider olur.
- Basit ama network churn ortamında maliyetli olabilir.

### Ring Algorithm
- Mantıksal halka üzerinde seçim yapılır.
- Topolojiye bağlı gecikme dezavantajı vardır.

## 2) Consensus

### Paxos
- Güçlü teorik taban, uygulaması karmaşıktır.

### Raft
- Anlaşılabilirlik odaklı consensus protokolüdür.
- Leader tabanlı replikasyonla operasyonel olarak yaygındır.

### Zab
- ZooKeeper ekosisteminde kullanılan total order broadcast yaklaşımıdır.

## 3) Load Balancing

- Round Robin
- Least Connections
- Weighted yaklaşımlar

Seçim yapılırken yalnızca dağılım değil, sticky session, zone-aware routing ve failure mode etkileri de değerlendirilmelidir.

## 4) Gossip

Merkezi koordinasyon olmadan durum bilgisini olasılıksal şekilde yayar. Büyük ölçekli sistemlerde membership/state dissemination için etkilidir.

## 5) Byzantine Fault Tolerance

- PBFT
- Tendermint

BFT algoritmaları, kötü niyetli veya tutarsız node davranışına karşı güvenli ilerleme sağlar ancak iletişim maliyeti yüksektir.
