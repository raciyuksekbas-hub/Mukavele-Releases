# Mukavele

Mukavele, avukatlık ücret sözleşmesi taslaklarının düzenli, hızlı ve standart bir biçimde hazırlanmasına yardımcı olan yerel bir masaüstü uygulamasıdır.

Uygulamanın amacı, avukatın her sözleşmede yeniden yazmak zorunda kaldığı ortak bilgileri ve hükümleri yapılandırılmış bir arayüz üzerinden alarak düzenlenebilir bir Microsoft Word (DOCX) taslağı oluşturmaktır.

Mukavele, kullanıcı adına hukukî karar vermez ve avukatın meslekî değerlendirmesinin yerine geçmez. Ürettiği belgeler taslak niteliğindedir.

Bu depo, uygulamanın **dağıtım paketlerini** barındırır. Uygulamanın kaynak kodu bu depo üzerinden yayımlanmamaktadır.

---

## İndirme

| Platform | Durum | Paket | İndirme |
|---|---|---|---|
| macOS 12 (Monterey) ve üzeri — Apple Silicon (arm64) | Kararlı sürüm | `Mukavele-2.0.0-arm64.dmg` | [v2.0.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.0.0) |
| Windows 10 / 11 — x64 | Kararlı sürüm | `Mukavele-2.0.0-windows-x64-setup.exe` (kurulum) | [v2.0.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.0.0) |
| Windows 10 / 11 — x64 | Kararlı sürüm | `Mukavele-2.0.0-windows-x64-portable.zip` (kurulumsuz) | [v2.0.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.0.0) |

macOS paketi yalnızca **Apple Silicon (arm64)** işlemcili Mac bilgisayarlar için üretilmiştir. Intel işlemcili Mac'ler için ayrı bir paket bulunmamaktadır ve paket "universal" değildir.

Windows paketi **64 bit (x64)** sistemler içindir.

Her iki platform için güncel kararlı sürüm **2.0.0**'dır. macOS ve Windows paketleri aynı kaynaktan üretilir ve aynı özellik setine sahiptir.

### Önceki sürümler

Eski paketler release sayfalarında erişilebilir durumdadır:

- [v1.5.1](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v1.5.1)
- [v1.4.1](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v1.4.1)
- [v1.4.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v1.4.0)

Yeni kurulumlar için 2.0.0 sürümü önerilir.

### Paket doğrulama

v2.0.0 paketleri aşağıdaki kaynak sürümünden üretilmiştir:

```
Source build commit: 00b1b32ae67ad5a47b81129a22128facfcf2f60d
```

İndirdiğiniz dosyanın bozulmadığını doğrulamak için release sayfasındaki
SHA-256 değerlerini kullanabilirsiniz.

---

## Mukavele nedir?

Mukavele, hukukçular ve özellikle avukatlar için geliştirilmiş bir belge hazırlama uygulamasıdır.

Uygulama:

- avukatlık ücret sözleşmesi taslağı oluşturur,
- kullanıcıdan aldığı taraf, dosya ve ücret bilgilerini önceden hazırlanmış sözleşme yapısı içinde birleştirir,
- ortaya düzenlenebilir bir Word (DOCX) belgesi çıkarır,
- oluşturulan belgeyi kullanıcının kendi bilgisayarında saklar.

Uygulama:

- kullanıcı adına hukukî karar vermez,
- somut olayın hukukî değerlendirmesini yapmaz,
- hukukî danışmanlık, görüş veya temsil hizmeti sunmaz,
- avukatın meslekî kontrolünün yerini almaz.

---

## Hangi problemi çözer?

- Tekrarlanan müvekkil ve dosya bilgilerinin her sözleşmede yeniden yazılmasını azaltır.
- Sözleşmeler arasında biçim ve içerik standardı kurulmasına yardımcı olur.
- Ücret, ödeme planı, taksit ve vade bilgilerinin düzenli biçimde girilmesini sağlar.
- Kaydedilen taraf ve dosya bilgilerinin sonraki sözleşmelerde yeniden kullanılmasını kolaylaştırır.
- Hazırlanan taslağın Word üzerinde ayrıca düzenlenebilmesine imkân verir.
- Sözleşme hazırlama süresini kısaltır.

