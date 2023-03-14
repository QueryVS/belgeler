# Dağıtık Sistemler

Dağıtık sistemler, birden fazla fiziksel veya sanal makinede çalışan ve bir araya getirilmiş olan yazılımlardır. Bu sistemler, büyük veri setleri, çoklu kullanıcı veya sensörler gibi büyük ölçekli problemleri çözmek için tasarlanmışlardır. Dağıtık sistemler, paralel veya seri olarak işlem yapabildiğinden, işlem gücünü veya bellek kapasitesini artırmak için birden fazla makine kullanabilirler. Aynı zamanda dağıtık sistemler, yedekleme veya hata toleransı gibi özellikleri içerebilir. Bu sebepten ötürü, dağıtık sistemlerin birçok farklı uygulamaları vardır, örneğin bulut bilgi işlem, büyük veri analitik, sosyal ağlar, sensör ağları veya kontrol sistemleri gibi.

## Dağıtık sistemler terminolojisi

 - Node / Application point: Dağıtık sistemde yer alan her bir işlem yapabilen birimler.
 - Cluster: Birkaç node arasındaki ağ bağlantısı.
 - Replica: Bir veri nesnesinin birden fazla kopyası, farklı nodlarda saklanır.
 - Consensus: Sistemdeki nodlar arasındaki veri veya eylemlerin senkronizasyonunu sağlamak için kullanılan algoritmalar.
 - Failover: Sistemdeki bir nodun arızalanması veya başka bir nedenle hizmet vermemesi durumunda, hizmeti devralacak başka bir nodun otomatik olarak aktif hale gelmesi.
 - Backup: Bir veri nesnesinin birden fazla kopyasının saklanması, olası bir arıza durumunda veri kaybını önlemek için.
 - Service Scaling: Sistemdeki trafiğe veya kullanıcı sayısına göre otomatik olarak hizmeti ölçeklendirmek için kullanılan mekanizmalar.
 - Shared Memory: Birçok nod tarafından erişilen ve kullanılan veri depolama alanı.
 - Data Partitioning: Sistemdeki verinin fiziksel veya lognik olarak nasıl bölüneceği.
 - Replica Management: Sistemdeki replikaların nasıl yönetileceği ve senkronize edileceği.
 - Data center: Sistemdeki fiziksel veya sanal makinelere erişimi sağlamak için kullanılan yer.
 - Distribüted system, distributed computing: Dağıtık sistemler genel olarak veya yapay olarak bölünen sistemler olarak tanımlanır.
 - Leader Election: Dağıtık sistemlerde önde gelen bir liderin seçilmesi için kullanılan algoritmalar.
 - Load balancing: İstekleri sistemdeki birçok noda eşit olarak dağıtmak için kullanılan mekanizmalar.
 - Partition Tolerance: Sistemin parçalanma olaylarına nasıl tepki vereceği.
 - Fault Tolerance: Sistemin hata olaylarına nasıl tepki vereceği.
 - Consistency Model: Sistemdeki verilerin nasıl senkronize edileceği ve nasıl tutarlı tutulacağı hakkında kurallar.
 - Eventual Consistency: Sistemin verilerinin zamanla tutarlı hale gelmesi beklenir.
 - Strong Consistency: Sistemde yapılan her işlem sonrası sistemin verileri tutarlı hale gelir.
 - CAP theorem: Sistemin parçalanma, tutarlılık veya performans arasında nasıl bir denge sağlayacağını tanımlayan teorem.
 - MapReduce: Büyük veri setlerini işlemek için kullanılan bir yazılım modeli.
 - Distributed Data Storage: Dağıtık sistemlerde verilerin nasıl saklanacağı ve nasıl erişileceği hakkında kurallar.
 - Gossip protocol: Dağıtık sistemlerde veri senkronizasyonu ve konsensüs sağlamak için kullanılan bir protokol.
 - Publish-Subscribe: Dağıtık sistemlerde veri dağıtımı veya etkileşim için kullanılan bir yapı.
 - Microservices: Dağıtık sistemlerde küçük ve tek odaklı hizmetlerin kullanılması.
 
### Dağıtık Sistemler hakkında önemli yazılar

 - **"Designing Data-Intensive Applications" by Martin Kleppmann**. Bu kitap, dağıtık sistemler ve büyük veri işleme teknolojileri hakkında temel kavramları ve tasarım ilkelerini anlatır.
 - **"The Morning Paper" blog, by Adrian Colyer**. Bu blog, dağıtık sistemler ve veri işleme alanlarındaki en yeni araştırmaların özetlerini sunar.
 - **"Distributed Systems for Fun and Profit" by Mikito Takada**. Bu kitap, dağıtık sistemlerin temel kavramlarını ve uygulamalarını kolayca anlaşılır bir şekilde anlatır.
 - **"Reliable, Scalable, and Maintainable Applications in the Cloud" by Jassy Lynn and Cindy Sridharan**. Bu kitap, bulut tabanlı dağıtık sistemlerin tasarımı, geliştirilmesi ve bakımı için ilkeleri anlatır.
 - **"Amazon DynamoDB: A Definitive Guide" by Rick Houlihan**. Bu kitap, Amazon'un dağıtık NoSQL veri tabanı olan DynamoDB'nin nasıl kullanılacağını anlatır.
 - **"Probabilistic Systems Analysis and Applied Probability" by Sheldon Ross**. Bu kitap, dağıtık sistemlerin performansının matematiksel olarak analiz edilmesi için gerekli olan kuramlara odaklanır.
 - **"The Part-Time Investor" by Nicholas Bloom and Benn Eifert**. Bu yazı, yatırımcıların şirketlerin dağıtık sistemlere yatırım yapmaları için nasıl değerlendirebilecekleri hakkında bilgi sağlar. Ayrıca, dağıtık sistemlerin potansiyel etkileri ve riskleri ile ilgili inceleme yapar.
 - **"Designing Data-Driven Systems" by Amr El Abbadi and Kamalakar Karlapalem**. Bu makale, büyük ölçekli veri odaklı sistemlerin tasarımında karşılaşılan çeşitli konuları kapsayan geniş bir özet sunar ve dağıtık sistemlerin mimari öğelerine odaklanır.
 - **"Kafka: The Definitive Guide" by Neha Narkhede, Gwen Shapira and Todd Palino**. Bu kitap, veri yoğun uygulamalar için yaygın olarak kullanılan dağıtık akış platformu olan Kafka'nın detaylı bir özetini sunar.
 - **"Microservices Architecture" by Irakli Nadareishvili**. Bu makale, mikro hizmet tabanlı dağıtık sistemlerin tasarımı, yapımı ve işletilmesi için ilkeler, desenler ve en iyi uygulamalara odaklanır.
 
### Dağıtık Sistemler Konusunda Takip Edilmesi ve Bakılması Gereken Kaynaklar

 - **AWS Builders Library** (https://aws.amazon.com/builders-library)
 - **Murat Demirbas** (http://muratbuffalo.blogspot.com/)
 - **Ahmet Alp Balkan** (https://www.youtube.com/@ahmetb)
 - **Cloud Native Turkiye & Kubernetes** (https://www.youtube.com/@cloudnativetr)
 - **Open Source Cloud Computing Infrastructure (Openstack)** (https://www.openstack.org/software/project-navigator/openstack-components#openstack-services)

