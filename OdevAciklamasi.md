Dizi: [22,27,16,2,18,6] 

1. Yukarıda verilen dizinin Insertion Sort türüne göre aşamalarını yazınız. 

1.Aşama: En baştan başlayarak en küçük olan değere bakarız. 
22 evet küçük ama devam. 
27 büyük devam.
16 küçük ama hala eleman var devam.
2 küçük. Bunu tut. 
18 ve 6, 2'den büyük. 
O zaman ilk aşamada en baştaki 22 elemanı ile 2'nin yerlerini değiştiririz. Birinci aşamanın sonunda dizimizin yeni hali şöyle olur;
[2,27,16,22,18,6]

2.Aşama: 2'yi yerleştirdik. Sıra 27'ye bakarak arama yapmakta. 
16 küçük ama devam. 
22 küçük devam. 
18 küçük ama hala eleman var aramaya devam. 
6, gezdiğimiz elemanlar arasında en küçüğü. O zaman 27 ile 6'nın yerlerini değiştiririz. 
İkinci aşama sonunda dizimizin yeni hali şöyle olur;
[2,6,16,22,18,27]

3.Aşama: 16 için bakıyoruz. Daha küçüğünü bulursak yerinden ediyoruz. 
22, 16'dan büyük. Devam.
18, bu da büyük. 
27, 16'dan baya büyük. O zaman 16'dan daha küçük bir sayı olmadığı için dizide herhangi bir değişiklik olmayacak. 
Üçüncü aşama sonunda dizimizin yeni hali;
[2,6,16,22,18,27]

4.Aşama: Dizinin geri kalanında 22'den küçük sayı arıyoruz. 
18 küçük. Ama bir eleman daha var. 
27, 22'den büyük. O zaman 18, 22'nin yerini aldı. 
Dördüncü aşama sonucunda dizinin hali; 
[2,6,16,18,22,27]

5.Aşama: 22'den sonra 27 geldiği ve o da 22'den büyük olduğu için herhangi bir değişiklik yapmıyoruz. Yani dizimiz son haline ulaşmış oluyor. 


2.Big-O gösterimini yazınız. 
Insertion sort'da her eleman içerisinde arama yaptığımız için ve aramalar ilerledikçe birer değer azaldığı için n+ (n-1)+ (n-2)+...+1 mantığından n2+n/2 bizim time complexitymiz olur. Domine eden fonksiyon n2'dir. O halde;
O(n2) olur. 

3.
Average Case: O(n2)
Best Case: O(n)
Worst Case: O(n2)

4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? 
Dizi sıralandıktan sonra 18'i sıralamaya göre bulabiliriz. Yani 18 en başta olmadığı için Best Case'e girmez. Ancak en sonda olmadığı için Worst Case olarak da değerlendirilemez. 18'in Average Case kapsamına girdiğini söyleyebilirim. 


[7,3,5,8,2,9,4,15,6] için Insertion Sort'a göre ilk 4 adım; 

1.Adım: 7'ye bakıyoruz ve dizinin geri kalanında 7'den küçük bir değer arıyoruz. 
3: 7'den küçük ama hala eleman var. Devam. 
5: Küçük ama elemanlar var ve daha küçük olanı bulma ihtimali devam ediyor. 
8: 7'den küçük değil. Şimdiye kadar en iyi seçenek 3'tü ama devam ediyoruz.
2: 7'den küçük. Ve en iyi ihtimal olan 3'ten de küçük. İhtimal var devam.
9: 7'den büyük. 
4: 7'den küçük ama elimizdeki en iyi ihtimal olan 2'den büyük. Devam.
15: 7'den büyük. Eledik. 
6: 7'den küçük. Ama en iyi ihtimal olan 2'den büyük. O nedenle 7 ile 2 yer değiştirmelidir. 
Dizinin yeni hali: [2,3,5,8,7,9,4,15,6] olur. 

2.Adım: 3 için arama yapıyoruz. Listenin devamındaki değerlerin tümünü gezdiğimizde 3'ten büyük olduğunu gördük. Bu nedenle 3 ile herhangi bir sayı yer değiştirmez. 2.adım sonunda da dizi 1.adımdaki gibi kalır. 

3.Adım: 5 için aramadayız. 
8: 5'ten büyük. Devam.
7: 5'ten büyük. 
9: Hala 5'ten büyük. 
4: 5'ten küçük. Ayrıca 3 zaten sırada olduğu için 5'ten küçük olan ve şartları sağlayabilen başka bir eleman olamaz. Bu nedenle 4 ve 5 bu aşamada yer değiştirir. 
Dizinin yeni hali: [2,3,4,8,7,9,5,15,6] olur.

4.Adım: İlk 3 elemanı en küçük olacak şekilde yerleştirdik. Şimdi sırada 8 var. 
7: 8'den küçük ama ihtimaller devam ediyor. 
9: 8'den büyük. 
5: 8'den küçük ve 5'ten küçük olan diğer tüm değerler zaten sıralandığı için dizinin geri kalanında istediğimiz şartları sağlayan başka eleman bulamayız. O halde 8 ve 5 yer değiştiriyor diyebiliriz. 
Yani 4.adımın sonunda dizinin yeni hali: [2,3,4,5,7,9,8,15,6] olur. 


