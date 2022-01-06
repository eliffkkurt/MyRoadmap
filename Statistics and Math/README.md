
### Güven Aralıkları
**Örnek Problem:** Bir ürüne fiyat belirlemek istediğimizde bunu bir aralık olarak belirlemek için kullanabiliriz.



### Bernoulli Dağılımı 
İki sonuçlu bir olaylar ilgilendiğimizde kullanılır.

### Binom Dağılımı
İki sonuçlu olay n kez gerçekleştirildiğinde k kez başarılı olma olasılığı hesaplanacağı zaman kullanılır.

**Örnek Problem:**  Reklamı 100 kişi gördüğünde 1, 5 ya da 10 kişinin tıklaması olasılığı nedir? 

### Poisson Dağılımı
Nadiren gözlemlenen olayların olasılığı hesaplanacağı zaman kullanılıyor. Beklenen sonucun gerçekleşme olasılığının bilinmesi gerekiyor.

**Örnek Problem:** 
- Bir üniversitede 5000 not girişinde 5 tane notun yanlış girilmesi olasılığı nedir?
- 3 kez hatalı ilan girilmesi olasılığı nedir?

### Normal Dağılım
**Örnek Problem:** Dağılımın normal olduğu biliniyor. Aylık ortalama satış sayısı 80K, standart sapması 5K'ymış. 90K'dan fazla satış yapma olasılığı nedir?

### Tek Örneklem T Testi ve Nonparametrik Tek Örneklem Testi 

**Tanım:** Elimizdeki örneklemin ortalamasına ilişkin test yapma ihtiyacımız olduğunda kullanırız.

**Varsayım:** Normal dağılım.

*Tüm testlerde varsayım sağlanmazsa nonparametrik tek örneklem testi yapıyoruz.*

**Örnek Problem:** 
- Ürün satın alma adımlarının optimize edilmesi amacıyla 4. adımın gerçekten gözlemlendiği gibi ortalama 20 sn sürüp sürmediğinin test edilmesi.
- Web sitemizde geçirilen ortalama sürenin artırılması amacıyla geçirilen ortalama sürenin danışman şirketin iddia ettiği gibi 170 sn olup olmadığının test edilmesi.


### Tek Örneklem Oran Testi

**Tanım:** Sınamak istediğimiz değer oransal bir ifadeyse kullanırız.

**Varsayım:** Gözlem sayısının 30'dan büyük olması.

**Örnek Problem:** 500 kişi reklamlara tıklamış, 40'ı sitemize gelip alışveriş yapmış. 40/500 dönüşüm oranını ifade ediyor. Dönüşüm oranının yazılım tarafından belirtildiği gibi gerçekten 0.125 olup olmadığının test edilmesi.


### Bağımsız İki Örneklem T Testi (A/B Testi) ve Nonparametrik Bağımsız İki Örneklem T Testi
**Tanım:** İki grup ortalaması arasında karşılaştırma yapmak istediğimizde kullanırız. 

**Varsayım:** Normal dağılım ve varyans homojenliği.

**Örnek Problem:** Kullanıcılara ürün öneren bir makine öğrenmesi projesine yatırım yapılmış. Modelin ürettiği tahminler neticesinde oluşan gelir ile eski sistemin sağladığı gelirler arasında anlamlı bir fark olup olmadığının test edilmesi.
