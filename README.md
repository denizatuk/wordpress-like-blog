# WordPress Benzeri Blog Sistemi

Modern, dinamik ve tam fonksiyonlu bir blog yönetim sistemi. WordPress benzeri özelliklere sahip, RESTful API ile çalışan basit bir CMS.

## Özellikler

- ✅ Blog yazıları yönetimi (CRUD)
- ✅ Kategoriler ve etiketler sistemi
- ✅ Yorum sistemi (onaylama/silme)
- ✅ Kullanıcı yönetimi
- ✅ Medya kütüphanesi
- ✅ Responsive tasarım
- ✅ RESTful API
- ✅ JSON tabanlı veritabanı

## Kurulum

1. Bağımlılıkları yükleyin:
```bash
npm install
```

2. Sunucuyu başlatın:
```bash
npm start
```

veya geliştirme modu için:
```bash
npm run dev
```

3. Tarayıcıda açın:
- Ana sayfa: http://localhost:3000
- Admin paneli: http://localhost:3000/admin.html

## API Endpoints

### Posts
- `GET /api/posts` - Tüm yazıları getir
- `GET /api/posts/:id` - Tek yazı getir
- `POST /api/posts` - Yeni yazı oluştur
- `PUT /api/posts/:id` - Yazı güncelle
- `DELETE /api/posts/:id` - Yazı sil

### Comments
- `GET /api/posts/:postId/comments` - Yazının yorumlarını getir
- `POST /api/posts/:postId/comments` - Yeni yorum ekle
- `GET /api/comments` - Tüm yorumları getir (admin)
- `PUT /api/comments/:id/approve` - Yorumu onayla
- `DELETE /api/comments/:id` - Yorum sil

### Categories
- `GET /api/categories` - Tüm kategorileri getir
- `POST /api/categories` - Yeni kategori ekle
- `PUT /api/categories/:id` - Kategori güncelle
- `DELETE /api/categories/:id` - Kategori sil

### Tags
- `GET /api/tags` - Tüm etiketleri getir
- `POST /api/tags` - Yeni etiket ekle

### Settings
- `GET /api/settings` - Ayarları getir
- `PUT /api/settings` - Ayarları güncelle

### Stats
- `GET /api/stats` - Dashboard istatistikleri

## Dosya Yapısı

```
├── index.html          # Ana sayfa (blog listesi)
├── single.html         # Tek yazı sayfası
├── admin.html          # Admin paneli
├── styles.css          # CSS stilleri
├── script.js           # Frontend JavaScript
├── admin.js            # Admin panel JavaScript
├── server.js           # Backend API sunucusu
├── database.json       # JSON veritabanı
├── package.json        # NPM bağımlılıkları
└── README.md          # Bu dosya
```

## Teknolojiler

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Backend**: Node.js, Express.js
- **Veritabanı**: JSON File
- **API**: RESTful

## Lisans

MIT