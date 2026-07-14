# Türkiye'deki Üniversitelerin Dağılım Haritası
## Proje Hakkında 
Bu proje, Türkiye'deki üniversitelerin şehir bazındaki dağılımını interaktif bir harita üzerinde görselleştirmek amacıyla geliştirilmiştir.

CSV formatındaki üniversite verileri okunarak şehirlere göre gruplandırılmış, her şehirde bulunan üniversite sayısı hesaplanmış ve sonuçlar renk yoğunluğuna göre harita üzerinde gösterilmiştir.

## Projenin Amacı
- Türkiye'de her şehirde kaç üniversite bulunduğunu görselleştirmek.
- Üniversite dağılımını kolay anlaşılır bir harita üzerinde sunmak.
- Ham verileri analiz ederek anlamlı bir görselleştirme oluşturmak.
- Veri analizi ve harita görselleştirme tekniklerini uygulamak.

## Kullanılan Teknolojiler
- Python
- Google Colab
- Google Sheets
- Pandas
- NumPy
- Folium
- Branca

## Proje Yapısı
```text
turkiyeuniversiteharitasi/
│
├── data/
│   ├── universiteverileri.csv
│   └── turkiye-provinces.geojson
│   ├── ilnufuslari.csv
├── src/
│   └── turkiyeuniversiteharitasi.py
│
├── index.html
├── README.md
├── requirements.txt
└── .gitignore
```
### Dosyaların Görevleri
- truniversiteharitasi.py: Verilerin okunması,analiz edilmesi ve haritanın oluşturulması.
- universiteler.csv: Üniversite isimleri ve bulundukları şehir bilgisi.
- turkiye-provinces.geojson: Türkiye'nin il sınırları bulunmaktadır.
- index_with_boundaries.html: Oluşturulan interaktif harita.
- requirements.txt: Projede kullanılan Python kütüphanelerinin listesi.
- .gitignore: Git tarafından takip edilmemesi gereken dosya ve klasörleri belirtir. 

## Çalışma Mantığı
1. CSV dosyası okunur.
1. Üniversiteler şehir bilgilerine göre gruplanır.
2. Her şehirde bulunan üniversite sayısı hesaplanır.
3. Şehir koordinatları ile üniversite sayıları eşleştirilir.
4. Üniversite sayısına göre renk skalası oluşturulur
5. Folium kullanılarak interaktif Türkiye haritası hazırlanır.
6. Harita index.html olarak oluşturulur.

## Nasıl Çalıştırılır?
1. Bu repoyu bilgisayarınıza indirin.
2. Gerekli Python kütüphanelerini yükleyin.
3. `src` klasöründeki Python dosyasını çalıştırın.
4. Oluşturulan `index.html` dosyasını tarayıcıda açarak haritayı görüntüleyin.

## Çıktı
Proje sonunda;
- Türkiye haritası oluşturulur.
- Her şehir için üniversite sayısı görüntülenir.
- İşaretçilerin renkleri üniversite sayısına göre değişir.
- Fare ile şehir üzerine gelindiğinde üniversite sayısı görüntülenir.

**Canlı Demo:**  
https://betulayvaz.github.io/turkiyeuniversitedagilimharitasi/