Mukavele, nihai sözleşmenin hazırlanmasında avukata yardımcı bir araçtır.

---

## Nasıl çalışır?

1. Müvekkil ve karşı taraf bilgileri girilir; daha önce kaydedilmiş taraflar yeniden kullanılabilir.
2. Dosya açılır; işin niteliği, hukuk alanı ve hukukî süreç bilgileri seçilir.
3. Ücret modeli belirlenir (maktu, nispi, karma, kalem bazlı veya dönemsel danışmanlık).
4. Ücret tutarı, KDV durumu, başarı primi, gecikme faizi, yargılama gideri avansı ve masraf kalemleri girilir.
5. Gerekiyorsa vade belirlenir veya taksitli ödeme planı oluşturulur; her taksit için tutar, vade ve açıklama girilebilir.
6. Sözleşmeye eklenecek seçenekler ve hükümler belirlenir.
7. Belge oluşturulmadan önce son hukukî kontrol uyarısı gösterilir ve kullanıcının onayı istenir.
8. Mukavele, girilen bilgileri sözleşme şablonuna işleyerek düzenlenebilir bir DOCX taslağı üretir.
9. Kullanıcı taslağı Microsoft Word veya uyumlu bir kelime işlemciyle açar.
10. Somut olaya göre hukukî ve malî son kontrol yapılır, gerekli düzeltmeler tamamlanır.
11. Kontroller tamamlandıktan sonra sözleşme tarafların kullanımına sunulur.

Oluşturulan belgelerin her sayfasında "TASLAKTIR — SON HUKUKÎ KONTROL YAPILMADAN İMZALANMAMALIDIR." ibaresi yer alır.

---

## Üretilen Belgelerin Niteliği

Mukavele tarafından oluşturulan DOCX belgeleri **taslak niteliğindedir**.

Uygulama, kullanıcının girdiği bilgiler ile uygulamadaki sözleşme şablonlarını bir araya getirir. Üretilen metin, herhangi bir somut dosya veya hukukî ilişki bakımından kendiliğinden nihai, eksiksiz ya da kullanıma hazır kabul edilmemelidir.

Taslak kullanılmadan veya imzaya sunulmadan önce kullanıcı tarafından kontrol edilmeli ve somut olayın özelliklerine göre uyarlanmalıdır.

---

## Hukukî Kontrol ve Kullanıcının Sorumluluğu

Mukavele, bir avukatın veya hukukçunun meslekî değerlendirmesinin yerine geçmez. Uygulama hukukî görüş, danışmanlık veya temsil hizmeti sunmaz. Uygulama ile kullanıcı arasında vekâlet ilişkisi kurulmaz.

Üretilen metinler taslaktır. Kullanıcı, taslağı değiştirmeden veya kontrol etmeden doğrudan kullanmamalıdır.

Aşağıdaki hususlar kullanıcı tarafından kontrol edilmelidir:

- taraf bilgileri ve tebligata elverişli adresler,
- vekâletin ve işin kapsamı,
- ücret modeli ve ücret tutarı,
- vergi, masraf ve gider hükümleri,
- ödeme planı, taksit ve vade koşulları,
- başarı primi ve gecikme faizi hükümleri,
- sona erme, fesih ve azil hükümleri,
- yetki ve uyuşmazlık çözümüne ilişkin kayıtlar,
- somut olaya uygulanacak diğer bütün hükümler.

Taslağın somut olaya, taraf iradelerine, güncel mevzuata, avukatlık meslek kurallarına ve uygulanabilir diğer düzenlemelere uygunluğu kullanıcı hukukçu tarafından değerlendirilmelidir.

Uygulama, oluşturulan taslağın eksiksiz, hatasız, güncel, her olay için uygun veya hukukî açıdan geçerli olduğunu garanti etmez.

