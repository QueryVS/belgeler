# init sistemleri Belgeler

init sistemi bir linux dağıtımı başlatıldığından çalıştırılan ilk programdır. Process id(PID) 1 dir ve daha sonra servisleri başlatmaktan sorumludur. Diğer servicler init sisteminin child process'i olaraka başlatılır. init sistemi /sbin/init dosyasından başlatılır ve bu dosyanın çalıştırılması gerektiği linux kernel'da tanımlıdır.

kernel config'i olarak `CONFIG_INIT` değişkeni bu bilgiyi tutar, default olarak `/sbin/init` olarak tanımlıdır bu dosya sembolik link'dir ve bu sembolik link'i değiştirerek init sisteminide değiştirebilirsiniz.

Günümüzde yaygın kullanılan bazı init sistemleri;

 - [**OpenRC**]()
 - [**Systemd**]()
 - [**SysVinit**]()
 - [**Runit**]()
 - [**s6**]()

Evet init sistemleri bu şekildedir. init sistemlerinin tek amacı verilen sıra ile servisleri başlatmak durdurmak olsada systemd ek özellikler sunar ve bazı servisler ve programlar systemd'ye bağımlıdır, systemd kullanılmayan bir linux dağıtımda bu programlar çalışmazlar bu yüzden bu programların çalışması için ek programlar ve ayarlar gerekir. 

Systemd bazı linux kullanıcıları tarafından sevilmez, nedeni diğer init sistemlerine göre yavaş, büyük olması bunun nedeni sadece init sisteminden beklendiği gibi servisleri başlatma durdurma işini yapmaması ve çok fazla özelliği barındırması, bu özelliklerin init sisteminde olmasının doğru olmadığını ve init sisteminin tasarımının bu kadar karmaşık olmasının iyi birşey olmadığını savunanlar tarafından sevilmez. Ayrıca sık sık güvenlik açıkları ile gündeme gelmeyi sever.

Bu yüzden [**nosystemd**](https://nosystemd.org/) diye bir kavram vardır. Eğer nosystemd bir sisteminiz olmasını istiyorsanız servislerinizi systmd'ye bağımlı olan servislerden arındırmanız ve alternatiflerine geçmeniz o şekilde init sistemini değiştirmeniz gereklidir. Veya sadece nosystemd init sistemli linux dağıtımlarını kurabilirsiniz bu sistemler nosystemd init sistemlerine uyumlu yani systemd bağımlılığı olmayan servisler ve programlar kullanılarak inşaa edilmiştir.

**Örneğin:**

 - [**Gentoo**](https://www.gentoo.org/)
 - [**Devuan**](https://www.devuan.org/)
 - [**Artix**](https://artixlinux.org/)
 - [**Void**](https://voidlinux.org/)
 - [**Slackware**](http://www.slackware.com/)
 - [**SulinOS**](https://sulinos.github.io/)
 - [**TurkmanOS**](https://turkman.gitlab.io/devel/doc/wiki/01-sistem/index.html)
