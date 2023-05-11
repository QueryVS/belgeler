# QueryVS belgeler

Bu repository alanım ile ilgili aldığım notlar ve çalışma notlarımı içeren repo'dur. 

**Bulabileceğiniz başlıca konular şunlardır ;**
 - [Distributed Systems](distributed_systems/README.md)
   - [**System Design**](distributed_systems/system_design/README.md)
     - [Terminology](distributed_systems/system_design/terminology)
       - Distributed Systems Properties
         - Scalability
         - Availability
         - Reliability
         - Consistency
         - Partition Tolerance
         - Fault Tolerance
         - Performance
         - Latency
         - Throughput
         - Security
         - Privacy
         - Caching
         - Auditing
         - Load Balancing
         - Data Partitioning
         - Data Replication
         - Message Queuing
         - Request-Response Communication
         - Publish-Subscribe Communication
         - Leader Election
     - [Theorems](distributed_systems/system_design/theorems.md)
       - CAP theorem
       - BASE theorem
       - FLP theorem
       - Brewer and Nash theorem
       - Gilbert ve Lynch theorem
       - Brewer theorem
       - Gilbert and Lynch's PACELC theorem
       - Brewer's CAP theorem
       - FLP impossibility theorem
       - Leslie Lamport's Byzantine fault tolerance theorem
       - Eric Brewer's Gossip protocol theorem
     - [Algorithms](distributed_systems/system_design/algorithms.md)
       - Leader Election
         - Bully
         - Ring
         - Paxos
         - Raft
         - Zab
       - Load Balancing
         - Round Robin
         - Least Connection
         - IP Hash
         - Random
         - Weighted Round Robin
         - Weighted Least Connection
       - Consensus
         - Paxos
         - Raft
         - Zab
       - Gossip
       - MapReduce
       - Byzantine Fault Tolerance
         - PBFT
         - Tendermint
         - Algorand 
         - Bitcoin Core
     - [Best Problems](distributed_systems/system_design/best_problems.md)
   - [**Infrastructure Engineering**](distributed_systems/infrastructure_engineering/README.md)
     - [Orchestration](distributed_systems/infrastructure_engineering/orchestration.md)
       - Virtual Machine
         - Virtlib
         - VMWare
         - VirtualBox
       - Container
         - Kubernetes
         - Mesos
         - Docker Swarm
     - [Container](distributed_systems/infrastructure_engineering/container.md)
       - Docker
       - containerd
       - podman
     - [Virtualization](distributed_systems/infrastructure_engineering/virtualization.md)
       - System VMs
       - Process VMs
       - Virtual Machine Language
     - [Proxy](distributed_systems/infrastructure_engineering/proxy.md)
       - nginx
     - [GitOPS](distributed_systems/infrastructure_engineering/gitops.md)
       - IaC
         - Terraform
         - Ansible
         - Chef
         - Puppet
     - [software engineering for infrastructure](distributed_systems/infrastructure_engineering/software_engineeringforinfra.md)
       - system tools
       - controller
       - Deployment Scripts
       - Monitoring service
       - Popular Language
         - Python
         - Golang
         - C/C++
     - [System Desing](distributed_systems/infrastructure_engineering/system_design.md)
       - Software Architectural Patterns
     - [Benchmark](distributed_systems/infrastructure_engineering/benchmark.md)
       - Devops Engineer
       - System Engineer
     - [Standards](distributed_systems/infrastructure_engineering/standards.md)
       - Security
         - ISO 27001 and ISO 27002
         - OWASP Top 10
     - [Management of infrastructure](distributed_systems/infrastructure_engineering/management.md)
       - Users permission
         - Developer level
           - Database permissions
           - Monitoring permissions
           - Deployment Permissions
           - Document Permissions
         - System Manager level 
           - Orchestration Management
           - Physical Server Management
           - Database Management
           - Users Management
           - VMs Management
           - Document Permissions
       - System checklists
         - troubleshooting
         - new change monitoring
       - Documentation
         - System design
         - Permissions lists
         - Services list
         - Evolution of Infrastructure
     - [**Cloud**](distributed_systems/infrastructure_engineering/cloud.md)
       - Public cloud
         - AWS
         - HuaweiCloud
         - Azure
       - Private Cloud
         - OpenStack
           - Compute
             - compute
             - containers
           - Hardware Lifecycle
             - ironic
             - cyborg
           - Storage
             - swift
             - cinder
             - manila
           - Networking
             - neutron
             - octavia
             - designate
           - Shared
             - keystone
             - placement
             - glance
             - barbican
           - Orchestration
             - heat
             - senlin
             - mistral
             - zaqar
             - blazar
             - aodh
           - Workload Provisioning
             - magnum
             - sahara
             - trove
           - Application Lifecycle
             - masakari
             - murano
             - solum
             - freezer
           - API proxies
             - EC2API
           - Web Frontend
             - horizon
             - skyline
   - [**Linux System Engineering**](distributed_systems/linux_system_engineering/README.md)
     - [Linux From Scratch](distributed_systems/linux_system_engineering/linux_from_scratch.md)
       - [LFS (Linux From Scratch)](https://www.linuxfromscratch.org/lfs/)
       - [BLFS (Beyond Linux From Scratch)](https://www.linuxfromscratch.org/blfs/)
       - [ALFS (Automated Linux From Scratch)](https://www.linuxfromscratch.org/alfs/)
       - [CLFS (Cross-Compiled Linux From Scratch)](https://trac.clfs.org/wiki/read)
     - [Init Systems](distributed_systems/linux_system_engineering/init_systems.md)
       - OpenRC
       - Systemd
       - SysVinit
     - [Kernel Space](distributed_systems/linux_system_engineering/kernel_space.md)
       - Syscalls
       - CPU Architecture
       - Driver
       - Firmware
       - Module
     - [User Space](distributed_systems/linux_system_engineering/user_space.md)
       - Command Language
         - Bash
         - ash
         - sh
         - csh
         - zsh
       - Netwoking
         - Wireless
         - Wired
         - Virtual Network
         - Route
       - tools
         - Developing
         - System
           - File
           - Storage
           - network
       - troubleshooting
         - Monitoring
         - Log analysis
   - [**Linux System Management**](distributed_systems/linux_system_management/README.md)
     - [linux distributions](distributed_systems/linux_system_management/linux_distributions.md)
       - Debian
         - Ubuntu
         - Devuan
       - Redhat
         - Fedora
         - CentOS
       - Gentoo
       - Arch
         - Artix
     - [Package Management](distributed_systems/linux_system_management/package_management.md)
       - rpm
       - yum
       - dnf
       - apt
       - apt-get
       - aptitude
       - pacman
       - portage
     - [Networking](distributed_systems/linux_system_management/networking.md)
       - wireless
       - wired
       - virtual network
       - VPN
       - Proxy
       - Router
       - DNS
     - [Useful Tools for Management](distributed_systems/linux_system_management/useful_tools_for_management.md)
       - Terminal Multiplexer 
         - Screen
           - [screenrc](https://gitlab.com/-/snippets/2253508)
         - Tmux
       - Editor
         - vi
         - vim
         - nano
   - [**Devops Engineering**](distributed_systems/devops_engineering/README.md)
     - [GitOps](distributed_systems/devops_engineering/gitops.md)
       - Merge Requests
       - CI/CD
     - [CI/CD Services](distributed_systems/devops_engineering/cicd_services.md)
       - Jenkins (CI/CD) 
       - Tekton CI
       - Argo CD
     - [Repository Services](distributed_systems/devops_engineering/repository_services.md)
       - Nexus
       - Jfrog Artifactory
     - [Git Repository Services](distributed_systems/devops_engineering/git_repository_services.md)
       - Gitlab
     - [Project Management Services](distributed_systems/devops_engineering/project_management_services.md)
       - JIRA
       - TaskCafe
       - Trello
     - [Messaging Services](distributed_systems/devops_engineering/messaging_services.md)
       - Slack
       - Zulip
     - [Monitoring Services](distributed_systems/devops_engineering/monitoring_services.md)
       - Web Applications
         - Kibana
         - Grafana
       - zabbix
       - ELKStack
         - kibana
         - elasticsearch
         - beats
         - logstash
   - [**Site Reliability Engineering**](distributed_systems/site_reliability_engineer/README.md)
     - [**Google SRE Book**](distributed_systems/site_reliability_engineer/google_sre_book.md)
       - Preface
       - Part I. Introductory Material
       - Part II. Designing Systems
       - Part III. Implementing Systems
       - Part IV. Maintaining Systems
       - Part V. Organization and Culture
 - [**Software Engineering**](software_engineering/README.md)
   - [Fundamentals](software_engineering/fundementals.md)
     - Algorithm
       - Basic concepts
         - UML
         - Pseudo code
         - flow chart
         - O(büyük o) notation
     - Coding
       - OOP
       - clean code
       - Design Patterns
   - [Programing Languages](software_engineering/programing_languages.md)
     - interpreted
       - Python
       - PHP
       - Perl
       - Ruby
     - compiled
       - Go
       - Rust
       - C
       - C++
       - Java
   - [Building and Running Code](software_engineering/building_and_running_code.md)
     - Languages
       - Compilable Languages
       - Interpretable Languages
     - Building Code
       - cmake
       - make
       - ninja
       - GNU autotools
 - [**Database**](database/README.md)
   - Relational Database
     - PostgreSQL
     - Mysql
     - MariaDB
   - Non-Relational Database
     - MongoDB
     - Elasticsearch
 - [**Message Broker**](message_broker/README.md)
   - Apache Kafka
   - RabbitMQ
 - [**Security**](security/README.md)
   - Offensive (Red Team)
   - Defensive (Blue Team)
 - [**Test Engineering**](test_engineering/README.md)
   - [Static tests](test_engineering/static_tests.md)
   - [Dynamic tests](test_engineering/dynamic_tests.md)
     - Functional Testing
       - Unit Testing
       - Integration testing
       - System Testing
       - Acceptance Testing
     - Non-Functonal testing
       - Performance Testing
       - Security Testing
       - Compliance Testing

## QueryVS Belgeler Giriş

Bu döküman infrastructure engineering ile ilgili kapsamlı bir döküman olması amacı ile hazırlanıyor. Ayrıca kendi bilgimin üzerinden geçmem ve bunu açıklamam bana yararlı olabileceğinden hazırlamaya başladım. Bu dökümana herkes destek verebilir. Eğer bilgisayar bilimi altında burada olmayan bir kategoriyi eklemek ve katkı sunmak istiyorsanız, yapabilirsiniz. Sadece değişiklik yaptıktan sonra pull request atın.

Bu dökümanda yazan bölümlerin tamamı açık olarak dağıtılmasına ve okunmasına izin verilmektedir. Yazıların kopyalanması kullanılması serbesttir sadece açık bir şekilde kaynak belirtilmelidir. 

Belgeler'de açıklanan ve Operating System ile ilgili olan bazı bilgiler çoğunlukla Linux Dağıtımlarını baz almaktadır. Ortak bilgiler zaten ortaktır.

Belgeye farklı kategorilerde katkı sağlayabilirsiniz. Örneğin Web3 veya AI kategorisinde katkı sağlamak isterseniz bu kategori için bir dizin oluşturun ve markdown dosyalarınızı oraya yazın README.md'de yazan içerik bilgisine göre ben anamenüyü güncellerim mümkünse [README.md](README.md) dosyasında değişiklik yapmayın conflict olmaması bakımından şuan tamamlanmamış bir dosya olduğundan bu dosya sürekli güncellenmektedir.

Belgeye katkı sağlarsanız. İsminiz ve katkı sağladığınız kategori Katkı sağlayanlar kısmına yazılır.

Belgelerde kategori için yazılan açıklama ve yazılar açık olmalıdır. Herhangi bir kaynaktan kopyaladığınız içerikler kabul edilmez bu konu hakkında yeterli düzeyde bilginiz olduktan sonra chatgpt veya başka kaynaktaki bilginin anlaşılmayan yerlerini açıklayarak tekrar yazınız.

Son olarak belge Türkçe ama Yazılım mühendisliğinde terim olarak kullandığım kelimeleri İngilizce yazdım sebebi bu şekilde google'da aradığınızda İngilizce hali ile bulabileceğiniz şeyler olması, yani katkı sağlayanlar yerine contributors yazdıysam bu sebebtendir. 

### Nasıl Kullanılır (Okuyucular)

Belgeler'in kategorisine göz gezdirdikten sonra gitmek istediğiniz alanın markdown'una kategorisi linkelenmiştir. Çift tıklayarak gidin.

Belgeler kategorilerinde sıfırdan o kategori hakkında tüm bilgiler yoktur. Kategori hakkında genel ve bazı spesifik bilgiler ve terminolojisi ve ilgili kategorileri hakkında bilgiler vardır. Bir kategori birden fazla alanda yer alabilir sebebi o kategorinin sadece o alanla ilgili kısmının orda açıklanacak olmasıdır.

### Nasıl kullanılır (Contributors)

**Giriş kısmında biraz açıkladığım gibi;**

Belgeye katkı sağlarsanız. İsminiz ve katkı sağladığınız kategori Katkı sağlayanlar kısmına yazılır.

Belgelerde kategori için yazılan açıklama ve yazılar açık olmalıdır. Herhangi bir kaynaktan kopyaladığınız içerikler kabul edilmez bu konu hakkında yeterli düzeyde bilginiz olduktan sonra chatgpt veya başka kaynaktaki bilginin anlaşılmayan yerlerini açıklayarak tekrar yazınız.

### Katkı sağlayanlar:

 - Ahmet Numan Coşkun (Distributed Systems)

### Kaynaklar

Her kategorinin altında spesifik kaynaklar yazmakta buraya aklıma ilk gelen kaynakları yazdım.

 - Engineering pages
 - Scholar
 - Medium
 - Linux Documents 
   - man pages
   - info documents
 - ChatGPT and other AI apps
 - Google SRE book
 - Ahmet Alp Balkan(youtube)