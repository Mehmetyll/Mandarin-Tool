[🇺🇸 EN - Auto](EN-Auto-Analyze) · **🇹🇷 TR - Otomatik**

# 🔍 Otomatik Analiz Sekmesi


Sistemin farklı bölümlerini kontrol eden **14 forensik tarama** içerir. Herhangi bir alt sekmeye tıklayarak tek tek çalıştırabilir veya **Tümünü Analiz Et** ile hepsini aynı anda başlatabilirsiniz.

> ⚠️ Bazı modüller düzgün çalışmak için Yönetici yetkisi gerektirir.

---

## Modüller

| Modül | Ne kontrol eder |
|-------|----------------|
| **Prefetch** | Windows Prefetch dosyalarından program çalıştırma geçmişi |
| **USN Journal** | NTFS günlüğünden dosya oluşturma/silme/yeniden adlandırma olayları |
| **JVM** | Çalışan Java işlemleri, yüklü ajanlar, classpath bilgisi |
| **Event Log** | Program çalıştırma ile ilgili Windows Olay Günlüğü kayıtları ⚠️ |
| **Servisler** | Kurulu Windows servisleri ve çalıştırılabilir dosya yolları |
| **Registry** | Kalıcılık ve program takibi için kullanılan kayıt defteri anahtarları |
| **Site Bypass** | Hosts dosyası değişiklikleri, DNS/proxy değişiklikleri |
| **USB** | USB cihaz bağlantı geçmişi (seri no, tarih, sürücü harfi) |
| **Son Dosyalar** | Son açılan dosyalar |
| **CLI** | Komut Satırı geçmişi |
| **PowerShell** | PowerShell komut geçmişi |
| **Crash Dumps** | Çöken programların raporları ve dump dosyaları |
| **Geri Dönüşüm Kutusu** | Silinen dosyalar (orijinal ad, yol ve zaman bilgisiyle) |
| **Alt Checker** | Lunar, Feather, SKlauncher, Vanilla'daki alternatif hesaplar |

---

## ⚠️ JVM Analiz — Önemli Not

**Modrinth**, **Badlion Client** ve **SKlauncher**, JVM Analiz sonuçlarında (Injection Detected log) yanlış pozitiflere neden olabilir. Normal aktivitelerinin bazıları otomatik taramalara şüpheli görünebilir. (Test edilen istemciler: Vanilla, Lunar, Feather, Prism, Norisk vb.)

**Ancak şu durumlarda yanlış alarm DEĞİLDİR:**
- Sonuçta doğrudan bir hile adı varsa (ör. `Wurst`, `Meteor`)
- Launcher kaydının yanında "+ Suspect Detected" yazıyorsa

Sadece Modrinth/SKlauncher'da (Injection Detected log) görüyorsanız ve hile adı yoksa → muhtemelen temiz. Sonuçlarda hile adları varsa veya "+ Suspect Detected" yazıyorsa → çok yüksek ihtimalle gerçek tespit.

Ek olarak, sonuçlarda "Bypass Detected" ibaresini görürseniz, kullanıcıyı bypass yapmaya çalıştığı için şüpheli sayabilirsiniz. (Lunar Client ve Badlion Client de false verebiliyor)
