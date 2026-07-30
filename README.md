# TeknoDükkan - E-Ticaret Veri tabanı Projesi

Merhaba! Bu depo (repository), veri tabanı dünyasına attığım ilk adımı ve SQL öğrenme serüvenimi temsil ediyor. 

Bu projede, bir e-ticaret platformunun arka planında çalışacak temel veri tabanı mimarisini sıfırdan tasarladım. Amacım, sadece kod yazmak değil, verilerin birbiriyle nasıl konuştuğunu ve şirket yöneticileri için nasıl anlamlı raporlara dönüştüğünü kavramaktı.

## Bu İlk Projemde Neler Öğrendim ve Uyguladım?
- **Mimari Kurulum:** `MUSTERILER`, `SIPARISLER` ve `URUNLER` olmak üzere 3 farklı tablo inşa ettim (`CREATE TABLE`).
- **Veri Güvenliği:** Hatalı veri girişini önlemek için `PRIMARY KEY` ve `NOT NULL` kısıtlamalarını uyguladım.
- **Veri Analizi:** Şirketin toplam cirosunu, sipariş adedini ve ortalama kazancını hesapladım (`SUM`, `COUNT`, `AVG`).
- **Gruplama:** VIP müşterileri tespit etmek için verileri grupladım (`GROUP BY`).
- **Veri Yönetimi:** Sistemdeki iptal kayıtları sildim ve fiyat güncellemeleri yaptım (`UPDATE`, `DELETE`).
- **Büyük Rapor (JOIN):** Dağınık haldeki 3 tabloyu birbirine bağlayarak "Hangi müşteri, hangi ürünü almış ve ne kadar ödemiş?" sorusunu cevaplayan ilişkisel final raporunu oluşturdum.

## Hedefim
İlk SQL projem olan bu çalışmayla veri tabanı mantığının temelini sağlam bir şekilde attığımı düşünüyorum. Yaklaşan staj sürecimde, bu temelin üzerine yeni teknolojiler eklemeyi ve gerçek dünya projelerinde deneyim kazanmayı hedefliyorum.
