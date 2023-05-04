# Summary

## docker-compose up

Bu komut, Docker Compose'unuzda belirtilen tüm hizmetleri başlatır.
Yani, web ve db hizmetlerimiz ayağa kalkacak.

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
