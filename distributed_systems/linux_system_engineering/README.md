# Linux System >Engineering Belgeler

Linux system engineering, Linux işletim sistemi üzerindeki sistemlerin planlama, tasarım, kurulum, yapılandırma, yönetim, güvenlik ve bakımını kapsayan bir disiplindir. Linux sistem mühendisleri, işletmelerin ihtiyaçlarına göre Linux sistemleri oluştururlar ve bu sistemlerin güvenli, performanslı ve verimli bir şekilde çalışmasını sağlarlar. Bu kapsamda, ağ, depolama, veri tabanı, uygulama ve güvenlik sistemleri gibi farklı alanlarda uzmanlaşabilirler. Linux sistem mühendisleri, sistemlerin sürekli olarak kontrol edilmesini, iyileştirilmesini ve gerekli güvenlik önlemlerinin alınmasını sağlarlar. Ayrıca, sistemlerin yedeklenmesi, sorunların giderilmesi, yama yönetimi ve performans analizleri gibi işlemler de yine Linux sistem mühendislerinin sorumlulukları arasındadır.

Linux sistem mühendisleri linux sistemlerinin, işletim sisteminin çalışma mantığını iyi bilmeli sistem parçalarına hakim olmalıdır. Bu sayede sistemde uygun şekilde değişiklik yapma,troubleshooting ve performans arttırma yapabilir. Sistemin kendisi ve üzerinde bulunan her servisin düzgün şekilde çalışabilmesini sağlamalıdır. Sistemi monitoring etme, log analizi, ve troubleshoot konusunda sisteme oldukça hakim olması gerekir.

- [Linux From Scratch](linux_from_scratch.md)
  - [LFS (Linux From Scratch)](https://www.linuxfromscratch.org/lfs/)
  - [BLFS (Beyond Linux From Scratch)](https://www.linuxfromscratch.org/blfs/)
  - [ALFS (Automated Linux From Scratch)](https://www.linuxfromscratch.org/alfs/)
  - [CLFS (Cross-Compiled Linux From Scratch)](https://trac.clfs.org/wiki/read)
- [Init Systems](init_systems.md)
  - OpenRC
  - Systemd
  - SysVinit
- [Kernel Space](kernel_space.md)
  - Syscalls
  - CPU Architecture
  - Driver
  - Firmware
  - Module
- [User Space](user_space.md)
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


## Linux'a Giriş Linux dağıtımları nasıl çalışır?

Linux dağıtımları parçalardan oluşur. Bu parçalar bir bütün halinde çalışarak işletim sistemi süreçlerinin yürümesini sağlar. Bilgisayarınızda güç tuşuna bastığınızdan işletim sisteminin açıldığı zamana kadar bu parçalar sıra ile başlatılır. Bu süreçlere hakim olmak ve linux sistemlerini parçalarını iyi bilmek hem linux kullanmayı zevkli bir hale getirir hemde linux sistemlerini istediğiniz gibi değiştirebilirsiniz. Bir sorun ile karşılaştığınızda sorunun nereden kaynaklandığını anlayabilir, araştırmanızı ona göre yapabilir veya çözüm yolunu kendiniz kafanızda kurup deneyebilirsiniz. Bir sorunun oluşmasına izin vermeden adımlarınızı ona göre atabilirsiniz.

### Süreçler:

 - Güç düğmesine basılır.
 - BIOS, donanımı kontrol eder, UEFI ise efi bölümünü okur
 - 