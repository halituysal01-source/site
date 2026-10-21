# İşletme tanıtımı

Türkçe, mobil uyumlu, HTML ve CSS ile hazırlanmış bir işletme tanıtım sayfası.
Harici paket, veritabanı, API anahtarı veya derleme işlemi gerektirmez.

## Çalıştırma

Python 3 bulunan bir ortamda depo kökünden çalıştırın:

```sh
python3 -m http.server 8000 --bind 127.0.0.1 --directory public
```

Sunucu geliştirme içindir. Durdurmak için `Ctrl+C` kullanın.
Bulut ortamındaki yeni görevlerde sunucunun yeniden başlatılması gerekir.

## Kişiselleştirme

- `public/index.html`: İşletme adını, sayfa başlığını, tanıtımını ve faaliyet alanlarını düzenleyin.
- Örnek hizmet kartlarını işletmenizin gerçek hizmetleri ve açıklamalarıyla değiştirin.
- İletişim alanına işletmenizin telefon, e-posta, adres veya sosyal profil bağlantılarını ekleyin.
- `public/styles.css`: Renk, yazı tipi ve yerleşimi düzenleyin.

İçerikteki örnek alanlar gerçek işletme, hizmet veya iletişim bilgisi iddiası taşımaz.
Yayımlamadan önce bu alanları doldurun. Statik barındırmada yayımlanacak klasör `public/` dizinidir.

## Doğrulama

Sunucu çalışırken başka bir terminalde:

```sh
curl --fail --silent http://127.0.0.1:8000/ -o /tmp/site-index.html
curl --fail --silent http://127.0.0.1:8000/styles.css -o /tmp/site-styles.css
```

Tarayıcıda masaüstü ve mobil genişliklerde menü bağlantılarını ve sayfa düzenini kontrol edin.
Bu başlangıç projesinde otomatik test paketi bulunmaz.
