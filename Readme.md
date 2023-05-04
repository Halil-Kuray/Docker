# Summary

## docker-compose up

Bu komut, Docker Compose'unuzda belirtilen tüm hizmetleri başlatır.
Yani, web ve db hizmetlerimiz ayağa kalkacak.

## Eğer dosya adınız docker-compose.yml değilse, 
-f parametresi ile dosya adınızı belirtin. Örneğin docker compose -f file_name.yaml up

## docker ps veya docker container ls
komutunu çalıştırarak oluşturulan container'ı görebilirsiniz.

## docker volume ls 
komutunu çalıştırarak oluşturulan volume'u görebilirsiniz.

## docker network ls 
komutunu çalıştırarak oluşturulan network'leri görebilirsiniz.

## docker-compose down

Bu komut, Docker Compose tarafından yönetilen tüm hizmetleri durdurur ve kaldırır. Yani, uygulamanızı durdurmak istediğinizde kullanabilirsiniz.

Bu komutla birlikte, Docker Compose, başlatılan tüm hizmetleri durduracak ve ayrıca veri bölümlerini de kaldıracaktır.

## docker-compose build

Bu komut, Docker Compose tarafından yönetilen tüm hizmetlerin Docker imajlarını yeniden oluşturur. Yani, uygulamanızda değişiklik yaptığınızda, Docker imajınızı güncellemek istediğinizde kullanabilirsiniz.

Bu komutla birlikte, Docker Compose, docker-compose.yml dosyasını arar ve her bir hizmet için Docker imajını yeniden oluşturur.

## docker-compose ps

Bu komut, Docker Compose tarafından yönetilen tüm hizmetlerin durumunu listeler.

Bu komutla birlikte, Docker Compose, tüm hizmetleri listeler ve hizmetlerin durumunu, hangi portların açık olduğunu ve diğer ayrıntıları gösterir.

## docker-compose logs

Bu komut, Docker Compose tarafından yönetilen tüm hizmetlerin günlüklerini görüntüler.

Bu komutla birlikte, Docker Compose, tüm hizmetlerin günlüklerini görüntüler. Günlükleri görmek için -f parametresini kullanabilirsiniz:

## docker-compose logs -f

Bu şekilde, günlüklerin gerçek zamanlı olarak güncellenmesini sağlayabilirsiniz.

# Docker Compose Bileşenleri ve Parametreleri Nelerdir?

## version

Compose dosyasının hangi compose sürümünü kullandığını belirtir. Her sürüm kendine ait özellikler ve yeni geliştirmeler içerebilir. Tüm sürümleri ve detayları için https://docs.docker.com/compose/compose-file/compose-versioning/

## services

Projenizdeki tüm container'ları tanımlar. Her container için bir isim ve build veya image komutları gerekir.

## volumes

Container'ların veri kaynaklarını tanımlar. Bu, verilerin container'lar arasında paylaşılmasını veya saklanmasını sağlar.

## networks

Container'lar arasındaki ağ bağlantılarını tanımlar.

## environment

Container'lar için ortam değişkenlerini tanımlar.

## depends_on

Container'lar arasındaki bağımlılıkları tanımlar.

## extends

Ayrı ayrı tanımlanmış olan containerların ortak olan ayarlarını kullanmak için kullanılabilir.

## ports

Containerların host makineye açacağı portlar tanımlanabilir.

## restart

Containerların nasıl yeniden başlatılacağını tanımlanabilir.

## command

Containerların başlatılırken çalıştırılması gereken komutlar tanımlanabilir.

## labels
Containerların etiketleri tanımlanabilir.

## tmpfs
Containerların tmpfs kullanmasının yapılandırılmasını yapabilirsiniz.

## build
Container'ların nasıl oluşturulduğunu tanımlar. Bu, bir Dockerfile kullanarak container'ların nasıl oluşturulduğunu belirten bir dizin belirtmenizi sağlar.

## cap_add
Container'lar için ekstra yetkiler tanımlar.

## cap_drop
Container'lar için yetkileri kaldırır.

## cgroup_parent
Container'ların cgroup parent'ını tanımlar.

## devices
Container'ların host makineye erişebileceği aygıtları tanımlar.

## dns
Container'ların DNS sunucularını tanımlar.

## dns_search
Container'ların DNS arama alanlarını tanımlar.

## entrypoint
Container'ların giriş noktasını tanımlar. Bu, container'ların nasıl çalıştırılacağını belirler ve komut satırından verilen komutları etkilemez.

## env_file
Container'lar için ortam değişkenlerinin yer aldığı bir dosya tanımlar.

## expose
Container'ların açtığı portları belirtir, ancak host makineye açılmaz.

## external_links
Container'lar için harici linkler tanımlar.

## extra_hosts
Container'lar için ekstra DNS girişlerini tanımlar.

## logging
Container'lar için günlükleme ayarlarını tanımlar.

## ulimits
Container'lar için sistem kaynak sınırlarını tanımlar.

## user
Container'lar için çalıştırılacak kullanıcıyı tanımlar.
