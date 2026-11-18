# NimbleShift – Test Senaryoları

## 1. Genel Bakış

Bu belge, NimbleShift uygulamasının temel özellikleri için hazırlanmış test senaryolarını içerir.

**Önemli:** Aşağıdaki senaryolar dokümantasyon amacıyla hazırlanmıştır. Henüz tamamının uygulama üzerinde çalıştırıldığı veya başarılı olduğu doğrulanmamıştır.

## 2. Kullanıcı Girişi ve Yetkilendirme

| No | Senaryo | Beklenen Sonuç |
|---|---|---|
| 1 | Kayıtlı kullanıcı giriş yapar. | Kullanıcı hesabına erişir. |
| 2 | Hatalı giriş bilgileri girilir. | Giriş işlemi başarısız olur. |
| 3 | Oturum açmamış kullanıcı korumalı bir sayfaya erişmeye çalışır. | Kullanıcı giriş sayfasına yönlendirilir. |
| 4 | Kullanıcı kendi rolüne ait olmayan bir işlemi yapmaya çalışır. | Yetkisiz işlem engellenir. |

## 3. İşletme ve Personel Yönetimi

| No | Senaryo | Beklenen Sonuç |
|---|---|---|
| 5 | Yönetici personel ekler. | Personel kaydı oluşturulur. |
| 6 | Yönetici personel bilgilerini düzenler. | Değişiklikler kaydedilir. |
| 7 | Personel başka bir işletmenin kayıtlarına erişmeye çalışır. | Erişim engellenir. |
| 8 | Abonelik personel limitine ulaşır. | Yeni personel ekleme işlemi sınırlandırılır. |

## 4. İzin Yönetimi

| No | Senaryo | Beklenen Sonuç |
|---|---|---|
| 9 | Personel izin talebi oluşturur. | Talep beklemede durumunda kaydedilir. |
| 10 | Yönetici izin talebini onaylar. | Talep onaylandı durumuna geçer. |
| 11 | Yönetici izin talebini reddeder. | Talep reddedildi durumuna geçer. |
| 12 | Yetkili kullanıcı kararı geri alır. | Talep yeniden beklemede durumuna geçer. |
| 13 | Yetkisiz kullanıcı izin kararını değiştirmeye çalışır. | İşlem engellenir. |

## 5. Vardiya Yönetimi

| No | Senaryo | Beklenen Sonuç |
|---|---|---|
| 14 | Yetkili kullanıcı vardiya oluşturur. | Vardiya kaydedilir. |
| 15 | Personel kendi vardiyalarını görüntüler. | Yalnızca erişmesine izin verilen vardiyalar gösterilir. |
| 16 | Personel başka bir personele ait vardiyayı görüntülemeye çalışır. | Yetkisiz erişim engellenir. |
| 17 | İptal edilmiş vardiya üzerinde işlem yapılmaya çalışılır. | Uygun olmayan işlem engellenir. |

## 6. Akıllı Vardiya Planlama

| No | Senaryo | Beklenen Sonuç |
|---|---|---|
| 18 | Yönetici akıllı planlamayı başlatır. | Sistem vardiya önerileri oluşturur. |
| 19 | Personel uygunluk koşullarını karşılamaz. | Personel öneriye dahil edilmez. |
| 20 | Yönetici önerileri yeniden oluşturur. | Eski taslakların yerine yeni öneriler oluşturulur. |
| 21 | Yönetici bir öneriyi onaylar. | Öneri gerçek vardiyaya dönüştürülür. |
| 22 | Aynı öneri ikinci kez onaylanmaya çalışılır. | Yinelenen onay engellenir. |
| 23 | Yönetici taslak öneriyi siler. | İlgili taslak kaldırılır. |

## 7. Güvenlik ve Veri Erişimi

| No | Senaryo | Beklenen Sonuç |
|---|---|---|
| 24 | Kullanıcı başka bir işletmenin verilerini arar. | Diğer işletmenin verilerine erişemez. |
| 25 | Personel yönetici yetkisi gerektiren bir işlem yapmaya çalışır. | İşlem engellenir. |
| 26 | Kullanıcı davet koduyla işletmeye katılmaya çalışır. | Yalnızca geçerli koşulları sağlayan kullanıcı katılabilir. |
| 27 | Kullanıcı korumalı verilere yetkisiz erişmeye çalışır. | Gizlilik kuralları erişimi engeller. |

## 8. Abonelik ve Ödeme

| No | Senaryo | Beklenen Sonuç |
|---|---|---|
| 28 | Kullanıcı abonelik paketini görüntüler. | Paket bilgileri gösterilir. |
| 29 | Kullanıcı paket limitini aşan işlem yapar. | İşlem paket koşullarına göre sınırlandırılır. |
| 30 | Ödeme işlemi başlatılır. | Ödeme entegrasyonu doğrulanmadan başarılı kabul edilmez. |

## 9. Test Durumu

Bu senaryolar test planı niteliğindedir.

Her senaryo uygulama üzerinde çalıştırıldığında sonucu ayrıca kaydedilmelidir:

- Başarılı
- Başarısız
- Henüz test edilmedi

Gerçek test sonuçları alınmadan uygulamanın tüm senaryolarda hatasız çalıştığı varsayılmamalıdır.
