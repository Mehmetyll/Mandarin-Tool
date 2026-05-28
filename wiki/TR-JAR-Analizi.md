[🇺🇸 EN - JAR Analyzer](EN-JAR-Analyzer) · **🇹🇷 TR - JAR Analizi**

# 🔬 JAR Analiz


JAR veya ZIP dosyasının içeriğini inceler. `.class` dosyalarını Java kaynak koduna çeviren yerleşik **CFR decompiler** içerir.

---

## JAR Nasıl Açılır

- **JAR Seç** butonuna tıklayıp dosya seçin
- Bir `.jar` dosyasını sürükleyip bırakın
- Mod Analiz'de sağ tık → "JAR Analiz'de Aç"

---

## Ne Görürsünüz

**Sol taraf** — Arşivdeki tüm girdileri listeleyen tablo (isim, tür, boyut).

**Sağ taraf** — Seçilen girdinin önizlemesi:
- `.class` dosyaları → decompile edilmiş Java kaynak kodu
- Metin dosyaları (`.json`, `.yml`, `.xml` vb.) → ham içerik
- Binary dosyalar → görüntülenmiyor

**Alt çubuk** — Özet: dosya boyutu, gizli mi, uzantı değişik mi, obfuscation seviyesi, toplam girdi, sınıf sayısı, ana sınıf.

---

## Temel Özellikler

- **Obfuscation tespiti** — Sınıf isimlerinde entropi analizi. Yüksek entropi = muhtemelen obfuscate edilmiş.
- **Gizli girdi tespiti** — Sıfır genişlikli Unicode karakter, nokta önekli yol veya RTL override kullanan girdileri işaretler.
- **Uzantı kontrolü** — Dosyanın gizlenip gizlenmediğini tespit eder (ör. `.png` olarak yeniden adlandırılmış JAR).
- **Arama** — Girdileri isim veya türe göre filtrele.
- **Sağ tıklama** — Girdi adını veya önizleme içeriğini kopyala.
