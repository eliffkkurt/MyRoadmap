# **Udemy - (50 Saat) Python A-Z™: Veri Bilimi ve Machine Learning**

6. Bölüm - Keşifçi Veri Analizi ve Veri Görselleştirme - Vahit Keskin anlattı. 

## Özet

Verinin kategorik ve sayısal değişken olmasına göre istatistiksel olarak gözden geçirildi ve grafiklerle görselleştirildi. Bu işlemler için seaborn'ün planets, diamonds, tips, iris, flights, fmri veri setleri kullanıldı.

Aşağıdaki grafik türlerine baktık: 

* Dağılım Grafikleri (Barplot-kategorik, Histogram-sayısal, Boxplot-sayısal, Violin-sayısal) 
* Korelasyon Grafikleri (Scatterplot-iki sayısal, Linear-iki sayısal, Scatterplot Matrisi-çoklu sayısal)
* Heatmap (Zaman serisi, Çok sınıflı kategori) 
* Çizgi Grafik (lineplot-time point,nesnelerin interneti)
* Basit Zaman Serisi

## Önemli Kodlar

- `df["method"]= pd.Categorical(df["method"])` yöntemiyle **object** tipinde olan değişkeni **category**ye dönüştürdük.

- `df.describe()` metoduyla veri setini istatistiksel olarak betimledik. median, mean, min, max, count değerlerini aldık. (Sadece nümerik değişkenlerin bu bilgilerini alıyoruz)

- Bize sayısal olarak verilen bazı değişkenleri **category**e dönüştürmemiz gerekebilir. (Örn. cinsiyet 1-0 olarak ifade edilmiş olabilir.)

- `df["year"] = pd.DatetimeIndex(df["year"])` metoduyla sayısal değişkeni (int, float) **datetime**'a çevirmemiz gerekir. 

- Verilerde eksik değişken olup olmadığını var olması durumunda onu doldurma yöntemlerini gördük.

- `df.select_dtypes(include = ["float64", "int64"])` koduyla istediğimiz veri tipindeki değişkenleri listeleyebiliyoruz.

- `df["method"].value_counts()` sütun içerisindeki kategorik sınıflardan her birinden kaçar tane olduğu bilgisini veriyor.

- `df["method"].value_counts().count()` sütun içerisinde kaç farklı kategorik sınıf olduğu bilgisini veriyor.

- `df["method"].unique()` koduyla sütun içerisindeki her farklı değişkenin isimlerinin listesini alıyoruz. 

- `df.pivot("month", "year", "passengers")` kodu zaman serilerinde (satırda ay, sütunda yıl, kesişimlerinde passengers olacak şekilde) tabloyu yeniden düzenlememizi sağlıyor.

- `from pandas.api.types import CategoricalDtype` `df["cut"] = df["cut"].astype(CategoricalDtype(ordered = True))` kodlarıyla nominal olan kategorik değişkeni ordinal hale çevirdik. Değişkenlerin arasında [Fair < Good < Very Good < Premium < Ideal] şeklinde bir ilişki olduğunu programa anlatabilmek için. Eğer sıralamayı istediğimiz gibi yapmazsa `category = ...(sıralamanın old. liste)` argümanını da eklememiz gerekir.
