# Her K-12 Okulunun Bugün Yapabileceği 10 Hızlı Kazanım

> Bütçe gerektirmeyen ya da minimal maliyetli, hemen uygulanabilir güvenlik iyileştirmeleri. Sıralı önem derecesine göre.

## 1. Yönetici Hesaplarını Envanterleyin ve Azaltın

**Sorun:** Çoğu okulda "admin@okul" gibi paylaşılan hesaplar var, herkesin şifresi var, kim ne yaptı bilinmiyor.

**Yapılacak:** Mevcut tüm yönetici hesaplarını listele. Hangi hesap kim tarafından kullanılıyor, kim biliyor? Paylaşılan hesapları bireysel hesaplara böl. Eski personelin hesaplarını kapat.

**Süre:** 2-4 saat **Maliyet:** Sıfır

---

## 2. Misafir WiFi'ı İdari Ağdan Ayırın

**Sorun:** Veliler veya misafirler için kullanılan WiFi şifresi öğretmenlerin kullandığı ağ ile aynıysa, misafir cihazları idari ağa erişebilir.

**Yapılacak:** Modem/router'da "Guest Network" özelliğini aktif et. Bu ağ ayrı SSID ve şifre ile çalışır, ana ağdan izole edilir. Çoğu modemde tek tık ayar.

**Süre:** 30 dakika **Maliyet:** Sıfır

---

## 3. Modem ve Yönetici Arayüzlerinin Varsayılan Şifrelerini Değiştirin

**Sorun:** Birçok kurum WiFi router, switch, NVR (kamera kayıt cihazı), yazıcı vb. cihazlara fabrika çıkışı varsayılan şifreyle erişiyor. (admin/admin, admin/1234)

**Yapılacak:** Her cihazın yönetim arayüzünü açın. Varsayılan şifreyi 12+ karakterli karmaşık bir şifreyle değiştirin. Bir parola yöneticisinde saklayın.

**Süre:** 1-2 saat **Maliyet:** Sıfır (Bitwarden, KeePassXC vb. ücretsiz parola yöneticileri)

---

## 4. Yedek Almak Yetmez — Yedeği Geri Yükleyebildiğinizi Test Edin

**Sorun:** Yedek alınıyor ama 5 yıldır kimse "geri yükleme" denememiş olabilir. Felaket anında yedeğin bozuk olduğu görülür.

**Yapılacak:** Mevcut yedek sistemini incele. Son yedekten test bir dosyayı/klasörü farklı bir konuma geri yükle. Çalışıyor mu? Çalışmıyorsa düzelt. Bunu 6 ayda bir tekrarla.

**Süre:** 1-2 saat (ilk kez), sonrasında 30 dakika **Maliyet:** Sıfır

---

## 5. Otomatik Güncellemeleri Aktif Edin (İşletim Sistemi + Antivirüs)

**Sorun:** Sınıflardaki PC'ler ve sunucular aylar/yıllar boyunca güncellenmemiş olabilir. Bilinen zafiyetler açık.

**Yapılacak:** Tüm Windows cihazlarında Windows Update otomatik aç. Antivirüs imzalarının güncel olduğunu doğrula. Eski Windows 7/8 cihazları varsa Linux'a geç ya da kullanım dışı bırak.

**Süre:** 2-4 saat **Maliyet:** Sıfır

---

## 6. USB Bellek Politikası Oluşturun

**Sorun:** USB bellekler ransomware ve diğer kötü amaçlı yazılımların en yaygın okul ağına giriş yolu. Öğretmenler evde flash bellek kullanıyor, okula getirip takıyor.

**Yapılacak:** En basit kontrol: kritik cihazlarda (sunucu, idari PC) USB depolama cihazlarını grup politikası ile devre dışı bırak. Eğitim materyali transferi için bulut depolama (Google Drive, OneDrive, MEB EBA Dosya) kullan.

**Süre:** 1-2 saat **Maliyet:** Sıfır

---

## 7. Phishing Farkındalığı Personel Eğitimi (15 dakika)

**Sorun:** Okul saldırılarının çoğu phishing ile başlıyor. Personel "MEB güncelleme" konulu maille login bilgilerini paylaşıyor.

**Yapılacak:** Öğretmenler kuruluna 15 dakikalık bir oturum koy. Gerçek phishing örneklerini göster (URL kontrolü, kötü gramer, aciliyet baskısı). E-posta üzerinden hiçbir zaman şifre/kimlik bilgisi istenmeyeceğini vurgula.

**Süre:** Hazırlık 1 saat, sunum 15 dakika **Maliyet:** Sıfır

---

## 8. WiFi Şifresini Karmaşıklaştırın ve WPA3'e Geçin

**Sorun:** Çoğu okul "okul2023" tipi tahmin edilebilir WiFi şifreleri kullanıyor, WPA2 ile.

**Yapılacak:** WiFi şifresini en az 16 karakterli rastgele bir parolaya değiştir (kelime + sayı + sembol). WPA3 destekli bir modemse WPA3 moduna geç. Şifreyi öğretmen odasına asma — sadece personele bireysel olarak ilet.

**Süre:** 30 dakika **Maliyet:** Sıfır

---

## 9. Kritik Servislerin Hangi Cihazda Çalıştığını Belgelendirin

**Sorun:** "Şu yazıcı sunucusu nerede?" "DHCP nereden geliyor?" "DNS hangisinde?" — kimse bilmiyor. Cihaz arızalandığında panik.

**Yapılacak:** Kağıt veya Excel'de basit bir tablo: Servis adı, çalıştığı cihaz, fiziksel konum, sorumlu kişi, varsa lisans/şifre konumu. Bu tek tablo, devir teslimlerde hayat kurtarır.

**Süre:** 2-3 saat **Maliyet:** Sıfır

---

## 10. Müdür İçin Tek Sayfalık "Olay Olursa Ne Yapılır" Belgesi

**Sorun:** Ransomware vurursa, internet kesilirse, kamera sistemi hacklenirse — müdür ne yapacak?

**Yapılacak:** Tek sayfalık bir belge yaz:
- Olası olay tipleri (ransomware, veri sızıntısı, hesap ele geçirilmesi)
- Her biri için: kim aranır (sen, MEB BTSB, polis), neyi kapatmalı (internet, ağ), ne söylememeli (medyaya, sosyal medyaya)
- Bilgilendirilmesi gereken kişilerin telefonları

Müdürün masasına as. Yedeği BT sorumlusunda olsun.

**Süre:** 2-3 saat **Maliyet:** Sıfır

---

## Sonuç

Bu 10 maddenin tamamı bir hafta sonu yapılabilir, hiçbir bütçe gerektirmez ve okulun güvenlik seviyesini hissedilir biçimde artırır. Bu liste bir başlangıçtır; gerçek bir değerlendirme için `docs/00-metodoloji.md` dosyasına bakın.

## Lisans

Bu liste MIT lisansı altındadır. Atıf yapmanıza gerek yok; kullanın, paylaşın, kendi okulunuza uyarlayın.
