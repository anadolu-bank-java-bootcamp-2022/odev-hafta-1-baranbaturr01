# Decomposition

## Decomposition Nedir?
- Bir problemi daha küçük alt problemlere ayırma sürecidir
- Başka bir söylem ile de bir sınıfın çok fazla özelliği varsa, bunların birleştirilmesi veya bölünmesi gibi bir işlemi yapmaktır.

## Decomposition Amacı Nedir(Neden)?
- Decomposition amacı, sistemdeki complexity(karmaşıklık) ile başa çıkmaktır. Buna kısaca divide and conquer denir.

## Fonksiyonel Decomposition 

- Büyük ve karmaşık fonksiyonlar Decomposition ile bölünmelidir.Bu olaya functional decomposition denir.

## Decomposition Avantajları Nelerdir?

- Reuseable code
- Easy to understand
- Easy to extend
- Easy to test
- Easy to debug

## Decomposition Nasıl Çalışır? 

- Mesela bir tane hesaplama yapan programa ihtiyacımız var ancak sadece 2 tane sayı alan bir fonksiyonumuz var.Ve biz 3 ve ya 4 tane sayı alan bir fonksiyon da yazmak istiyoruz.
- Bu durumda bizim ihtiyacımızın çok fazla sayı alan bir fonksiyonunu yazmak istiyoruz.
- Biz tek fonksiyon iççerisinde parametrelerin default değerlerini kontrol ede ede bu işlemi yapabiliriz aslında .Yani ;
 - Üçüncü  parametre yok ise iki parametreli işlem yapmak istiyor diyebiliriz .Bu işlemlerin hepsini tek bir foksiyondan yönetmek ciddi bir karmaşıklıga yol açar 
 - Bunun yerine bir adet base class oluşturup içerisine işlem fonksiyonlarını tanımlayıp ,başka sınıfları burdan extend almasını sağlayarak methodları override edebiliriz.
 - Bu sayede daha fazla bölüp daha kolay testler edebiliriz.

 ! [](/assets/decomposition.jpg)
 
 - yukarıdaki görsel araştırmalarım sonucunda elde ettiğim güzel ve açıklayıcı bir görseldir .Onuda paylaşmak istedim.Güzel bir proje işleyiş görselidir.Decomposition mantıgı ile oluşturulmuştur.
