# NimbleShift – Veritabanı Yapısı

## 1. Genel Bakış

NimbleShift, işletme, personel, izin, vardiya ve planlama bilgilerini saklamak için Bubble'ın yerleşik veritabanını kullanır.

Veritabanı yedi ana veri türünden oluşmaktadır.

## 2. Ana Veri Türleri

### İşletmeler
İşletmelere ait temel bilgileri ve abonelikle ilgili verileri saklar.

### Kullanıcılar
Uygulama kullanıcılarına ait bilgileri ve kullanıcı rolüyle ilgili verileri saklar.

### Personel
Personel kayıtlarını ve personelin bağlı olduğu işletme bilgilerini saklar.

### İzinler
Personel izin taleplerini ve bu taleplerin onay durumlarını saklar.

### Vardiyalar
Planlanmış vardiyaları ve taslak vardiya önerilerini saklar.

### Kurallar
Vardiya planlama sürecinde kullanılan kuralları saklar.

### Personel İhtiyaçları
Vardiya önerileri oluşturulurken dikkate alınan personel ihtiyaçlarını saklar.

## 3. Seçenek Kümeleri (Option Sets)

Uygulamada şu anda dokuz seçenek kümesi kullanılmaktadır:

- Abonelik Paketi
- Görev Unvanı
- İzin Durumu
- İzin Kaydı
- İzin Türü
- Kullanıcı Rolü
- Müsaitlik
- Vardiya Durumu
- Çalışma Türü

## 4. Veri İlişkileri

Uygulamadaki operasyonel kayıtlar, ilgili işletmeyle ilişkilendirilecek şekilde tasarlanmıştır.

Personel, izin, vardiya, kural ve personel ihtiyaçları kayıtlarında işletme ilişkileri kullanılarak işletme bazlı veri ayrımı desteklenir.

## 5. Erişim Kontrolü

İşletme verilerine erişimi sınırlandırmak için Bubble Gizlilik Kuralları (Privacy Rules) ve iş akışı koşulları kullanılmaktadır.

Kullanıcılar yalnızca işletme ilişkileri ve kullanıcı rollerinin izin verdiği kayıtlara erişebilmelidir.

## 6. Veri Tutarlılığı

Vardiya onaylama, izin kararları ve personel yönetimi gibi önemli işlemlerde veri tutarlılığını korumak için iş akışı koşulları kullanılmaktadır.

## 7. Mevcut Kapsam

Bu belge bilinen veritabanı yapısını genel hatlarıyla açıklar.

Tüm alanların, veri ilişkilerinin ve gizlilik kurallarının ayrıntılı olarak doğrulandığı anlamına gelmez.
