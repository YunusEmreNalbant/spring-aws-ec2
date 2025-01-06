# AWS EC2 ve GitHub Actions ile Otomatik Deployment

Bu proje, AWS'in ücretsiz sunucusunda (EC2) bir uygulamanın GitHub Actions ile otomatik deployment sürecini gösterir.

## CI/CD Süreci
 Main branch'e pushlanan kod değişikliklerinde otomatik olarak:
- Testler çalıştırır
- Docker imajı oluşturulur
- EC2'ye deploy eder.

## GitHub Secrets Ayarları
Repository'de şu secret'lar tanımlanmalıdır:
- `DOCKER_USERNAME`: Docker Hub kullanıcı adı
- `DOCKER_PASSWORD`: Docker Hub şifresi/token
- `EC2_HOST`: EC2 public IP adresi
- `EC2_USERNAME`: EC2 kullanıcı adı
- `EC2_SSH_KEY`: EC2 instance'ına bağlanmak için SSH key
