# AstroWAMP Portable Node.js Application

> **Language / Dil:** [🇹🇷 Türkçe](README.md) | [🇬🇧 English](README_EN.md)

## Download için mesaj atın onder7@gmail.com
https://drive.google.com/file/d/1NIlF4qbY1sI4bFeWArmao9pla2ZPQsli/view?usp=sharing

https://ondernet.net/astrowamp-portable-nodejs-application

[![Proje Demo Videosu](https://img.youtube.com/vi/UdduVA40EsM/maxresdefault.jpg)](https://www.youtube.com/watch?v=UdduVA40EsM)

## 🚀 Standalone Executable

Bu, AstroWAMP Node.js uygulamasının portable (taşınabilir) versiyonudur. Node.js runtime dahil tek bir .exe dosyası olarak çalışır.

### 🎯 Tam Özellikli Geliştirme Ortamı

AstroWAMP ile aşağıdaki servisleri tek bir platformda çalıştırabilirsiniz:

- ⚡ **Apache Web Server** - Güçlü ve esnek web sunucusu
- 🐘 **PHP** - En popüler sunucu taraflı programlama dili
- 🗄️ **MySQL Database** - Güvenilir ve hızlı veritabanı yönetimi
- 🟢 **Node.js** - Modern JavaScript runtime ortamı
- 📊 **phpMyAdmin** - Kolay veritabanı yönetim arayüzü

Tüm bu servisleri tek bir tıklama ile başlatıp durdurun! Kurulum gerektirmez, tamamen portable.

<img width="1660" height="773" alt="image" src="https://github.com/user-attachments/assets/1980b6a6-015f-4531-94ed-81817e88e3ee" />

<img width="1914" height="1025" alt="image" src="https://github.com/user-attachments/assets/df255f66-d1d2-4e83-bbf9-98eff522de02" />

<img width="1971" height="634" alt="image" src="https://github.com/user-attachments/assets/5c251090-576a-4961-b34b-100902e82932" />

<img width="1917" height="1005" alt="image" src="https://github.com/user-attachments/assets/8e587391-4b6f-44e5-ace7-839d76d4b25c" />

<img width="1918" height="1029" alt="image" src="https://github.com/user-attachments/assets/288caebd-808f-48db-baed-8b581adfae41" />

<img width="1913" height="1032" alt="image" src="https://github.com/user-attachments/assets/eda1fdb3-58ab-4582-b109-da30bc79655d" />

<img width="1215" height="922" alt="image" src="https://github.com/user-attachments/assets/7bbb5f08-b6a1-4204-951a-1ff5d175c5a5" />

<img width="1303" height="894" alt="image" src="https://github.com/user-attachments/assets/68b3ec67-8cc4-4e31-af88-aca05f912cdd" />

<img width="1912" height="1029" alt="image" src="https://github.com/user-attachments/assets/4b81c527-aebd-4177-bbf2-273c20a4dad0" />


## 📦 İçindekiler

```
portable/
├── AstroWAMP-NodeApp.exe    # Ana executable (Node.js runtime dahil)
├── data/                     # Veri depolama (otomatik oluşturulur)
├── uploads/                  # Dosya yüklemeleri (otomatik oluşturulur)
└── logs/                     # Uygulama logları (otomatik oluşturulur)
```

## ⚡ Hızlı Başlangıç

### Windows

1. `AstroWAMP-NodeApp.exe` dosyasını çift tıklayın
2. Tarayıcınızda `http://localhost:5000` adresini açın
3. Kullanmaya başlayın!

## 🔧 Yapılandırma

### Port Değiştirme

Port numarasını değiştirmek için environment variable kullanın:

```cmd
set PORT=3000
AstroWAMP-NodeApp.exe
```

Veya komut satırında:

```cmd
AstroWAMP-NodeApp.exe --port 3000
```

### Farklı Konumda Çalıştırma

Tüm `portable/` klasörünü istediğiniz yere kopyalayın:
- Farklı bir sürücüye (C:, D:, E:, vb.)
- USB disk
- Network sürücü
- Bulut depolama klasörü

Executable her zaman bulunduğu klasör içinde çalışır.

## 🌐 API Endpoints

Uygulama çalıştıktan sonra şu endpoint'lere erişebilirsiniz:

- **Ana Sayfa**: `http://localhost:5000/`
- **Status API**: `http://localhost:5000/api/status`
- **System Info**: `http://localhost:5000/api/info`
- **Portable Paths**: `http://localhost:5000/api/paths`
- **Health Check**: `http://localhost:5000/api/health`

## 📝 Özellikler

✅ **Tek Dosya**: Node.js runtime dahil, ek kurulum gerektirmez
✅ **Portable**: Herhangi bir konumdan çalışır
✅ **Otomatik Klasörler**: Gerekli klasörleri otomatik oluşturur
✅ **Loglama**: Her işlem otomatik loglanır
✅ **Modern UI**: AstroWAMP tasarımıyla uyumlu arayüz
✅ **RESTful API**: Tam özellikli API endpoint'leri

## 🗂️ Veri Yönetimi

### Data Klasörü
`data/` klasörüne istediğiniz verileri kaydedebilirsiniz:
```javascript
// Örnek kullanım kodda
const filePath = path.join(DATA_DIR, 'mydata.json');
fs.writeFileSync(filePath, JSON.stringify(data));
```

### Uploads Klasörü
Dosya yüklemeleri için `uploads/` klasörü kullanılır.

### Logs Klasörü
Tüm işlemler `logs/app-YYYY-MM-DD.log` formatında loglanır.

## 🔒 Güvenlik

- Port varsayılan olarak sadece localhost'tan erişilebilir
- Dış erişim için firewall ayarları yapmanız gerekebilir
- Üretim ortamında ek güvenlik önlemleri alın

## 🐛 Sorun Giderme
### Apache (httpd start olmaz ise kurmayın unutmayın) -> VC_redist.x64.exe 

Ana proje için: AstroWAMP GitHub
### "Port Already in Use" Hatası
```cmd
# Farklı bir port kullanın
set PORT=3001
AstroWAMP-NodeApp.exe
```

### Klasörler Oluşturulmuyor
- Yazma izni olduğundan emin olun
- Yönetici olarak çalıştırın (gerekirse)

### Executable Çalışmıyor
- Windows Defender / Antivirüs kontrolü yapın
- .exe dosyasını "izin ver" listesine ekleyin

## 📊 Sistem Gereksinimleri

- **OS**: Windows 7/8/10/11 (x64)
- **RAM**: En az 256 MB
- **Disk**: En az 50 MB boş alan
- **Network**: İsteğe bağlı (sadece localhost için gerekmez)

## 🔄 Güncelleme

Yeni bir versiyon çıktığında:
1. Mevcut `data/`, `uploads/`, `logs/` klasörlerini yedekleyin
2. `AstroWAMP-NodeApp.exe` dosyasını yeni versiyonla değiştirin
3. Executable'ı çalıştırın

Verileriniz korunur!

## 📚 Daha Fazla Bilgi
Apache (httpd start olmaz ise kurmayını unutmayın) -> VC_redist.x64.exe
Ana proje için: [AstroWAMP GitHub](https://github.com/onder7/astrowamp)

## 📄 Lisans

MIT License - Özgürce kullanabilir, değiştirebilir ve dağıtabilirsiniz.

---

**❤️ ile AstroWAMP için yapıldı** | Portable Development Environment
