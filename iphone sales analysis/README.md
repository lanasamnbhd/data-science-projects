-TR-

Bu proje, ham bir e-ticaret sipariş dosyasını alıp, veri bilimi araçlarını (Pandas, Matplotlib) kullanarak anlamlı hale (business insights) dönüştürme sürecidir.
Proje; veriyi temizleme, doğru veri tiplerine dönüştürme (özellikle zaman verisi) ve veriyi parçalara ayırarak (saatlik analiz) müşteri davranışlarını modeller.
Sonuç olarak, işletme sahibine "Müşteriler en çok hangi saatlerde alışveriş yapıyor?" sorusunun cevabını vererek pazarlama veya stok stratejilerini buna göre belirlemesine yardımcı olur.
1. Adım: kütüphanelerin yüklenmesi (import)
   Pandas, NumPy ve Matplotlib kütüphaneleri çağrılır.
   Pandas: veriyi tablo halinde tutmak ve işlemek için,
   Numpy: sayısal işlemler için,
   Matplotlib: veriyi grafiklere dökmek için kullanılır.
2. Adım: veri setinin yüklenmesi
   Bilgisayardaki ham veri dosyası Python'un anlayacağı bir formata çevrilir.
3. Adım: veri ön işleme
   "Transaction Date" sütunu __pd.to_datetime()__ fonksiyonu ile tarih formatına çevrilir.
4. Adım: feature extreaction
   Tarih sütunundan __"Hour"__ bilgisi ayrıştırılarak yeni bir sütun oluşturulur.
   Böylece, "Günün hangi saatlerinde satışlar artıyor?" sorusu cevaplanır.
5. Adım: veri analizi ve sayma
   Hangi saatte kaç adet sipariş olduğunu saymak için yapılır.
6. Adım: görselleştirme
   __plt.plot()__ fonksiyonu kullanılarak grafik çizilir. Başlıklar ve eksen isimleri eklenir.
   Bu sayede, okunması zor olan sayısal tablolar görselleştirilerek hangi saatte satışların zirve yaptığı hakkında anında fikir sahibi olabiliriz.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

-ENG-

This project demonstrates the process of transforming a raw e-commerce order file into actionable business insights using data science tools (Pandas, Matplotlib). 
The workflow involves data cleaning, type conversion (specifically for time-series data), and granular segmentation (hourly analysis) to model customer behavior.
Ultimately, it helps business owners answer the critical question: "At what times do customers shop the most?" enabling them to optimize marketing or inventory strategies accordingly.
Step 1: library import 
  Importing Pandas, NumPy, and Matplotlib.
  Pandas: For data manipulation and DataFrame management.
  NumPy: For numerical operations.
  Matplotlib: For data visualization.
Step 2: loading the dataset
  Loading the raw data file from the local drive and converting it into a format readable by Python.
Step 3: data preprocessing 
  The "Transaction Date" column is converted into a proper datetime format using the pd.to_datetime() function.
Step 4: feature extraction 
  The "Hour" information is extracted from the date column to create a new feature. This allows us to address the question, "At what time of day do sales increase?"
Step 5: data analysis and counting 
  Aggregating the data to count the number of orders that occurred during each specific hour.
Step 6: visualization 
  A graph is generated using the plt.plot() function, complete with titles and axis labels. This visualizes otherwise difficult-to-read numerical tables, providing instant insight into when sales peak.
   
