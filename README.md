# Mukavele

**Avukat–müvekkil ilişkisinin farklı aşamalarında kullanılan belgelerin yerel, yapılandırılmış ve denetlenebilir biçimde hazırlanmasına yardımcı masaüstü uygulaması.**

Mukavele; büro, taraf ve dosya bilgilerinin tekrar tekrar yazılmasını azaltır, önceden tanımlanmış belge yapılarını kullanıcı girdileriyle birleştirir ve belge üretimini bilgisayar üzerinde gerçekleştirir.

Uygulama kullanıcı adına hukukî karar vermez, somut olayın hukukî değerlendirmesini yapmaz ve avukatın meslekî denetiminin yerine geçmez.

> Bu depo Mukavele'nin **macOS ve Windows dağıtım paketlerini** barındırır. Kaynak kod bu public depoda yayımlanmamaktadır.

---

## Güncel sürüm: v3.0.0

Mukavele v3.0.0 ile Avukatlık Ücret Sözleşmesi yalnız dava ve icra takibi için değil, **tek seferlik hukuki hizmetler** (ihtarname, danışma, mütalaa, bağımsız dilekçe, sözleşme hazırlama ve inceleme, görüşmeye katılım) ve **sürekli hukuki danışmanlık** için de hazırlanabiliyor. Ceza işlerinde soruşturma ve infaz evreleri ayrı aşamalar olarak seçiliyor; müvekkilin sıfatı (şüpheli, sanık, hükümlü, mağdur, suçtan zarar gören, katılan) ayrıca belirleniyor. Arayüz kenar çubuklu yeni bir düzene, açık ve koyu temaya kavuştu; **Ücret Tarifeleri** ekranında AAÜT'ler ve baroların tavsiye niteliğindeki tarifeleri yer alıyor.

Bu sürüm veritabanını yükseltir: yükseltmeden önce veri klasörünüzün bir kopyasını alın (uygulama da yükseltmeden önce kendiliğinden bir yedek alır). Ayrıntılar için [v3.0.0 sürüm notlarına](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v3.0.0) bakın.

Uygulama üç belge ailesini destekler:

| Belge | Amaç |
|---|---|
| **Avukatlık Ücret Sözleşmesi** | Ücret, ödeme, işin kapsamı ve sözleşmesel hükümler için yapılandırılmış sözleşme taslağı oluşturur. |
| **İbraname** | Sona eren bir iş bakımından görev, hesaplaşma, kapanış ve ibra beyanlarının düzenlenmesine yardımcı olur. |
| **Müvekkil Talimatı** | Müvekkilin kanun yolu, sulh, feragat veya belirli bir işleme ilişkin açık talimatının kayıt altına alınmasına yardımcı olur. |

Belge üretimi **Word (`.docx`)** ve **UYAP (`.udf`)** çıktılarıyla çalışır.

İbraname ve Müvekkil Talimatında **“Dosyaya Özgü Özel Hususlar”** alanı kullanıcı tarafından doldurulur; Mukavele bu metni üretmez, değiştirmez veya özetlemez.

---

## İndirme

| Platform | Paket | İndirme |
|---|---|---|
| **Windows 10 / 11 — x64** | Kurulum | [Mukavele-3.0.0-windows-x64-setup.exe](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/download/v3.0.0/Mukavele-3.0.0-windows-x64-setup.exe) |
| **Windows 10 / 11 — x64** | Kurulumsuz | [Mukavele-3.0.0-windows-x64-portable.zip](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/download/v3.0.0/Mukavele-3.0.0-windows-x64-portable.zip) |
| **macOS 12+ — Apple Silicon (arm64)** | DMG | [Mukavele-3.0.0-arm64.dmg](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/download/v3.0.0/Mukavele-3.0.0-arm64.dmg) |

**Release sayfası:** [Mukavele v3.0.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v3.0.0)

### Platform notları

- macOS paketi yalnızca **Apple Silicon (arm64)** işlemcili Mac bilgisayarlar içindir.
- Windows paketi **64 bit (x64)** sistemler içindir.
- macOS paketi **Developer ID** ile imzalıdır, Hardened Runtime kullanır ve **Apple tarafından notarize edilmiştir**; bilet pakete iliştirildiği için ek bir adım gerekmez.
- Windows paketi dijital olarak imzalanmamıştır; SmartScreen uyarısı görülebilir.

---

## Paket doğrulama

v3.0.0 dağıtım paketleri şu kaynak sürümünden üretilmiştir:

```text
Source build commit: a5c699167c438b9164d03c36f6680fc9343a6a96
```

SHA-256 değerleri:

```text
a786229ee18924d313a8068e0f41c83c19a638d488b9a7646d6ad6ec32aff6cc  Mukavele-3.0.0-arm64.dmg
19b3d6b14906cbd6ade2e8b42269e7e8e3d87021c50fada43668b01a4f354c1a  Mukavele-3.0.0-windows-x64-setup.exe
9555138377b26cc46d4de940df52e3a7e6dd737bd72436e51f70c039690052d8  Mukavele-3.0.0-windows-x64-portable.zip
```

