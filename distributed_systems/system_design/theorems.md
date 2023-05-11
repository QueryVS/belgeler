# Theorems

Distributed systems'da tekrarlanmış ve hesaplanmış bazı system design'larının uygulanış aşamasında davranışları hakkında bazı teoremler ortaya çıkmıştır. Bu teoremler system design'ı yapılırken dikkate alınmalıdır.

## Teoremler

 - **CAP theorem**
 - **BASE theorem**
 - **FLP theorem**
 - **Brewer and Nash theorem**
 - **Gilbert ve Lynch theorem**
 - **Brewer theorem**
 - **Gilbert and Lynch's PACELC theorem**
 - **Brewer's CAP theorem**
 - **FLP impossibility theorem**
 - **Leslie Lamport's Byzantine fault tolerance theorem**
 - **Eric Brewer's Gossip protocol theorem**

## CAP theorem
Bir dağıtık sistemde Consistency (tutarlılık), Availability (uygunluk) ve Partition Tolerance (parçalanma toleransı) üçlüsünden en fazla ikisi sağlanabilir. Bu teorem, bir sistem tasarımında bu üç özelliğin birlikte nasıl optimize edilebileceği konusunda karar verilirken dikkate alınır.

 - **Consistency** : Her okumada en son yazma işleminden sonra elde edilen sonucun aynı olacağı garantilenir. Bu, sistemdeki her düğümün aynı veriye sahip olduğunu ve herhangi bir düğümde yapılan bir değişikliğin diğer düğümlere de yansıtıldığını ifade eder.
 - **Availability** : Sistem, herhangi bir istemci tarafından her zaman erişilebilir ve kullanılabilir olmalıdır. Bu, kullanıcıların taleplerine hızlı yanıt verilmesi gerektiği anlamına gelir.
 - **Partition Tolerance** : bir sistemde ağdaki bölünmelerin (partition) oluşması durumunda bile sistemin çalışmaya devam etmesi yeteneğidir. Yani bir ağ bölündüğünde bile her bölümdeki düğümler birbirleriyle iletişim kurabilecek ve sistem çalışmaya devam edecektir. Bu kavram, özellikle dağıtık sistemlerde önemlidir, çünkü ağda kesintiler yaşanabilir ve birçok düğüm arasındaki iletişim kaybolabilir.

## BASE theorem
Bir sistemde ACID (Atomiklik, Tutarlılık, Yalıtım, Dayanıklılık) özelliklerinin tamamının sağlanması yerine, Basically Available (temelde uygun), Soft state (geçici durum) ve Eventually consistent (sonunda tutarlı) özelliklerine önem verilmesi gerektiğini savunan teoremdir.

BASE (Basically Available, Soft state, Eventually consistent) teoremi, NoSQL veritabanı sistemleri gibi dağıtık sistemlerin tasarımında kullanılan bir ilkedir.

 - **Basically Available (Temelde Uygun Olabilir)**: Sistem, her zaman uygun olmalıdır. Ancak bazen performans düşebilir ya da hizmet kalitesi etkilenebilir.
 - **Soft state (Yumuşak Durum)**: Sistem, belirli bir zamanda doğru olmayan durumlar içerebilir. Yumuşak durum, bir zaman aralığında doğru olan verilerin, diğer zaman aralıklarında yanlış olabileceğini ifade eder.
 - **Eventually consistent (Sonunda Tutarlı)**: Sistem, bir süre sonra tamamen tutarlı hale gelmelidir. Ancak, belirli bir işlem sonrasında sistemin tamamen tutarlı olması için bir süre beklemek gerekebilir.

BASE teoremi, **ACID (Atomicity, Consistency, Isolation, Durability)** **teoreminin** zıttıdır. ACID teoremi, ilişkisel veritabanları için geliştirilmiştir ve verilerin her zaman tamamen tutarlı olması gerektiği prensibine dayanırken, BASE teoremi daha esnek bir yaklaşım benimser ve dağıtık sistemlerin özelliklerine daha uygun bir şekilde tasarlanmasına yardımcı olur.
## FLP theorem
FLP (Fischer-Lynch-Paterson) teoremi, asenkron bir sistemin en az üç düğümü arasında anlaşmazlık çözümlemesinin imkansız olduğunu matematiksel olarak kanıtlar. Bu teorem, Byzantine Generals Problem (BGP) olarak da bilinen ve aynı anda en az bir düğümün hatalı çalıştığı bir senaryoyu ele alır.

BGP, farklı yerlerdeki generallerin bir saldırı planı üzerinde anlaşmalarını gerektiren bir senaryodur. Ancak, düşmanın saldırısını engellemek için yeterli sayıda general birlikte çalışmadığında başarısız olur. Bu senaryoda, bazı generallerin yanıltıcı bilgi yayabileceği veya arızalanabileceği gibi hatalar ortaya çıkabilir. Bu nedenle, generallerin doğru bir şekilde anlaşmaya varması için, hatalı davranan generallerin etkilerini ortadan kaldırmak için bir çözümleme mekanizması gereklidir.

FLP teoremi, bu senaryoda, asenkron bir sistemde en az üç düğümün varlığında, bir kararın alınmasının imkansız olduğunu kanıtlar. Bu teorem, anlaşmazlık çözümleme için zaman aşımı, sırayla mesaj gönderme veya diğer yöntemler gibi tekniklerin kullanılamayacağı durumlarda önemli bir rol oynar.

### Byzantine Generals Problem

