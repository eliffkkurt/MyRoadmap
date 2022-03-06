
# Python

- Python Basics
- Data Types
- Args and Kwargs
- Object Oriented Programming in Python
- Decorators

## Python Basics

**1) Integers and Floats**

**2) String**

**3) Substring**

**4) print()**

  - *Özel Karakterler için Escape Sequence*
  - *Format Method ve F-string ile Print Etmek*
  
**5) Değer Atamak (Assigning Variable)**

**6) Veri Tipine Bakmak (Looking at types)**

**7) Veri Tipini Dönüştürmek (Type Casting - Type Conversion)**

**8) Yorum Yazmak (Writing Comment)**

**9) Build-in Functions**

  - *`.upper()`, `.lower()` fonksiyonlarıyla harfleri tamamen büyütüp tamamen küçültebiliyoruz.*
  - *`.capitalize()` ile ilk harfini büyütebiliyoruz. Birden fazla kelime varsa sadece ilk kelimenin ilk harfini büyütüyor.*
  - *`.title()` ile kelimelerin hepsinin ilk harfini büyütüyoruz.*
  - *`.replace("x","i")` harfleri değiştirebiliyoruz.*
  - *`.strip()` ile boşlukları, `.strip(*)` gibi ifadelerle istediğimiz ifadeleri stringden silebiliyoruz.*

**10) Ulaşılabilir Metodları Keşfetmek (Exploring Available Methods)**

**11) Alt çizgilerle Okuma (Underscore Placeholders)**

**12) Unpacking**

**Exercises**


## Data Types

**1) Lists**
- *Liste İçerisindeki Elemanlar*
- *Listede İndeksleme*
- *Listenin Değerlerini Değiştirme*
- *Liste İçin Kullanılan Fonksiyonlar*

  Ekleme
  - Listenin Sonuna Eleman Ekleme: `l.append(200)`
  - Spesifik İndekse Eleman Ekleme: `l.insert(3,100)`
  - İki Listeyi Birleştirme: `l + başka_liste` veya `l.extend([8,9])`

  Silme
  - İlk Oluşan Öğeyi Listeden Silme: `l.remove(40)`
  - Spesifik İndeksten Eleman Silme: `del l[1]`
  - Spesifik Bir İndeksten Eleman Silme ve Sildiği Elemanı Gösterme: `l.pop(4)`
  - Bütün Elemanları Silme: `l.clear()`

  Diğerleri
  - Listenin İçindeki Elemanın İndeksini Öğrenme: `l.index(30)`
  - Aynı Elemandan Kaç Tane Olduğunu Sayma: `l.count(44)`
  - Elemanları Tersten Yazma: `l.reverse()`  
  - Elemanları Sıralama: `l.sort()`
  - Listeyi Kopyalama: `l.copy()`



**2) Tuple**

- *Tuple İçerisindeki Elemanlar*
- *Tuple'da İndeksleme*

**3) Namedtuple**

**4) Dictionary**

- *Dictionary İçerisindeki Elemanlar*
- *Dictionary'nin Değerlerini Değiştirme*
- *Dictionary'de Ekleme ve Silme İşlemleri*

  - `d["key"]=value` ile ekleme işlemini gerçekleştiriyoruz.
  - `del d["key"]` ile silme işlemini gerçekleştiriyoruz.

**4) Set**

- *Set İçerisindeki Elemanlar*
- *Setler'de Ekleme ve Silme İşlemleri*

  - `s.add(6)` ile ekleme işlemini gerçekleştiriyoruz.
  - `s.discard(10)` ile veya `s.remove(10)` ile silme işlemini gerçekleştiriyoruz. `s.remove(10)` ilgili eleman set içerisinde yoksa hata dönerken `s.discard(10)` hata dönmez.

- *Setler'de Küme İşlemleri*


## Pandas

**1) Pandas Basics**
- **CSV Dosyası Okuma**

  `df = pd.read_csv("data/survey_results_public.csv")`

- **Dataframe'de İlk ve Son Satırlara Bakma**
  - `df.head()` 

  - `df.tail()`

- **Dataframe'deki Tüm Satır ve Sütunları Görüntüleme**

  - `pd.set_option("display.max_columns",df.shape[1])` ile tüm sütunları görebiliyoruz.

  - `pd.set_option("display.max_rows",schema_df.shape[0])` ile tüm satırları görebiliyoruz.

  - `pd.reset_option("display.max_columns")` ve `pd.reset_option("display.max_rows")` ile resetleme işlemi yapıyoruz.

