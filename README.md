# Mukavele

**Avukat–müvekkil ilişkisinin farklı aşamalarında kullanılan belgelerin yerel, yapılandırılmış ve denetlenebilir biçimde hazırlanmasına yardımcı masaüstü uygulaması.**

Mukavele; büro, taraf ve dosya bilgilerinin tekrar tekrar yazılmasını azaltır, önceden tanımlanmış belge yapılarını kullanıcı girdileriyle birleştirir ve belge üretimini bilgisayar üzerinde gerçekleştirir.

Uygulama kullanıcı adına hukukî karar vermez, somut olayın hukukî değerlendirmesini yapmaz ve avukatın meslekî denetiminin yerine geçmez.

> Bu depo Mukavele'nin **macOS ve Windows dağıtım paketlerini** barındırır. Kaynak kod bu public depoda yayımlanmamaktadır.

---

## Güncel sürüm: v2.2.0

Mukavele v2.2.0 ile üç belge ailesi desteklenir:

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
| **Windows 10 / 11 — x64** | Kurulum | [Mukavele-2.2.0-windows-x64-setup.exe](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/download/v2.2.0/Mukavele-2.2.0-windows-x64-setup.exe) |
| **Windows 10 / 11 — x64** | Kurulumsuz | [Mukavele-2.2.0-windows-x64-portable.zip](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/download/v2.2.0/Mukavele-2.2.0-windows-x64-portable.zip) |
| **macOS 12+ — Apple Silicon (arm64)** | DMG | [Mukavele-2.2.0-arm64.dmg](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/download/v2.2.0/Mukavele-2.2.0-arm64.dmg) |

**Release sayfası:** [Mukavele v2.2.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.2.0)

### Platform notları

- macOS paketi yalnızca **Apple Silicon (arm64)** işlemcili Mac bilgisayarlar içindir.
- Windows paketi **64 bit (x64)** sistemler içindir.
- macOS paketi Apple tarafından notarize edilmemiştir.
- Windows paketi dijital olarak imzalanmamıştır.

---

## Paket doğrulama

v2.2.0 dağıtım paketleri şu kaynak sürümünden üretilmiştir:

```text
Source build commit: bfab704b964233b6b789371d1d20c8c1d9c24496
```

SHA-256 değerleri:

```text
89b9bf95fe55fe7c52aa00f193041d7988c9b2be8e8b8b2f5b01c4da2b2cfd5d  Mukavele-2.2.0-arm64.dmg
0f263d3b6b0610d9051937a6f523bd76671e315189dfe86c4d24b03a5e1286b7  Mukavele-2.2.0-windows-x64-portable.zip
790dae86cb1fe53e279c0d3b0cbaf5928ecf399a1aa72bff0b13618fe6956688  Mukavele-2.2.0-windows-x64-setup.exe
```

Aynı değerler release içindeki [`SHA256SUMS.txt`](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/download/v2.2.0/SHA256SUMS.txt) dosyasında da yer alır.

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

- [v2.1.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.1.0)
- [v2.0.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v2.0.0)
- [v1.5.1](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v1.5.1)
- [v1.4.1](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v1.4.1)
- [v1.4.0](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases/tag/v1.4.0)

Tüm sürümler: [Releases](https://github.com/raciyuksekbas-hub/Mukavele-Releases/releases)

---

## Dağıtım deposu

Bu repository yalnızca Mukavele'nin **kullanıcıya sunulan dağıtım paketleri ve sürüm bilgileri** için kullanılmaktadır. Kaynak kod bu public repository içinde yayımlanmamaktadır.
