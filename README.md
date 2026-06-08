Apartman ve Aidat Yönetim Sistemi Projesi
# Apartman Aidat ve Yönetim Sistemi

## Proje Amacı
Bu projenin amacı, apartman ve site yöneticilerinin daireleri, apartman sakinlerini ve aidat ödemelerini terminal üzerinden kolayca takip edebileceği, nesne yönelimli programlama (OOP) tabanlı bir otomasyon geliştirmektir.

## Kullanılan Teknolojiler
- Python
- JSON
- OOP

## Kullanılan OOP Yapıları
- **Class:** `Daire`, `Aidat`, `ApartmanSistemi`, `Kisi`, `ApartmanSakini`, `Yonetici`
- **Object:** Sınıflardan `sistem`, `yeni_daire`, `yeni_sakin` gibi çeşitli nesneler türetilmiştir.
- **Inheritance:** `ApartmanSakini` ve `Yonetici` sınıfları, temel `Kisi` sınıfından miras (kalıtım) almıştır.
- **Encapsulation:** Sakinlerin TC Kimlik No ve Telefon bilgileri (`__tc_no`, `__telefon`) kapsüllenmiş ve `@property` dekoratörleri ile kontrol altına alınmıştır.
- **Polymorphism:** `bilgi_goster()` metodu, `ApartmanSakini` ve `Yonetici` sınıfları için farklı içerikler üretecek şekilde ezilmiş (override) ve çok biçimlilik sağlanmıştır.
- **Abstraction:** `Kisi` sınıfı soyut sınıf (`ABC`) olarak tasarlanmış ve kendisinden türeyen sınıfları `bilgi_goster` metodunu kullanmaya zorlamıştır.

## Proje Özellikleri
- Daire ve kullanıcı (apartman sakini) ekleme
- Daireleri ve aktif borç durumlarını listeleme
- Daire numarasına göre borç sorgulama ve arama
- JSON dosyasına veri kaydetme
- JSON dosyasından veri yükleme
- Geciken ödemeleri raporlama

## Kurulum
Projeyi çalıştırmak için terminalinizde projenin bulunduğu dizine gidin ve aşağıdaki komutu çalıştırın:

```bash
python main.py

Geliştiren
Ad Soyad: [Uğurcan Selvi]
