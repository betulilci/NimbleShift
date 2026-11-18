# NimbleShift – Güvenlik

## 1. Genel Bakış

NimbleShift, uygulama verilerini korumak için Bubble'ın yerleşik kimlik doğrulama sistemini, gizlilik kurallarını ve iş akışı koşullarını kullanır.

Güvenlik yaklaşımı, işletme sahipliği ve kullanıcı rolleri temelinde tasarlanmıştır.

## 2. Kullanıcı Kimlik Doğrulama

Uygulamada Bubble kullanıcı kimlik doğrulama sistemi kullanılmaktadır.

Yapılandırılmış parola politikası şu koşulları içerir:

- En az 8 karakter
- En az bir rakam
- En az bir büyük harf
- En az bir özel karakter

## 3. Kullanıcı Rolleri

NimbleShift üç temel kullanıcı rolüne sahiptir:

- Yönetici
- Planlayıcı
- Personel

Uygulama özelliklerine erişim, kullanıcının rolüne göre sınırlandırılmaktadır.

## 4. İşletme Bazlı Veri Güvenliği

İşletmeyle ilişkili kayıtların yalnızca aynı işletmeye bağlı yetkili kullanıcılar tarafından erişilebilir olması hedeflenmektedir.

Veri erişimini sınırlandırmak için Bubble Gizlilik Kuralları kullanılmaktadır.

## 5. İş Akışı Düzeyinde Güvenlik

Önemli işlemlerde ek güvenlik kontrolleri uygulanmaktadır.

Bunlar arasında:

- Vardiya oluşturma ve onaylama
- Vardiya iptali ve değişimi
- İzin onaylama ve reddetme
- Personel yönetimi
- Abonelik paketi limitleri

yer almaktadır.

## 6. Davet Kodu Güvenliği

İşletme davet kodları hassas bilgi olarak değerlendirilmektedir.

Yetkisiz kullanıcıların bu kodları arama yoluyla keşfetme riskini azaltmak amacıyla erişim kısıtlamaları uygulanmıştır.

## 7. Doğrulanması Gereken Güvenlik Alanları

Uygulamanın genel kullanıma açılmasından önce aşağıdaki alanların ayrıca incelenmesi gerekmektedir:

- İşletmeler arası veri izolasyonu
- Alan düzeyindeki gizlilik ve arama izinleri
- Dosya ve ek erişim izinleri
- Davet koduyla işletmeye katılma süreci
- Arka plan iş akışlarının kimlik doğrulaması
- Stripe webhook güvenliği
- Tüm sayfa ve iş akışlarında rol bazlı erişim

## 8. Ödeme Güvenliği

Uygulamada Stripe entegrasyonu bulunmaktadır. Ancak ödeme işlemleri ve webhook davranışları henüz tam olarak doğrulanmamıştır.

Ödeme sistemi, uygun ücretli Bubble ortamında gerekli kontroller tamamlanmadan gerçek kullanıma hazır kabul edilmemelidir.

## 9. Güvenlik Durumu

Geliştirme sürecinde çeşitli güvenlik iyileştirmeleri uygulanmıştır.

Ancak bu belge tamamlanmış bir güvenlik denetimi anlamına gelmez ve uygulamanın tüm güvenlik gereksinimlerini karşıladığını garanti etmez.

Genel kullanıma açılmadan önce kapsamlı bir güvenlik incelemesi yapılmalıdır.
