
# Python

- Python Basics
- Data Types
- Args and Kwargs

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
