<div align="center">
  <h1>🌌 VOIDSUB</h1>
  <p><strong>Gerçek Zamanlı, Oyun ve Ekran İçi Çeviri Asistanı</strong></p>
  
 ---

## 📌 VOIDSUB Nedir?
VOIDSUB, masaüstünüzdeki veya oynadığınız oyunlardaki İngilizce metinleri anında algılayıp, ekranınıza şık bir katman (Overlay) üzerinden Türkçe'ye çeviren yüksek performanslı bir çeviri asistanıdır. Yabancı dildeki oyunları, görsel romanları, uygulamaları veya altyazısız videoları dil engeline takılmadan deneyimlemenizi sağlar.

**Şu an için öncelikli olarak İngilizce'den ➔ Türkçe'ye odaklanmıştır.**

## 👨‍💻 Geliştirici Notu (Projenin Hikayesi)
Bu proje devasa şirketlerin değil, **tek bir bağımsız geliştiricinin 4 aylık kesintisiz ve yoğun emeğinin** bir ürünüdür. Sıfırdan tasarlanan mimarisi, yapay zeka entegrasyonları, performans yönetimi ve UI/UX tasarımı tek elden yoğrularak, piyasadaki en akıcı ve modern "Live Translation" (Canlı Çeviri) aracı olma hedefiyle gün yüzüne çıkarılmıştır. 

## ✨ Detaylı Özellikler
VOIDSUB, sadece bir çeviri kutusundan ibaret değildir. İçerisinde pek çok "gizli" ve gelişmiş katman özelliği barındırır:

* **🎮 Gelişmiş Oyun İçi OSD (On-Screen Display):** 
  * Çeviriler, oyun ekranının hemen üzerinde modern bir pencereyle (OSD) gösterilir.
  * *Akıllı Konumlandırma:* Overlay, seçtiğiniz tarama alanına göre (snap-to-region) otomatik hizalanır.
  * *Animasyonlar:* Metinlerin şelale (waterfall) veya atlama (jump) efektleriyle ekrana gelmesini sağlayabilirsiniz.
* **🧠 Optik Motor (OCR) Desteği:** 
  * **Windows OCR:** Windows'un dahili, çok hafif ve inanılmaz hızlı okuma motoru.
  * **EasyOCR / PyTorch:** Derin öğrenme (Yapay Zeka) destekli, zor fontları bile okuyabilen güçlü AI motoru.
* **🎨 Tam Özelleştirilebilir Arayüz:** Katman penceresinin rengini, yazı tipini, boyutunu ve şeffaflığını dilediğiniz gibi ayarlayabilirsiniz.
* **⚡ Yüksek Performans & GPU Desteği:** CUDA uyumlu ekran kartlarında AI motorlarıyla (EasyOCR) üst düzey performans sunar. Bilgisayarınızı yormaz.
* **🔄 Akıllı Arka Plan Güncelleyicisi:** Yeni bir sürüm çıktığında devasa setup dosyalarına gerek kalmadan kendini ufak yamalarla otomatik günceller.
* **🚀 Dashboard:** Hangi motorun kaç milisaniyede (ms) çeviri yaptığını arayüzdeki panelden canlı olarak takip edebilirsiniz.

## 🚀 Kısayol Tuşları & Kullanım
VOIDSUB, oyun oynarken odağınızı kaybetmemeniz için Global Klavye Kısayolları ile yönetilir:

| Tuş | İşlev |
| :---: | :--- |
| **`F5`** | Çeviriyi Başlat / Durdur (Motoru aktif eder veya kapatır) |
| **`F6`** | Ana Tarama Alanını Seç / Kalibrasyon Yap |
| **`F7`** | Anlık/Geçici Bölge Çevirisi (Tek seferlik anında çeviri) |
| **`F8`** | Katmanı (Çeviri Penceresini) Gizle / Göster |
| **`F9`** | Menüyü (VOIDSUB Arayüzünü) Öne Getir |

## 🎮 En İyi Oyun Deneyimi İçin Tavsiyeler & Kalibrasyon
Programın oyunlarda kusursuz çeviri yapabilmesi için şu altın kurallara uymanız şiddetle tavsiye edilir:

1. **Görüntü Modu:** Oyunlarınızı **"Çerçevesiz Tam Ekran" (Borderless Window)** veya **"Pencereli" (Windowed)** modda oynayın. (Özel Tam Ekran (Exclusive Fullscreen) modları bazı oyunlarda OSD katmanının görünmesini engelleyebilir).
2. **Altyazı Arka Planı:** Eğer oynadığınız oyun destekliyorsa, oyun içi altyazı ayarlarından "Metin Arka Planını (Text Background) Siyah (Opak)" yapın. Bu, OCR motorunun yazıları arka plandaki karmaşık görsellerden çok daha kolay ve net ayıklamasını sağlar.
3. **Doğru Kalibrasyon (F6):** F6 tuşuna basarak seçtiğiniz tarama alanını, *oyundaki altyazıların tam çıkacağı kutunun sınırlarına göre* (ne çok dar ne çok geniş) belirleyin. Kutu dışına taşan yazılar okunmaz, çok geniş kutularda ise çeviri hızı düşebilir.

## 🛠 İndirme ve Kurulum
1. [Releases (Sürümler)](https://github.com/Nokrima/VOIDSUB/releases/latest) sayfamıza gidin.
2. En güncel sürüme ait **`setup.exe`** dosyasını indirin.
3. Kurulumu tamamladıktan sonra uygulamayı çalıştırın.
4. "Motor Durumu" panelinden dilediğiniz çeviri motorunu (örn: Windows OCR) aktif edin.
5. **F6** tuşu ile kalibrasyon (tarama) alanınızı seçip **F5** tuşu ile çeviriyi başlatın.

## ⚙️ Sistem Gereksinimleri
* **İşletim Sistemi:** Windows 10 veya Windows 11 (64-bit zorunludur)
* **İşlemci (CPU):** Intel Core i3 / AMD Ryzen 3 ve üzeri
* **Bellek (RAM):** Minimum 4 GB (Tavsiye edilen: 8 GB ve üzeri)
* **Ekran Kartı (GPU):** EasyOCR/PyTorch AI motoru için **NVIDIA CUDA** destekli (Örn: GTX 1050 ve üzeri) ekran kartı şiddetle tavsiye edilir. 
* **İnternet:** Çeviri servislerine (Google vb.) erişim için kesintisiz internet bağlantısı.

---

## 🛡️ Güvenlik Uyarıları (Windows Defender & SmartScreen)

Kurulum esnasında veya programı ilk çalıştırdığınızda **Windows Defender** veya **SmartScreen** size bir güvenlik uyarısı gösterebilir. Bunun başlıca iki sebebi vardır:

1. **İmza ve Bilinirlik:** VOIDSUB, kurumsal şirketlere ait pahalı dijital sertifikalar (EV Code Signing) barındırmayan tek kişilik bağımsız bir projedir. Windows, henüz ekosistemde "yaygınlaşmamış" yeni `.exe` dosyalarını otomatik olarak şüpheli bulabilir.
2. **Ekran Yakalama ve Low-Level Tuş İzinleri:** Uygulama, arka planda ekranınızı anlık okumak (Capture) ve global klavye tuşlarınızı (F5, F6) dinlemek zorundadır. Antivirüs yazılımları bu düşük seviyeli sistem izinlerini siber tehditlerin davranışlarına benzettiği için **"False-Positive" (Yanlış Alarm)** verir.

**Çözüm:** Mavi ekranlı SmartScreen uyarısı alırsanız **Ek Bilgi (More Info)** ➔ **Yine de Çalıştır (Run Anyway)** diyerek ilerleyebilirsiniz. Antivirüsünüz setup dosyasını engellerse, VOIDSUB'ı güvenilir (Dışlamalar) listesine eklemeniz yeterlidir. Uygulamamız %100 şeffaftır ve arka planda asla zararlı bir işlem yürütmez.

---

*Küçük büyük demeden yapacağınız her destek, uykusuz geçen gecelerin en büyük motivasyon kaynağıdır!* ❤️