Taslağın imzalanması, müvekkile sunulması veya üçüncü kişilere iletilmesi kararı kullanıcı hukukçunun bağımsız meslekî değerlendirmesine dayanmalıdır.

Kanunen sınırlandırılması veya kaldırılması mümkün olmayan sorumluluklar saklıdır.

---

## macOS Kurulumu

1. [v2.0.0 release sayfasını](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.0.0) açın.
2. **Assets** altındaki `Mukavele-2.0.0-arm64.dmg` dosyasını indirin.
3. DMG dosyasını açın.
4. Mukavele uygulamasını **Applications (Uygulamalar)** klasörüne sürükleyin.
5. Uygulamayı Applications klasöründen çalıştırın.

### macOS güvenlik uyarısı

macOS paketi ad-hoc imzalıdır ve **Apple notarization sürecinden geçirilmemiştir**. Bu nedenle ilk çalıştırmada aşağıdakine benzer bir uyarı görülebilir:

> "Mukavele açılamıyor çünkü Apple bu uygulamayı doğrulayamadı."

Bu durumda aşağıdaki adımlar bir kez uygulanır:

1. **Sistem Ayarları → Gizlilik ve Güvenlik** bölümünü açın.
2. Sayfanın alt kısmındaki **"Yine de Aç"** düğmesine tıklayın.
3. Açılan pencerede **"Aç"** seçeneğini seçin.

Sonraki çalıştırmalarda uygulama doğrudan açılır.

---

## Windows Kurulumu

### Setup ile kurulum (önerilen)

1. [v2.0.0 release sayfasından](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.0.0) `Mukavele-2.0.0-windows-x64-setup.exe` dosyasını indirin.
2. Dosyayı çalıştırın.
3. Windows SmartScreen uyarısı çıkarsa **"Daha fazla bilgi"** seçeneğine basın.
4. **"Yine de çalıştır"** seçeneğiyle devam edin.
5. Kurulumu tamamlayın.
6. Başlat menüsünden Mukavele'yi açın.

Kurulum yönetici yetkisi gerektirmez; uygulama yalnızca ilgili kullanıcı hesabına kurulur.

### Portable kullanım (alternatif)

1. `Mukavele-2.0.0-windows-x64-portable.zip` dosyasını indirin.
2. ZIP dosyasını kalıcı bir klasöre çıkarın.
3. Klasör içindeki `Mukavele.exe` dosyasını çalıştırın.
4. Uygulamayı ZIP dosyasının içinden doğrudan çalıştırmayın.

Windows paketi **dijital olarak imzalanmamıştır**. SmartScreen "bilinmeyen yayıncı" uyarısı bu nedenle beklenen bir durumdur.

---

## Belgelerin Kaydedildiği Yer

Üretilen sözleşme taslaklarının varsayılan kayıt konumu sürüme göre değişir:

| Platform | Varsayılan klasör |
|---|---|
| Windows | `Belgeler\Mukavele Sözleşme Taslakları` |
| macOS | `~/Documents/Mukavele Sözleşme Taslakları` |

Windows'ta "Belgeler" klasörü OneDrive'a yönlendirilmişse taslaklar yönlendirilen konuma yazılır.

1.4.0 öncesi sürümlerle oluşturulmuş belgeler eski klasörlerinde kalır; taşınmaz veya silinmez ve uygulama içinden açılmaya devam edebilir.

---

## Veriler ve Gizlilik

Mukavele yerel çalışan bir masaüstü uygulamasıdır.

- Müvekkil, dosya ve sözleşme bilgileri kullanıcının kendi bilgisayarında, yerel bir **SQLite** veritabanında saklanır.
- Uygulama, çalışmak için üyelik, çevrim içi hesap veya lisans sunucusu gerektirmez.
- Uygulamanın çalışma zamanı bağımlılıkları PySide6, python-docx, docxtpl ve Jinja2'dir; bunların tamamı yerel kütüphanelerdir.
- Uygulama kaynağında herhangi bir HTTP istemcisi, telemetri, analitik veya hata raporlama bileşeni bulunmamaktadır.
- Uygulama yapay zekâ modeli veya yapay zekâ servisi kullanmaz.

