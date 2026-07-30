#  TeknoDükkan - E-Ticaret Veritabanı Projesi

Merhaba! Bu depo (repository), veri tabanı dünyasına attığım ilk adımı ve SQL öğrenme serüvenimi temsil ediyor. 

Bu projede, bir e-ticaret platformunun arka planında çalışacak temel veritabanı mimarisini sıfırdan tasarladım. Amacım, sadece kod yazmak değil, verilerin birbiriyle nasıl konuştuğunu ve şirket yöneticileri için nasıl anlamlı raporlara dönüştüğünü kavramaktı.

##  Bu İlk Projemde Neler Öğrendim ve Uyguladım?
- **Mimari Kurulum:** `MUSTERILER`, `SIPARISLER` ve `URUNLER` olmak üzere 3 farklı tablo inşa ettim (`CREATE TABLE`).
- **Veri Güvenliği:** Hatalı veri girişini önlemek için `PRIMARY KEY` ve `NOT NULL` kısıtlamalarını uyguladım.
- **Veri Analizi:** Şirketin toplam cirosunu, sipariş adedini ve ortalama kazancını hesapladım (`SUM`, `COUNT`, `AVG`).
- **Gruplama:** Verileri belirli kriterlere göre grupladım (`GROUP BY`).
- **Veri Yönetimi:** Sistemdeki iptal kayıtları sildim ve fiyat güncellemeleri yaptım (`UPDATE`, `DELETE`).
- **Büyük Rapor (JOIN):** Dağınık haldeki 3 tabloyu birbirine bağlayarak ilişkisel final raporunu oluşturdum.

---

##  Veri Sözlüğü (Tablo Yapıları)
Projemde kurduğum 3 boyutlu mimarinin tablo detayları şu şekildedir:

###  Müşteriler Tablosu (MUSTERILER)
| Sütun Adı | Veri Tipi | Açıklama |
| :--- | :--- | :--- |
| MUSTERI_ID | Integer (PK) | Müşterinin benzersiz kimlik numarası |
| AD | Varchar(50) | Müşterinin Adı ve Soyadı |

###  Ürünler Tablosu (URUNLER)
| Sütun Adı | Veri Tipi | Açıklama |
| :--- | :--- | :--- |
| URUN_ID | Integer (PK) | Her ürünün benzersiz barkod numarası |
| URUN_ADI | Varchar(50) | Ürünün sistemdeki adı |
| FIYAT | Integer | Ürünün güncel satış fiyatı |

###  Siparişler Tablosu (SIPARISLER)
| Sütun Adı | Veri Tipi | Açıklama |
| :--- | :--- | :--- |
| SIPARIS_ID | Integer (PK) | Siparişin işlem numarası |
| MUSTERI_ID | Integer (FK) | Siparişi veren müşterinin ID'si (Köprü 1) |
| URUN_ID | Integer (FK) | Satın alınan ürünün ID'si (Köprü 2) |
| TUTAR | Integer | Ödenen toplam tutar |

---

##  Proje Çıktısı (Büyük Final Raporu)
Aşağıdaki tablo, `JOIN` komutu kullanılarak 3 farklı tablonun (Müşteriler, Siparişler ve Ürünler) birleştirilmesiyle elde edilen final raporunun ekran görüntüsüdür:



<img width="815" height="140" alt="Ekran görüntüsü 2026-07-30 141505" src="https://github.com/user-attachments/assets/10bda0c2-4792-4131-b683-954f3cee02fa" />


##  Hedefim
İlk SQL projem olan bu çalışmayla veri tabanı mantığının temelini sağlam bir şekilde attığımı düşünüyorum. Yaklaşan staj sürecimde, bu temelin üzerine yeni teknolojiler eklemeyi ve gerçek dünya projelerinde deneyim kazanmayı hedefliyorum.
