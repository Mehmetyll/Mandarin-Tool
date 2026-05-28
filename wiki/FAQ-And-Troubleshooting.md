# ❓ FAQ

**🇺🇸 English** · [🇹🇷 Türkçe](SSS-TR)

**Q: What Java version do I need?**
Java 21 or higher.

**Q: Why do some modules show empty results?**
You're probably not running as Administrator (or there's really nothing). Right-click CMD → Run as admin → `java -jar MandarinTool.jar`

**Q: Does it work on Linux/macOS?**
No. MandarinTool is Windows only.

**Q: Does it modify my system?**
No. It only reads and analyzes — nothing is changed or deleted.

**Q: What is "Extension Changed"?**
It detects files with a fake extension (e.g., a JAR renamed to `.png`). Uses magic byte checking.

**Q: How does obfuscation detection work?**
Checks the randomness of class file names using entropy analysis. Random names = likely obfuscated.

**Q: What's the "All Disks" template?**
Uses the NTFS USN Journal to find all JAR files on every drive instantly instead of walking the whole filesystem.

---

## Common Fixes

**"JavaFX runtime components are missing"**
→ Use a JDK that includes JavaFX, like [Liberica Full JDK](https://bell-sw.com/pages/downloads/).

**"Access is denied" errors**
→ Run as Administrator.

**Download shows "Failed"**
→ Try again, or click the tool's link to download manually from the website.

**UI looks broken**
→ Try a different theme in Settings, or run with: `java -Dglass.win.uiScale=1.0 -jar MandarinTool.jar`

---

**Still stuck?** Discord: `mandalinasslee` · [GitHub Issues](https://github.com/Mehmetyll/Mandarin-Tool/issues)
