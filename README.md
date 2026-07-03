<div align="center">
  <h1>🌌 VOIDSUB</h1>
  <p><strong>Gerçek Zamanlı, Oyun ve Ekran İçi Çeviri Asistanı</strong></p>
</div>

---

## 📌 VOIDSUB Nedir?
VOIDSUB, masaüstünüzdeki veya oynadığınız oyunlardaki metinleri anında algılayıp, ekranınıza şık bir katman (Overlay) üzerinden çeviren yüksek performanslı bir çeviri asistanıdır. Yabancı dildeki oyunları, görsel romanları, uygulamaları veya altyazısız videoları dil engeline takılmadan, kendi dilinizde deneyimlemenizi sağlar.

## ✨ Detaylı Özellikler
Yalnızca ekranda bir metin çevirmekten ibaret değil, size özel olarak tasarlanmış geniş bir yelpaze sunar:

* **🎮 Oyun İçi OSD (On-Screen Display):** Çevirileri, oyun ekranının hemen üzerinde, göz yormayan, modern ve saydam bir pencereyle (OSD) gösterir.
* **🧠 Çoklu Optik Motor (OCR) Desteği:** 
  * **Windows OCR:** Windows'un dahili, çok hafif ve inanılmaz hızlı okuma motoru.
  * **EasyOCR / PyTorch:** Derin öğrenme (Yapay Zeka) destekli, zor fontları bile okuyabilen güçlü motor.
* **🎨 Tam Özelleştirilebilir Arayüz:** Katman penceresinin rengini, yazı tipini, boyutunu, şeffaflığını ve metin animasyonlarını (kayma, zıplama vb.) dilediğiniz gibi ayarlayabilirsiniz.
* **⚡ Yüksek Performans & GPU Desteği:** Donanım hızlandırmalı okuma motorları sayesinde metinleri saliseler içinde yakalar. CUDA uyumlu ekran kartlarında AI motorlarıyla üst düzey performans sunar.
* **🎯 Esnek Tarama & Çeviri Seçenekleri:** İster tüm ekranı otomatik taratın, ister sadece diyalog kutusunu (F6) seçin, isterseniz de tek seferlik anlık çeviri (F7) yapın.
* **🔄 Akıllı Arka Plan Güncelleyicisi:** Yeni bir sürüm çıktığında devasa setup dosyalarına gerek kalmadan kendini saniyeler içinde ufak parçalarla (yama) otomatik günceller.
* **🚀 Gelişmiş Log ve Dashboard:** Hangi motorun ne kadar hızla (MS) çeviri yaptığını arayüzdeki modern panelden anlık olarak takip edebilirsiniz.

## 🚀 Kısayol Tuşları & Kullanım
VOIDSUB, oyun oynarken odağınızı kaybetmemeniz için Global Klavye Kısayolları ile yönetilir:

| Tuş | İşlev |
| :---: | :--- |
| **`F5`** | Çeviriyi Başlat / Durdur (Motoru aktif eder veya kapatır) |
| **`F6`** | Ana Tarama Alanını Seç (Sürekli çeviri yapılacak bölgeyi belirler) |
| **`F7`** | Anlık/Geçici Bölge Çevirisi (Sadece o anlık, tek seferlik çeviri yapmak için) |
| **`F8`** | Katmanı (Çeviri Penceresini) Gizle / Göster |
| **`F9`** | Menüyü (VOIDSUB Arayüzünü) Öne Getir |

## 🛠 İndirme ve Kurulum
1. [Releases (Sürümler)](https://github.com/Nokrima/VOIDSUB/releases/latest) sayfamıza gidin.
2. En güncel sürüme ait **`setup.exe`** dosyasını indirin.
3. Kurulumu tamamladıktan sonra VOIDSUB uygulamasını çalıştırın.
4. "Motor Durumu" panelinden dilediğiniz çeviri motorunu kurun.
5. **F6** tuşu ile ekranınızdaki çevrilecek alanı seçin ve **F5** tuşu ile çeviriyi başlatın.

## ⚙️ Sistem Gereksinimleri
Kesintisiz ve akıcı bir çeviri deneyimi için tavsiye edilen gereksinimler:

* **İşletim Sistemi:** Windows 10 veya Windows 11 (64-bit zorunludur)
* **İşlemci (CPU):** Intel Core i3 / AMD Ryzen 3 ve üzeri (AI OCR için daha yüksek modeller tavsiye edilir)
* **Bellek (RAM):** Minimum 4 GB (Tavsiye edilen: 8 GB ve üzeri)
* **Ekran Kartı (GPU):** 
  * EasyOCR/PyTorch AI motoru kullanılacaksa **NVIDIA CUDA** destekli (Örn: GTX 1050 ve üzeri) ekran kartı şiddetle tavsiye edilir. (İşlemci ile de çalışır ancak hız farkı yaşanabilir).
* **Diğer Bağlantılar:** Çeviri servislerine (Google vb.) sorunsuz erişim için aktif bir internet bağlantısı.

---

## 🛡️ Güvenlik Uyarıları (Windows Defender & SmartScreen)

Kurulum esnasında veya programı ilk çalıştırdığınızda **Windows Defender, SmartScreen** veya kullandığınız üçüncü parti bir Antivirüs yazılımı size bir **güvenlik uyarısı** gösterebilir *(Örn: "Windows kişisel bilgisayarınızı korudu")*. 

Bunun sebepleri şunlardır:
1. **İmza ve Bilinirlik:** VOIDSUB, bağımsız bir geliştirici projesidir. Kurumsal şirketlere ait pahalı dijital sertifikalar barındırmadığı ve henüz Windows ekosisteminde "yaygın olarak indirilen yeni bir program" olduğu için Windows varsayılan olarak bu tür `.exe` dosyalarını şüpheli bulabilir.
2. **Ekran Yakalama ve Klavye (Hotkey) İzinleri:** Uygulama yapısı gereği **ekranınızı anlık okumak** (oyun içi metinleri taramak) ve **global klavye kısayollarını dinlemek** (F5, F6 gibi tuşlara oyun içindeyken tepki vermek) zorundadır. Antivirüs yazılımları bu tür düşük seviyeli (Low-Level Hooking) sistem izinlerini haklı olarak siber tehditlerin davranışlarına benzettiği için **"False-Positive" (Yanlış Alarm)** verebilir.

**Ne Yapmalıyım?**
* Uygulamamız tamamen şeffaftır ve arka planda kötü amaçlı herhangi bir eylem yürütmez.
* Eğer mavi ekranlı **SmartScreen engeli** ile karşılaşırsanız; **Ek Bilgi (More Info)** butonuna tıklayıp **Yine de Çalıştır (Run Anyway)** seçeneğiyle devam edebilirsiniz.
* Antivirüs programınız `setup.exe`'yi siler veya çalışmasını engellerse, VOIDSUB klasörünü güvenilir listesine *(Exclusions / Dışlamalar)* eklemeniz gerekebilir.
