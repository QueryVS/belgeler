# GitOps Belgeler

GitOps, modern yazılım geliştirme ve dağıtım yöntemlerinden biridir ve temel olarak, bir uygulamanın geliştirme, test, dağıtım ve yönetim süreçlerinin otomasyonunu sağlamak için Git versiyon kontrol sistemini kullanır.

GitOps yaklaşımı, bir uygulamanın tüm kaynak kodunun bir Git deposunda tutulmasıyla başlar. Bu depo, uygulamanın tüm yapılandırma dosyalarını, dağıtım dosyalarını ve altyapı kaynaklarını içerebilir. Geliştirme ekibi, uygulamayı güncelleştirirken bu Git deposunu kullanır ve GitOps platformu, bu güncellemeleri alır ve altyapıya ve uygulama dağıtımına yansıtır.

GitOps platformu, bu süreci otomatikleştirmek için CI/CD araçlarını kullanır. Bu araçlar, Git depolarındaki değişiklikleri izler ve değişiklikleri altyapıda ve uygulama dağıtımında uygular. Bu sayede, uygulamanın her bir güncelleştirilmesi, tamamen otomatik ve tutarlı bir şekilde dağıtılır.

Bu yaklaşımın bir diğer önemli özelliği, altyapı ve uygulama kaynaklarının kod olarak yönetilmesidir. Bu, altyapıyı bir şekilde kod haline getirerek, altyapıyı hızlı ve güvenli bir şekilde yeniden oluşturabilmeyi ve hata ayıklamayı kolaylaştırır.

GitOps, birçok avantajı olan modern bir yaklaşımdır. Bu yaklaşım, uygulama dağıtım sürecinde insan hatasını en aza indirir, uygulamayı hızlı bir şekilde güncellemeye ve hata ayıklamaya olanak tanır ve altyapı ve uygulama kaynaklarını birleştirerek, daha iyi bir yönetim sağlar.

**Bu gitops'un genel tanımıdır. infrastructure engineering altında gitops'u incelediğimiz için sadece IaC(Infrastructure as Code), yaklaşımını yazacağım. GitOps yaklaşımının bir parçası olan merge requests, ci/cd konuları [Devops Engineering](../devops_engineering) bölümünde olacak.**

## Infrastructure as Code (IaC)

IaC (Infrastructure as Code), altyapı kaynaklarının, yazılım geliştirme için kullanılan kaynak kodu gibi kodlanması ve yönetilmesi anlamına gelir. Yani, altyapıyı oluşturan sunucular, ağ bileşenleri, depolama cihazları vb. gibi tüm kaynaklar, yazılım kodu gibi bir dosyada veya koda tanımlanır.

IaC, manuel olarak yapılan altyapı yönetimine göre birçok avantaj sağlar. İlk olarak, IaC, otomatikleştirme ve tekrar kullanılabilirlik sağlar. Altyapı kaynakları, kodlanarak otomatikleştirilebilir, böylece manuel işlemlere ihtiyaç kalmaz. Ayrıca, IaC kodu, yeniden kullanılabilir ve değiştirilebilir olduğu için altyapı yönetimi daha hızlı ve verimli hale gelir.

**Avantajları**:
 - tekrarlanabilirliği artırır. IaC kodu, aynı altyapıyı birden fazla kez oluşturmak için kullanılabilir. Bu, test ve üretim ortamları arasındaki tutarlılığı artırır ve altyapı kaynaklarını yönetmek için ihtiyaç duyulan süreyi azaltır.

 - değişiklik yönetimini kolaylaştırır. IaC kodu, kaynak kod yönetim sistemi kullanarak yönetilir ve versiyon kontrolü sağlar. Bu sayede, değişikliklerin tarihçesi takip edilebilir ve hataları tespit etmek ve geri almaya olanak tanır.

 - hata oranlarını azaltır. Manuel işlemler, hatalara neden olabilecek insan hatalarına açıktır. IaC, otomatikleştirme sayesinde, hataların azaltılmasına ve kaynakların tutarlı ve güvenli bir şekilde yönetilmesine yardımcı olur.

IaC yaklaşımı, modern yazılım geliştirme süreçlerinin bir parçası haline gelmiştir ve birçok büyük organizasyon tarafından kullanılmaktadır.

### IaC nasıl yazılır?

Eskiden IaC yazmak için genellikle manuel olarak yapılandırma dosyaları veya betikler kullanılırdı. Ancak bu yöntemlerde yapılandırmalar genellikle statikti ve süreç yavaş ve hatalara açıktı.

Bugün ise popüler IaC araçları, altyapı kaynaklarının kodla tanımlanmasını kolaylaştırmak için tasarlanmıştır. Bu araçlar, YAML, JSON, HCL gibi yapılandırılmış veri formatlarını kullanırlar ve bir dizi kaynak dosyasından oluşurlar.

Bununla birlikte, IaC yaklaşımına uygun olması için, altyapı kaynakları hakkında yapılan herhangi bir değişiklik, kaynak kodu yönetim sistemi kullanılarak tutulmalı ve IaC aracı tarafından yönetilmelidir. Bu yaklaşım, altyapı kaynaklarını daha iyi yönetmek, hataları azaltmak ve değişiklikleri izlemek için kullanılır.

Günümüzde basit konfügrasyon dosyaları yazarak IaC yazabilmemizi sağlayan araçlar vardır. 

#### Bazı IaC araçları:

 - **Terraform** 
 - **Ansible** 
 - **Chef** 
 - **Puppet**  