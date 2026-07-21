# Türkiye'deki Üniversitelerin Dağılım Haritası
## Proje Hakkında 
Bu proje, Türkiye'deki üniversitelerin şehir bazındaki dağılımını interaktif bir harita üzerinde görselleştirmek amacıyla geliştirilmiştir.

Üniversite verileri analiz edilerek şehirlerde bulunan üniversite sayıları hesaplanmış ve sonuçlar interaktif bir Türkiye haritası üzerinde gösterilmiştir. Harita ilk açıldığında Türkiye'deki tüm üniversitelerin şehir bazındaki dağılımı görüntülenmektedir.

Harita üzerindeki şehirlerin üzerine gelindiğinde ilgili şehre ait üniversite sayısı, nüfus bilgisi ve 100.000 kişiye düşen üniversite oranı görüntülenmektedir.

Projede ayrıca üniversitelerin kuruluş yıllarına göre filtrelenebilmesini sağlayan bir Kuruluş Yılı filtresi bulunmaktadır. Kullanıcı belirli bir yıl girerek, o yıl ve öncesinde kurulmuş üniversitelerin şehir bazındaki dağılımını harita üzerinde görüntüleyebilmektedir.

## Projenin Amacı
- Türkiye'deki üniversitelerin şehir bazındaki dağılımını görselleştirmek.
- Her şehirde bulunan üniversite sayısını interaktif bir harita üzerinde göstermek.
- Şehirlerin nüfus bilgilerini ve 100.000 kişiye düşen üniversite oranını görüntülemek.
- Üniversiteleri kuruluş yıllarına göre filtreleyebilmek.
- Filtreleme sonucunda şehirlerdeki üniversite sayılarını dinamik olarak güncellemek.
- Seçilen yıl ve öncesinde kurulmuş üniversitelerin şehir bazındaki dağılımını incelemek.
- Seçilen şehirdeki üniversitelerin isimlerine ulaşılabilmesini sağlamak.
- Veri analizi ve harita görselleştirme tekniklerini uygulamak.

## Kullanılan Teknolojiler
- Python
- Google Colab
- Google Sheets
- Pandas
- NumPy
- Folium
- Branca
- HTML
- JavaScript
- GitHub Pages

## Proje Yapısı
```text
turkiyeuniversiteharitasi/
│
├── data/
│   ├── universiteverileri.csv
│   ├── turkiye-provinces.geojson
│   └── ilnufuslari.csv
│
├── src/
│   └── turkiyeuniversiteharitasi.ipynb
│
├── v1/
│   └── index.html
│
├── index.html
├── universities.html
├── README.md
├── requirements.txt
└── .gitignore
```
### Dosyaların Görevleri
- turkiyeuniversiteharitasi.ipynb: Verilerin okunması,analiz edilmesi ve haritanın oluşturulmasını sağlayan Python kodlarını içerir.
- universiteler.csv: Üniversite isimleri,şehirleri ve kuruluş yılları gibi üniversitelere ait verileri içerir.
- turkiye-provinces.geojson: Türkiye'nin il sınırları bulunmaktadır.
- index.html: Projenin ana interaktif haritasını içerir.
- universities.html: Haritada seçilen şehre ait üniversiteleri listeler.Seçilen kuruluş yılına göre filtreleme yapılmasını sağlar.
- requirements.txt: Projede kullanılan Python kütüphanelerinin listesi.
- .gitignore: Git tarafından takip edilmemesi gereken dosya ve klasörleri belirtir.
- ilnufuslari.csv: Şehirlerin nüfus bilgilerini içerir.

## Çalışma Mantığı
1. Üniversite verileri okunur.
2. Üniversitelerin şehir ve kuruluş yılı bilgileri analiz edilir.
3. Şehirlerde bulunan üniversite sayıları hesaplanır.
4. Şehir koordinatları üniversite verileriyle eşleştirilir.
5. Şehirlerin nüfus bilgileri kullanılarak 100.000 kişiye düşen üniversite oranları hesaplanır.
6. Folium kullanılarak interaktif Türkiye haritası oluşturulur.
7. Harita ilk açıldığında Türkiye'deki tüm üniversitelerin şehir bazındaki dağılımı gösterilir.
8. Şehirler, üniversite sayılarını temsil eden daire işaretçileri ile harita üzerinde gösterilir.
9. Dairelerin büyüklüğü şehirde bulunan üniversite sayısına göre belirlenir.
10. Dairelerin üzerine gelindiğinde ilgili şehrin üniversite sayısı, nüfusu ve 100.000 kişiye düşen üniversite oranı görüntülenir.
11. Kullanıcı, Kuruluş Yılı alanına bir yıl girerek üniversiteleri kuruluş yılına göre filtreleyebilir.
12. Filtrele butonuna tıklandığında, seçilen yıl ve öncesinde kurulmuş üniversitelere göre şehirlerdeki üniversite sayıları yeniden hesaplanır.
13. Filtreleme sonucunda haritadaki daireler güncellenir ve ilgili şehirlerdeki filtrelenmiş üniversite sayıları gösterilir.
14. Filtrelenmiş şehir dairelerine tıklanarak Üniversiteleri Gör bağlantısına ulaşılabilir.
15. Açılan yeni sayfada, seçilen şehirde bulunan ve seçilen yıla kadar kurulmuş üniversiteler listelenir.

## Nasıl Çalıştırılır?
1. Projeyi bilgisayarınıza indirin.
2. Gerekli Python kütüphanelerini yükleyin.
3. `src` klasöründeki `turkiyeuniversiteharitasi.py` Python dosyasını çalıştırın.
4. Python kodunun çalışması sonucunda `index.html` ve `universities.html` dosyaları oluşturulur veya güncellenir.
5. `index.html` ve `universities.html` dosyalarının aynı klasörde bulunduğundan emin olun.
6. `index.html` dosyasını bir web tarayıcısında açın.
7. Harita üzerinden şehirleri ve üniversite bilgilerini görüntüleyebilir, kuruluş yılına göre filtreleme yapabilir ve ilgili şehirdeki üniversiteleri `Üniversiteleri Gör` bağlantısı üzerinden listeleyebilirsiniz.
   
## Çıktı
Proje sonunda;
- Türkiye'nin interaktif üniversite dağılım haritası oluşturulur.
- Harita ilk açıldığında tüm üniversitelerin şehir bazındaki dağılımı görüntülenir.
- Şehirlerin üzerinde üniversite sayılarını temsil eden daireler gösterilir.
- Dairelerin üzerine gelindiğinde üniversite sayısı, nüfus ve 100.000 kişiye düşen üniversite oranı görüntülenir.
- Üniversiteler kuruluş yılına göre filtrelenebilir.
- Filtreleme sonucunda şehirlerdeki üniversite sayıları dinamik olarak güncellenir.
- Filtrelenmiş şehirlerdeki üniversitelerin isimlerine yeni bir sayfa üzerinden ulaşılabilir.

**Canlı Demo:**  
https://betulayvaz.github.io/turkiyeuniversitedagilimharitasi/