Byzantine Generals Problem, bir grup generallerin bir saldırı planı üzerinde anlaşmaya çalıştığı bir senaryoyu modelleyen bir problemdir. Bu senaryoda, farklı ordu birimlerinin birbirlerine mesaj gönderme yoluyla iletişim kurdukları varsayılır. Generallerin bazıları, saldırıya katılmak istemeyen veya saldırıya karşı olanlar gibi yanlış mesajlar gönderebilirler.

Bu senaryoda, her generalin iki işlemi vardır: diğer generallerle iletişim kurmak ve bir karar vermek. Ancak bazı generaller yanıltıcı mesajlar göndererek diğer generalleri yanıltabilirler. Bu nedenle, generallerin arasında güvenilir bir iletişim kurulması gerekmektedir.

Byzantine Generals Problem, dağıtık sistemlerde güvenilirlik ve doğruluk sağlamak için kullanılan Byzantine Fault Tolerance (BFT) algoritmalarının temelini oluşturur. BFT algoritmaları, tüm düğümlerin birbiriyle iletişim kurduğu ve bazı düğümlerin yanıltıcı mesajlar gönderebileceği dağıtık sistemlerde kullanılır. BFT algoritmaları, sistemdeki tüm düğümlerin karar verme sürecine katıldığı ve birlikte çalışarak doğru bir sonuca ulaşmayı amaçlayan konsensüs algoritmalarıdır.
Byzantine Generals Problem, birçok farklı algoritmanın geliştirilmesine neden olmuştur. Bunlardan bazıları şunlardır:

 - **Practical Byzantine Fault Tolerance (PBFT):** İşlemci hatası ya da düşman saldırısı gibi farklı türlerdeki hatalarla başa çıkmak için kullanılan bir algoritmadır. PBFT, düğümlerin çoğunluğunun doğru çalıştığı durumlarda çalışır ve bir lider seçerek onaylı işlemleri gerçekleştirmek için kullanılır.
 - **Proof of Stake (PoS)**: Blockchain teknolojisi kullanılarak yapılan kripto para işlemlerinin onaylanmasında kullanılan bir algoritmadır. PoS, yüksek miktarda kripto para tutanların işlemi doğrulamasına dayanır ve işlemlerin doğru şekilde gerçekleştirilmesi için çoğunluk oyu kullanılır.
 - **Federated Byzantine Agreement (FBA):** Blokzincir teknolojisi için kullanılan bir onaylama protokolüdür. FBA, birkaç farklı düğüm tarafından onaylanan bir işlemi kabul etmek için kullanılır ve blokzincirlerin merkeziyetsizleştirilmesinde önemli bir rol oynar.
 - **Directed Acyclic Graph (DAG) algoritmaları:** DAG algoritmaları, kripto para birimi işlemlerinin onaylanmasında kullanılan bir tür blokzincir teknolojisidir. Bu algoritmalar, işlemlerin onaylanması için birçok farklı düğümün bir araya gelmesine dayanır ve işlemlerin doğruluğunu sağlamak için çoğunluk oyu kullanılır.

Bu algoritmalar, Byzantine Generals Problem gibi dağıtık sistemlerin güvenilirliğiyle ilgili sorunları ele almak için tasarlanmıştır.

## Brewer and Nash theorem
Aynı anda tutarlılık, düşük gecikme süresi ve yüksek kullanılabilirliğe sahip bir ağ oluşturmanın imkansız olduğunu savunan teorem.
## Gilbert ve Lynch theorem
Bir dağıtık sistemde veri bütünlüğü sorunlarına (data integrity) karşı iki temel çözüm yolu olan "tutarlılığı arttırma" ve "kullanılabilirliği arttırma" arasında bir tercih yapılması gerektiği fikrini savunan teorem.
## Brewer theorem
CAP teoreminin orijinal formülasyonudur ve aynı anda consistency, availability ve partition tolerance mümkün olmadığını belirtir.
## Gilbert and Lynch's PACELC theorem
CAP teoreminden esinlenerek, tutarlılık (Consistency), uygunluk (Availability) ve bölünebilirlik (Partition tolerance) özelliklerinin yanı sıra Veri uygunluğu (Eventual consistency), yerellik (Locality) ve yönetilebilirlik (Control) özelliklerini de ekleyerek daha kapsamlı bir sistem özellikleri kategorizasyonu sunan bir teorem.
## Brewer's CAP theorem
Bir dağıtık sistemde aynı anda tutarlılık, uygunluk ve bölünebilirlik özelliklerinin sağlanamayacağını savunan teorem.
## FLP impossibility theorem
Bu teorem, asenkron mesajlaşma sistemlerinde bir arıza tespit algoritması oluşturmanın imkansız olduğunu ortaya koyar. Bu teorem, bir arıza tespit algoritması oluşturmak için belirli bir zaman aşımı süresi verildiğinde, bu algoritmanın doğru sonuç üretmesinin mümkün olmadığını gösterir.
## Leslie Lamport's Byzantine fault tolerance theorem
Bu teorem, bir dağıtık sistemde Byzantine hatalarını tolere etmek için gereken minimum sayıda düğümün hesaplanmasını sağlar. Byzantine hataları, bir düğümün hatalı davrandığı veya düğümlerin birbirleriyle uyumsuz olduğu hatalardır.
## Eric Brewer's Gossip protocol theorem
Bu teorem, bir dağıtılmış sistemde her düğümün herhangi bir başka düğüm hakkında bilgi sahibi olabileceğini ve bu bilgiyi sistemde yayabileceğini varsayar. Bu teorem, bir dağıtılmış sistemdeki veri tutarsızlıklarının, düğümler arasındaki haberleşme yetersizliğinden kaynaklanabileceğini gösterir. Gossip protokolleri, düğümler arasındaki haberleşmeyi artırarak bu tutarsızlıkları azaltmaya çalışır.