# Veri Seti Olusturma ve Modelleme
   Bu topladığımız veri setindeki amacımız tweetlerini aldığımız Twitter hesabının genellikle hangi konular üzerinde konuştuğunu belirleyebilmek ve bu konu başlıklarını grafiklere bölerek gösterebilmektir.

   Bu tabloyu oluşturabilmek için öncelikle veri almak istediği Twitter hesabından 2000 tane tweeti bir csv dosyasına kaydettik.Daha sonrasında konu başlığını tweet contentinden belirlemek istediğimiz için Content sütununu yeni bir csv dosyasına kaydettik. Bu sayede ihtiyacımız olmayan diğer sütunlardan(likecount,url,replycount,...) kurtulduk. Content sütununu csv dosyasına kaydettikten sonra veri setimizi temizlemek için "re" kütüphanesini kullanarak boşluklardan,urllerden,sayılardan ve çeşitli noktalama işaretlerinden arındırmış olduk.Sonrasında ise temizlemiş olduğumuz veri setini clean adındaki yeni bir sütuna kaydettik ve bu clean sütununu yeni bir csv dosyasına kaydettik.Böylelikle veri setimizi temizlemiş olduk.

   Temizlediğimiz veri setini sklearn kütüphanesini içinde bulunan Latent Dirichlet Allocation modellemesini kullanarak elde ettiğimiz verilerden 8 adet Topic oluşturduk.Bu Topiclere sırasıyla baktığımızda ise Topic 1'in ağırlıklı olarak kullandığı kelimelerden konusunun toplu açılış töreni ile ilgili olduğunu saptadık.
Topic 2'ye baktığımızda konu başlığının tarım ve spor alanında maddi destek ile alakalı olduğunu söyleyebiliriz.Aynı şekilde Topic 3; Ak partinin düzenlemiş olduğu toplantı ve buluşmalar, Topic 4; Kabine toplantısı sonrası millete sesleniş, Topic 5 ve Topic 6' da ise kelimelerin kullanım oranları birbirine çok yakın olduğu için net bir konu başlığı çıkaramıyoruz, Topic 7; Ak parti üyeleriyle İstanbul'da gerçekleştirilen genişletilmiş toplantı ve son konu başlığımız olan Topic 8' de ise konunun; Türkiye Cumhurbaşkanı'nın gerçekleştirdiği basın toplantısı ile ilgili olduğunu çıkarabiliyoruz.


![Topics](https://user-images.githubusercontent.com/78156402/210576658-b5c1c280-e84e-4ce2-b37c-755fcd8b5c74.jpg)





Öğrenci Adı : Mustafa Enes Saatçi - 193405054 ///
Öğrenci Adı : Gülnur Korkmaz - 203405046