Verilerin saklandığı klasörler:

| Platform | Uygulama verisi |
|---|---|
| Windows | `%LOCALAPPDATA%\AvukatlikSozlesmeSistemi` |
| macOS | `~/Library/Application Support/AvukatlikSozlesmeSistemi` |

Bu klasörler veritabanını, uygulama günlüklerini ve yedekleri içerir. Uygulamanın kaldırılması bu klasörleri silmez.

Kullanıcı; kendi bilgisayarının güvenliğinden, verilerin yedeklenmesinden ve bu verilere erişimin denetlenmesinden sorumludur.

---

## Windows Beta Sürümü Hakkında

Windows sürümü beta aşamasındadır.

- Paket gerçek bir Windows ortamında derlenmiş ve otomatik testlerden geçirilmiştir.
- Farklı bilgisayar yapılandırmalarında, ekran ölçeklerinde ve yüksek DPI ayarlarında beklenmeyen görünüm veya davranış sorunları oluşabilir.
- Karşılaşılan sorunların bildirilmesi, sürümün olgunlaşmasına katkı sağlar.

---

## Geri Bildirim

Hata bildirimleri ve öneriler bu deponun [Issues](https://github.com/raciyuksekbas-hub/Mukavele-Releases/issues) bölümünden iletilebilir.

Bildirim yaparken aşağıdaki bilgilerin paylaşılması sorunun anlaşılmasını kolaylaştırır:

- işletim sistemi ve sürümü,
- Mukavele sürümü (örneğin `1.4.0`),
- yapılan işlem sırası,
- beklenen sonuç,
- gerçekleşen sonuç,
- varsa ekran görüntüsü.

**Önemli:** Bildirim, müvekkile veya üçüncü kişilere ait kişisel veri içeriyorsa bu bilgiler paylaşımdan önce gizlenmelidir.

---

## Telif ve Lisans

Copyright © 2026 Raci Çetin Yüksekbaş. Tüm hakları saklıdır.

Mukavele açık kaynaklı bir yazılım değildir. Yazılımın kaynak kodunun veya çalıştırılabilir sürümlerinin kullanımı, çoğaltılması, değiştirilmesi ve yeniden dağıtımı ayrıca belirlenen lisans koşullarına tabidir. Açık bir lisans verilmediği sürece herhangi bir kullanım veya yeniden dağıtım hakkı tanındığı kabul edilmez.

Bu depo yalnızca uygulamanın dağıtım dosyalarını barındırır. Uygulamanın kaynak kodu bu depo üzerinden yayımlanmamaktadır. GitHub'ın release sayfalarında otomatik olarak gösterdiği "Source code (zip/tar.gz)" bağlantıları uygulamanın kaynak kodunu içermez.

---

## Meslektaşlarıma Bir Not

Kıymetli meslektaşlarım,

Ben yazılımcı değilim. Yalnızca yapay zekâ kullanmayı seven; vibe coding yöntemiyle, yani geliştiricilerin tek tek kod satırları yazmak yerine doğal dilde ne yapmak istediklerini yapay zekâya anlatarak yazılım geliştirdiği yeni nesil yaklaşımdan yararlanıp kendimin ve meslektaşlarımın işine yarayacak araçlar üretmeye çalışan bir hukukçuyum.

Bu nedenle MetinBul’un hataları, eksikleri veya geliştirilmesi gereken yönleri olabilir. Uygulamayı kullandıkça karşılaştığınız sorunları, dileklerinizi, önerilerinizi ve eleştirilerinizi benimle paylaşırsanız, MetinBul’u birlikte daha iyi bir hale getirebiliriz.

Uygulamayı sizlere ücretsiz olarak sunuyorum. Bunun karşılığında tek beklentim; beni yetiştiren müteveffa anneannem Cemile Salman’ın aziz ruhu ve hatırası için, kendi inancınız çerçevesinde bir dua etmenizdir.

Sevgiler,
Raci

---
