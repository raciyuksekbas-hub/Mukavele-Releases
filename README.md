# Mukavele

**Avukat–müvekkil ilişkisinin farklı aşamalarında kullanılan belgelerin yerel, yapılandırılmış ve denetlenebilir biçimde hazırlanmasına yardımcı masaüstü uygulaması.**

Mukavele; büro, taraf ve dosya bilgilerinin tekrar tekrar yazılmasını azaltır, önceden tanımlanmış belge yapılarını kullanıcı girdileriyle birleştirir ve belge üretimini bilgisayar üzerinde gerçekleştirir.

Uygulama kullanıcı adına hukukî karar vermez, somut olayın hukukî değerlendirmesini yapmaz ve avukatın meslekî denetiminin yerine geçmez.

> Bu depo Mukavele'nin **macOS ve Windows dağıtım paketlerini** barındırır. Kaynak kod bu public depoda yayımlanmamaktadır.

---

## Güncel sürüm: v2.3.0

Mukavele v2.3.0 ile arayüz kapsamlı biçimde yenilendi: ana bölümler **Oluştur**, **Belgeler** ve **Kayıtlar** olarak sadeleştirildi, klavye ile kullanım ve ekran okuyucu semantiği gözden geçirildi, büyük yazı ve yüksek ekran ölçeklerinde oluşan taşma sorunları giderildi.

Sözleşme motoru, belge şablonları ve veri modeli bu sürümde değişmedi; üretilen belgeler önceki sürümle aynıdır.

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
| **Windows 10 / 11 — x64** | Kurulum | [Mukavele-2.3.0-windows-x64-setup.exe](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/download/v2.3.0/Mukavele-2.3.0-windows-x64-setup.exe) |
| **Windows 10 / 11 — x64** | Kurulumsuz | [Mukavele-2.3.0-windows-x64-portable.zip](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/download/v2.3.0/Mukavele-2.3.0-windows-x64-portable.zip) |
| **macOS 12+ — Apple Silicon (arm64)** | DMG | [Mukavele-2.3.0-arm64.dmg](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/download/v2.3.0/Mukavele-2.3.0-arm64.dmg) |

**Release sayfası:** [Mukavele v2.3.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.3.0)

### Platform notları

- macOS paketi yalnızca **Apple Silicon (arm64)** işlemcili Mac bilgisayarlar içindir.
- Windows paketi **64 bit (x64)** sistemler içindir.
- macOS paketi **Developer ID** ile imzalıdır, Hardened Runtime kullanır ve **Apple tarafından notarize edilmiştir**; bilet pakete iliştirildiği için ek bir adım gerekmez.
- Windows paketi dijital olarak imzalanmamıştır; SmartScreen uyarısı görülebilir.

---

## Paket doğrulama

v2.3.0 dağıtım paketleri şu kaynak sürümünden üretilmiştir:

```text
Source build commit: 67cb6b0cd8191c2d9ad3acd958753a6df6d46eca
```

SHA-256 değerleri:

```text
02d8c1aaa6b3ef525c1a1977d4e458b2a64b169018f20dcf3ae8a2a1ae8a2045  Mukavele-2.3.0-arm64.dmg
a62ddb48bcb53af3fe17c2361ff7ccd71b273ae5669b0c0252b855135ca16482  Mukavele-2.3.0-windows-x64-setup.exe
49ab9bf537924985c10e5a8100c5265ee920ece5e92adc363ff42f16bcae475d  Mukavele-2.3.0-windows-x64-portable.zip
```

Aynı değerler release içindeki [`SHA256SUMS.txt`](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/download/v2.3.0/SHA256SUMS.txt) dosyasında da yer alır.

---

## Nasıl çalışır?

1. Büro, taraf ve gerekiyorsa dosya bilgileri kaydedilir.
2. **Belge Oluştur** ekranından belge türü seçilir.
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