Aynı değerler release içindeki [`SHA256SUMS.txt`](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/download/v3.0.0/SHA256SUMS.txt) dosyasında da yer alır.

---

## Nasıl çalışır?

1. Büro, taraf ve gerekiyorsa dosya bilgileri kaydedilir.
2. Anasayfa'daki **Belge oluştur** bölümünden belge türü seçilir; sözleşmede hizmet türü (dava ve icra takibi, tek seferlik hizmet, sürekli danışmanlık) sihirbazın ilk adımlarında belirlenir.
3. Seçilen belgeye özgü bilgiler kullanıcı tarafından girilir.
4. Mukavele, bu bilgileri önceden tanımlanmış belge yapısıyla birleştirir.
5. Belge çıktıları kullanıcının bilgisayarında oluşturulur.
6. Son hukukî ve meslekî kontrol kullanıcı tarafından yapılır.

Mukavele'nin amacı hukukî muhakemeyi otomatikleştirmek değil; güvenli biçimde otomatikleştirilebilen tekrarları azaltmaktır.

---

## Yerel çalışma ve gizlilik

Mukavele **local-first** çalışan bir masaüstü uygulamasıdır.

- Müvekkil, dosya ve belge bilgileri kullanıcının kendi bilgisayarında yerel **SQLite** veritabanında tutulur.
- Belge üretimi yerel olarak gerçekleştirilir.
- Kullanım için üyelik, çevrim içi hesap veya lisans sunucusu gerekmez.
- Uygulama yapay zekâ modeli veya yapay zekâ servisi kullanmaz.
- Telemetri veya analitik amacıyla kullanıcı verisi göndermez.

---

## Belgelerin niteliği

Mukavele tarafından oluşturulan belgeler **taslak niteliğindedir**.

Uygulama:

- kullanıcı adına hukukî karar vermez,
- somut olayın hukukî değerlendirmesini yapmaz,
- hukukî görüş, danışmanlık veya temsil hizmeti sunmaz,
- avukatın meslekî değerlendirmesinin yerine geçmez.

Belgenin somut olaya, taraf iradelerine, güncel mevzuata ve uygulanabilir meslek kurallarına uygunluğu kullanıcı hukukçu tarafından değerlendirilmelidir.

---

## Önceki sürümler

- [v2.3.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.3.0)
- [v2.2.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.2.0)
- [v2.1.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.1.0)
- [v2.0.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.0.0)
- [v1.5.1](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v1.5.1)
- [v1.4.1](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v1.4.1)
- [v1.4.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v1.4.0)

Tüm sürümler: [Releases](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases)

---

## Meslektaşlarımdan Bir Ricam Var

Kıymetli meslektaşlarım,

Ben yazılımcı değilim. Yalnızca yapay zekâ kullanmayı seven; vibe coding (sezgisel yazılım/yazılımsama) yöntemiyle, yani geliştiricilerin tek tek kod satırları yazmak yerine kendi anadillerinde ne yapmak istediklerini yapay zekâya anlatarak yazılım geliştirdiği yeni nesil yaklaşımdan yararlanıp kendimin ve meslektaşlarımın işine yarayacak araçlar üretmeye çalışan bir hukukçuyum.

Bu nedenle Mukavele'nin hataları, eksikleri veya geliştirilmesi gereken yönleri olabilir. Uygulamayı kullandıkça karşılaştığınız sorunları, dileklerinizi, önerilerinizi ve eleştirilerinizi benimle paylaşırsanız, Mukavele'yi birlikte daha iyi bir hale getirebiliriz.

Uygulamayı sizlere ücretsiz olarak sunuyorum. Bunun karşılığında tek beklentim; beni yetiştiren müteveffa anneannem Cemile Salman’ın aziz ruhu ve hatırası için, kendi inancınız çerçevesinde bir dua etmenizdir.

Sevgiler,  
Raci

---

## Uygulamanın Temel Prensiplerinden Bir Tanesi

**Geliştirdiğim uygulamalar yerel olarak çalışan masaüstü uygulamalarıdır. Kullanım verileri, telemetri, analitik veriler, belge içerikleri veya diğer kullanıcı verileri bana ya da üçüncü kişilere gönderilmez; merkezi olarak toplanmaz, saklanmaz veya işlenmez. Uygulamaların temel işlevleri ve veri işleme süreçleri kullanıcının kendi cihazında gerçekleşir.**

---

## Dağıtım deposu

Bu repository yalnızca Mukavele'nin **kullanıcıya sunulan dağıtım paketleri ve sürüm bilgileri** için kullanılmaktadır. Kaynak kod bu public repository içinde yayımlanmamaktadır.
