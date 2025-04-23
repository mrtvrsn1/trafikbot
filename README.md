# Trafik Botu Projesi

Bu proje, .NET 6 ile geliştirilen bir trafik botu sistemidir. Projede şu bileşenler bulunur:

- **TrafikBotu.API**: Proxy okuma, ayar yönetimi ve API servisi
- **TrafikBotu.Client (Blazor WebAssembly)**: Trafik başlatma arayüzü
- **TrafikBotu.BotEngine**: Selenium tabanlı tarayıcı bot motoru
- **TrafikBotu.Shared**: Ortak model katmanı
- **docker-compose.yml**: Servisleri birlikte çalıştırmak için yapılandırma

## Özellikler
- Proxy.txt'den IP'lerle giriş
- Farklı User-Agent ve gerçekçi kullanıcı simülasyonu
- Ana sayfa → blog sayfası → son makale → yorum
- Bogus ile Türkçe yorum üretimi
- Cloudflare geçme desteği
- 8 saatlik görev süresi içinde 10 trafik, en az 3 yorum

## Kurulum
```bash
git clone https://github.com/mrtvrsn1/trafikbot.git
cd trafikbot
docker-compose up --build
