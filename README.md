# Mukavele

**Mukavele**, avukatların avukatlık ve hukukî danışmanlık sözleşmelerini daha hızlı, standart ve düzenli şekilde hazırlamalarına yardımcı olmak amacıyla geliştirilmiş, macOS üzerinde çalışan yerel bir masaüstü uygulamasıdır.

Uygulama; kullanıcı tarafından girilen taraf, ücret ve iş bilgilerini önceden yapılandırılmış sözleşme şablonlarına aktararak düzenlenebilir **Microsoft Word (DOCX)** belgeleri oluşturur.

Mukavele tamamen **çevrimdışı (offline)** çalışır. Kullanıcı verileri herhangi bir bulut servisine veya yapay zekâ sistemine gönderilmez.

---

# Başlıca Özellikler

- 📄 Avukatlık ücret sözleşmeleri oluşturma
- ⚖️ Maktu, nispi ve karma ücret modelleri
- 💳 Taksitli ödeme planlarının otomatik oluşturulması
- 🏢 Sürekli hukukî danışmanlık sözleşmeleri
- 🏠 Tahliye ve kira bedelinin tespiti süreçlerine ilişkin sözleşmeler
- 📝 Düzenlenebilir Microsoft Word (DOCX) çıktısı
- 💾 Yerel SQLite veritabanı ile çevrimdışı çalışma
- 🔒 Kullanıcı verilerinin cihaz dışına çıkarılmaması
- ⚠️ Belge oluşturulmadan önce hukukî kontrol uyarısı
- 📑 Oluşturulan belgelerin her sayfasında otomatik **TASLAKTIR** uyarısı

---

# Gizlilik

Mukavele tasarım gereği çevrimdışı çalışmaktadır.

- Kullanıcı verileri internet üzerinden paylaşılmaz.
- Yapay zekâ servislerine gönderilmez.
- Veriler yalnızca kullanıcının kendi bilgisayarında saklanır.
- Uygulama, çalışabilmek için çevrimiçi bir hesaba ihtiyaç duymaz.

---

# Hukukî Sorumluluk

Mukavele, bir **belge otomasyon uygulamasıdır**.

Uygulama hukukî değerlendirme yapmaz, kullanıcı yerine karar vermez ve oluşturduğu belgelerin somut olaya uygunluğunu garanti etmez.

**Oluşturulan bütün belgeler taslak niteliğindedir.**

Belgenin;

- somut olaya uygunluğu,
- güncel mevzuata uygunluğu,
- ücret hükümleri,
- taraf bilgileri,
- tarihleri,
- son hukukî ve maddi kontrolü

tamamen **son kullanıcının sorumluluğundadır.**

Belgeler, son kontroller yapılmadan imzalanmamalı ve kullanılmamalıdır.

---

# Sistem Gereksinimleri

- macOS
- Apple Silicon işlemcili Mac (M1, M2, M3, M4 ve sonraki modeller)

---

# Kurulum

1. Bu sayfanın **Releases** bölümünü açın.
2. **Assets** altında bulunan **Mukavele-1.3.2-arm64.dmg** dosyasını indirin.
3. İndirilen `.dmg` dosyasını açın.
4. **Mukavele** uygulamasını **Applications (Uygulamalar)** klasörüne sürükleyin.
5. Uygulamayı **Applications** klasöründen çalıştırın.

---

# macOS Güvenlik Uyarısı

İlk çalıştırmada macOS aşağıdaki uyarıyı gösterebilir:

> "Mukavele açılamıyor çünkü Apple bu uygulamayı doğrulayamadı."

Bu normaldir.

Aşağıdaki adımları yalnızca **bir kez** uygulamanız yeterlidir:

1. **Sistem Ayarları → Gizlilik ve Güvenlik** menüsünü açın.
2. Sayfanın alt kısmındaki **"Yine de Aç"** düğmesine tıklayın.
3. Açılan pencerede tekrar **"Aç"** seçeneğini seçin.

Sonraki çalıştırmalarda uygulama normal şekilde açılacaktır.

> **Not:** Mukavele şu anda Apple Notarization sürecinden geçirilmemiştir. Bu nedenle macOS ilk çalıştırmada ek güvenlik onayı istemektedir. Uygulama doğrudan geliştiricisi tarafından GitHub üzerinden yayımlanmaktadır. İlerleyen sürümlerde Apple Notarization desteğinin eklenmesi planlanmaktadır.

---

# Geri Bildirim

Mukavele aktif olarak geliştirilmektedir.

Hata bildirimleri, öneriler ve geliştirme fikirleri her zaman memnuniyetle karşılanmaktadır.
