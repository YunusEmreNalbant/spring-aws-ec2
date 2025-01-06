# AWS EC2 ve GitHub Actions ile Otomatik Deployment

Bu proje, AWS'in ücretsiz sunucusunda (EC2) bir uygulamanın GitHub Actions ile otomatik deployment sürecini gösterir.

## AWS EC2 Nedir?
Amazon'un sunduğu sanal sunucu hizmetidir. Free Tier kapsamında aylık 750 saat ücretsiz t2.micro sunucu kullanım hakkı verir.

## GitHub Actions Nedir?
GitHub'ın CI/CD aracıdır. Kod değişikliklerinde otomatik olarak:
- Testleri çalıştırır
- Docker imajı oluşturur
- EC2'ye deploy eder

## Nasıl Çalışır?
1. GitHub'a kod push edilir
2. GitHub Actions tetiklenir
3. Uygulama EC2'de çalışmaya başlar 