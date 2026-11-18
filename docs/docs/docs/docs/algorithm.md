# NimbleShift – Akıllı Vardiya Planlama Algoritması

## 1. Genel Bakış

NimbleShift, işletmelerin personel ihtiyaçlarına ve personel uygunluklarına göre vardiya önerileri oluşturmasına yardımcı olan akıllı vardiya planlama özelliğine sahiptir.

Planlama mantığı Bubble İş Akışları (Workflows) kullanılarak uygulanmıştır.

## 2. Planlama Süreci

Mevcut planlama süreci şu adımlardan oluşur:

1. Yönetici personel ihtiyaçlarını tanımlar.
2. Akıllı planlama iş akışı başlatılır.
3. Sistem uygun personelleri değerlendirir.
4. Uygun personeller vardiya önerileri için seçilir.
5. Öneriler taslak vardiya olarak kaydedilir.
6. Yönetici oluşturulan önerileri inceler.
7. Yönetici önerileri yeniden oluşturabilir veya silebilir.
8. Onaylanan öneriler gerçek vardiyalara dönüştürülür.

## 3. Taslak Vardiya Yönetimi

Uygulama, Vardiyalar veri türündeki `onerilen` alanını kullanarak taslak öneriler ile gerçek vardiyaları birbirinden ayırır.

- `onerilen = yes`: Kayıt bir taslak vardiya önerisidir.
- `onerilen = no`: Kayıt gerçek bir vardiyadır.

Bu yapı, önerilerin gerçek vardiya planına dahil edilmeden önce yönetici tarafından incelenmesini sağlar.

## 4. Personel Seçimi

Mevcut seçim mekanizması, uygun personeller arasından rastgele seçim yapar.

İlgili hafta içerisinde henüz vardiyası bulunmayan personele öncelik verilir.

Vardiyası bulunmayan personeller önceliklendirildikten sonra kalan uygun personeller arasından rastgele seçim yapılır.

## 5. Önerileri Yeniden Oluşturma

Yönetici, henüz onaylanmamış taslak vardiya önerilerini yeniden oluşturabilir.

Yeniden oluşturma sürecinde ilgili eski taslakların temizlenmesi hedeflenir. Böylece yeni önerilerle eski önerilerin birlikte kalması önlenir.

## 6. Vardiya Onaylama

Yönetici bir öneriyi onayladığında uygulama gerekli koşulları kontrol eder ve taslak kaydı planlanmış vardiyaya dönüştürür.

Onay iş akışı, aynı önerinin birden fazla kez onaylanmasını önleyecek şekilde düzenlenmiştir.

## 7. Mevcut Sınırlamalar

Mevcut algoritma tam kapsamlı bir matematiksel optimizasyon sistemi değildir.

Vardiyaların tüm personel arasında matematiksel olarak en dengeli biçimde dağıtılmasını garanti etmez.

Gelecekte gelişmiş optimizasyon, adalet puanlaması ve iş yükü dengeleme özellikleri eklenebilir.

## 8. Kullanılan Teknolojiler

Planlama mantığında şu Bubble özellikleri kullanılmaktadır:

- Bubble Database
- Bubble Backend Workflows
- Bubble İş Akışı Koşulları
- Personel uygunluk kontrolleri
- Rastgele personel seçimi

Şu anda harici bir Python veya SQL optimizasyon servisi kullanılmamaktadır.

## 9. Mevcut Durum

Bu belge mevcut planlama yaklaşımını ve bilinen sınırlamaları açıklar. Algoritmanın tüm senaryolarda doğru çalıştığı henüz doğrulanmış değildir.