**2) Dataframe - Series**

- **Dictionary'den Dataframe Oluşturmak**

    `df = pd.DataFrame(people)`
    
- **Dataframe'in Satır Belirtmeden Sütun Bilgisine Erişmek**

   *iloc*, *loc* belirtmeden iki parantezle satırların ilgili sütun bilgilerini getirmiş oluyoruz. 

  - `df[["name","last_name"]]` ile name ve last_name sütunundaki tüm satırların bilgisine dataframe olarak erişiyoruz.
    
- **Dataframe'in Satırlarına Erişmek**

  İlki satır, ikincisi sütun.

  *iloc*

  - `df.iloc[0]["name"]` ile 0. satırdaki name sütunundaki hücreyi 'Finley' şeklinde bilgi olarak alıyoruz.

  - `df.iloc[[0]]` ile 0. satırdaki tüm sütunları dataframe olarak alıyoruz.

  - `df.iloc[[0,1]]` ile 0 ve 1. satırdaki tüm sütunları dataframe olarak alıyoruz.

  - `df.iloc[0:3]` ile 0. satırdan başlayıp 2. satıra kadarki tüm sütun bilgilerini dataframe olarak alıyoruz.

  *loc*

  Indekslerin etiketlerine göre öğelere erişiyoruz.

  - `df.loc[[0,2]]` ile 0 ve 2 etiketli satırlarındaki tüm sütunları dataframe olarak alıyoruz.
  
- *Dataframe'in Belirli Satırlarında Belirli Sütunlarına Erişmek*

  **İlki satır ikincisi sütun**

  *iloc*

  - `df.iloc[[0,1],1]` ile 0 ve 1. satırdaki 1. sütundaki bilgileri series olarak (indeks bilgisiyle) alıyoruz. `df.iloc[[0,1],1][0]` şeklinde belirttiğimizde ise indeks bilgisi olmadan içeriği alabiliyoruz.


  - Sütunu indeksle belirtmek yerine `df.iloc[[0,1]]["last_name"]` şeklinde direkt adını yazarak da series olarak alabiliriz.


  - `df.iloc[[0,1],[0,2]]` şeklinde birden fazla sütun çekersek dataframe şeklinde almış oluruz.


  - Satır aralığı belirtmek istiyorsak satır tarafını parantezden kurtarıp aralığı `df.iloc[0:2,[0,2]]` şeklinde iki noktayla belirtiyoruz.


  - Sütun aralığı belirtmek istiyorsak sütun tarafını parantezden kurtarıyoruz, aralığı `df.iloc[[0,1],0:2]` şeklinde iki noktayla (:) belirtiyoruz.


  - İki indeks arasındaki tüm satırlara ve sütunlara erişmek istiyorsak `df.iloc[0:3,0:3]` şeklinde parantezden kurtarıyoruz iki tarafı da.

  *loc*

  Indekslerin etiketlerine göre öğelere erişiyoruz.

  - `df.loc[[0,2],0]` hata verir çünkü 0 olan bir sütun adı yok.

  - `df.loc[[0,2],"name"]` şeklinde sütun adı yazmak gerekir.

  iloc'tan farklı olarak; 

  - `df.loc[0:2, "name"]` ifadesinde 2. indeksteki satır da dataframe'e dahil edilir.

  - `df.loc[0:2, "name":"age"]` şeklinde sütunlar arasını kendi isimleriyle aralık vererek alabiliriz. Fakat `df.iloc[0:2, "name":"age"]` hata verecektir.


## Args and Kwargs

**1) Unpacking**

**2) Args**

**3) Kwargs**

**4) Using Args and Kwargs Together**

## Object Oriented Programming in Python

**Object Oriented Programming**
  - Objects
  - Class
  - Attributes
  - Methods
  - Inheritance
  - Polymorphism
  - Special Methods
  
 **Object Oriented Programming In Python**
 - Classes and Objects
  - Class Definition
  - Creating Objects (Instances) and How To Access Properties / Call Methods
  - Subclasses
  - Class Decorators And classmethod
  - classmethod vs. staticmethod
  - Getters / Setters / Deleters

## Decorators

**1) First Class Functions**
  - Functions as an Parameters
  - Returning Functions

**2) Closures**

**3) Decorators**
  - Class Decorators

**Exercises**
