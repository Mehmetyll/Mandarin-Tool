[🇺🇸 EN - FAQ](EN-FAQ) · **🇹🇷 TR - SSS**

# ❓ Sık Sorulan Sorular


**S: Hangi Java sürümünü kullanmalıyım?**
Java 21 veya üzeri.

**S: Bazı modüller neden boş sonuç gösteriyor?**
Muhtemelen Yönetici olarak çalıştırmıyorsunuz. CMD'yi sağ tık → Yönetici olarak çalıştır → `java -jar MandarinTool.jar`

**S: Linux/macOS'ta çalışır mı?**
Hayır. MandarinTool sadece Windows için.

**S: Sistemimi değiştirir mi?**
Hayır. Sadece okur ve analiz eder — hiçbir şey değiştirilmez veya silinmez.

**S: "Uzantı Değişik" ne demek?**
Sahte uzantılı dosyaları tespit eder (ör. `.png` olarak yeniden adlandırılmış JAR). Magic byte kontrolü kullanır.

**S: Obfuscation tespiti nasıl çalışır?**
Sınıf dosya isimlerindeki rastgeleliği entropi analizi ile kontrol eder. Rastgele isimler = muhtemelen obfuscate edilmiş.

**S: "Tüm Diskler" şablonu nedir?**
Tüm dosya sistemini taramak yerine NTFS USN Journal kullanarak tüm sürücülerdeki JAR dosyalarını anında bulur.

---

## Yaygın Çözümler

**"Erişim engellendi" hataları**
→ Yönetici olarak çalıştırın.

**İndirme "Başarısız" gösteriyor**
→ Tekrar deneyin veya aracın linkine tıklayıp web sitesinden manuel indirin.

---

**Hala sorun mu var?** Discord: `mandalinasslee` · [GitHub Issues](https://github.com/Mehmetyll/Mandarin-Tool/issues)
