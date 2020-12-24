# git-undo-tryouts
Git undo tryouts


undo işlemlerinde önemli unsurlar
1. tag kullanımı
    - gün içerisinde birçok commit gönderiyoruz
    - bu commitleri hem yeni bir özellik eklediğimiz zaman   
        hem de bu özellikle ilgili yazdığımız kodu deploy edip sonucunu görebilmek için kullnıyoruz.
    - Bu durumda bir commit 2 amaçla kullanılmış oluyor. 
    - Bu da şöyle bir karışıklığa sebep olyuyor
    - bir özellik ne zaman yapılmaya başlandı ve bitti yani tamamlandığını belirten commit hangisi
    - tabii ki yeni özellik belirten özel bir ifade kullanılabilir ya da commit lerde na yazıldığına tek tek bakılabilir ama
        ama bunun yerine her özellik eklenirken TAG ları kullanmak çok daha mantıklı.
    - Tagları kullandığımız zaman ister kodun sonucunu deploy edip görelip isterse sadece gün sonıu commiti göndermiş olalım 
        uyguladığımız özelliğin bitip bitmediğini 
        hangi özelliklerin eklendiğini ne bir şekilde görebiliriz.
        bu aynı zamanda rapor çıkartırken de çok işe yarar 
        geçmiş stabil versiyonların neler olduğunu da netleştirir
        istediğimiz zaman eski bir commite dönemk istediğimizde de çok büyük rahatlık sağlar
        hangi commit stabil çalışıyor hangisi bug içeriyor net bir şekilde belli olur.
2. eski commite dönerken commit no yerine tag kullanılabilir
3. eski commite dönerken kullanılan araçlar
    - checkout commit-no
    - checkout tag-name
    - revert
    - reset
    
4. eski commite dönerken 
    - commitlerin push edilmiş olması veya olmaması nelere yol açıyor bu 3 yöntemde

5. Bunların haricinde 
    - sadece eski bir commite gidip bakmak tekrar son commit e dönmek isteyebilirim
    - geriye gidip geçmiş bir commiti head yapmak isteyebilirim
        - bu esnada arada kalan commt leri silmek isteyebilirim
        - bu esnada arada kalan commt leri silmemek isteyebilirim
    

