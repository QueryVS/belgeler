# Infrastructure Engineering belgeler

Infrastructure Engineering(Altyapı mühendisliği), genel bir tanımdır. Bir yazılımın çalışması için genel ortamı tasarlamak,ayarlamak,yönetmek infrastructure engineering olarak adlandırabilir. Yapılması gereken işleri 4 kelime ile anlatabilsekte infrastructure engineering disiplinleri ve terminolojisi oldukça kapsamlıdır. Yazılımın üzerinde çalışacağı altyapıları yönetmek ve tasarlamak yazılımın ihtiyaçlarına göre hizmet kesintisi olmadan yapılması gerekir.

Sistem tasarımı(System Design)`da bu ölçüde ne kadar performans istendiğine, maliyetine,uptime,migration,scaling konularındaki ihtiyaçlara göre değişir. Sistem mimarisi tasarlandıktan sonra sistemi kurmak yönetmek infrastructure engineering altında farklı mühendislik disiplinlerini içerebilir.

### ilgili diğer alanlar

 - Linux System engineer
 - Linux System Manager
 - Devops Engineer
 - DevSecOps engineer
 - SecOps engineer
 - Cloud engineer
 - Cloud Systems Administrator
 - Cloud Solutions Architect
 - Cloud Security Engineer
 - Cloud Support Engineer
 - Platform Engineer

Bu alanlar Infrastructure Engineering altında Infrastructure engineering`e yardım eden alanlar.

## İçerikler

Bu içeriklerin bazıları diğer yazılarda örneğin DevOps veya Linux System Engineering/management altında olabilir. Burada daha genel bilgi o kısımlarda daha spesifik ve alan title'ı ile uygun bilgiler vereceğim. 
 - [Orchestration](orchestration.md)
   - Virtual Machine
     - Virtlib
     - VMWare
     - VirtualBox
   - Container
     - Kubernetes
     - Mesos
     - Docker Swarm
 - [Container](container.md)
   - Docker
   - containerd
   - podman
 - [Virtualization](virtualization.md)
   - System VMs
   - Process VMs
   - Virtual Machine Language
 - [Proxy](proxy.md)
   - nginx
 - [GitOPS](gitops.md)
   - IaC
     - Terraform
     - Ansible
     - Chef
     - Puppet
 - [software engineering for infrastructure](software_engineeringforinfra.md)
   - system tools
   - controller
   - Deployment Scripts
   - Monitoring service
   - Popular Language
     - Python
     - Golang
     - C/C++
 - [System Desing](system_design.md)
   - Software Architectural Patterns
 - [Benchmark](benchmark.md)
   - Devops Engineer
   - System Engineer
 - [Standards](standards.md)
   - Security
     - ISO 27001 and ISO 27002
     - OWASP Top 10
 - [Management of infrastructure](management.md)
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
 - [**Cloud**](cloud.md)
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