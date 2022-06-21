# Insertion Sort Projesi
www.patika.dev Veri yapıları ve algoritmalar bölümünün ilk projesi için oluşturulmuştur.

dizi = [22,27,16,2,18,6]
## 1.Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
Arama indexi (dizi zero-based olarak ele alındığında başlangıç elemanı 0 olacağından) 1'den başlayarak solunda kalan dizi elemanları ile küçük mü sorgulaması yapılır ve küçükse bulunulan indexteki değer solundaki değer ile yer değiştirir. Mevcut olarak sorgulanan değer solundaki değerden küçük olduğu sürece, İndex değeri her adımda 0 oluncaya kadar (yani en soldaki elemana gelinceye kadar) devam edecektir. Sorgulanan değer solundakinden büyük veya eşit olma durumunda ise son index değerinde duracaktır.

Sıralama aşamalarında dizinin değerleri:
```linux
[22, 27, 16, 2, 18, 6] #sıralama başlangıç indexi olan 1'deki 27 değeri 22'den küçük olmadığı için yer değiştirme olmaz ve sonraki adıma geçilir.
[16, 22, 27, 2, 18, 6] #16 değeri 27'den küçük olduğu için önce 1.index'e ardından 22'den küçük olduğu için 0.cı indexe kayacaktır.
[2, 16, 22, 27, 18, 6] #2 değeri kendinden önceki tüm değerlerden daha küçük olduğundan sırayla 0.indexe kadar kayacaktır.
[2, 16, 18, 22, 27, 6] #18 değeri 27 ve 22'den küçük olduğu için sırasıyla sola kayarak 2.indexte duracaktır.
[2, 6, 16, 18, 22, 27] #6 değeri 27, 27, 18 ve 16 değerlerinden küçük olduğu için sırasıyla sola kayarak 1.index'te yer bulacaktır.
```

## 2.Big-O gösterimini yazınız. 
not(Tr) : Big-O gösteriminde n harfi girdi sayısını (dizi eleman sayısı vb.) ve N harfi ise işlem sayısını ifade etmektedir.

not(En) : (O is the order of growth and n is the length of the input.)

```
Big-O notation : Quadratic time – O(n²)
```
## 3.Time Complexity: 
Average case: Aranan sayının ortada olması
Worst case  : Aranan sayının sonda olması 
Best case   : Aranan sayının dizinin en başında olması.

## 4.Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
[2, 6, 16, 18, 22, 27] #Sıralama sonrası 18 değeri dizinin ortasındaki eleman olduğu için "Average Case" kapsamında olacaktır.

## [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

```
[3, 7, 5, 8, 2, 9, 4, 15, 6]  # 2.sırada yer alan 3 değeri 7 ile karşılaştırılarak 1.sıraya kaydırılır.
[3, 5, 7, 8, 2, 9, 4, 15, 6]  # 3.sırada yer alan 5 değeri 7 ile karşılaştırılarak 2.sıraya kaydırılır.
[3, 5, 7, 8, 2, 9, 4, 15, 6]  # 4.sırada yer alan 8 değeri 7 ile karşılaştırılır, konumu değişmez ve 4.sırada kalır.
[2, 3, 5, 7, 8, 9, 4, 15, 6]  # 5.sırada yer alan 2 değeri sırasıyla 8, 7 , 5 ve 3 değerleriyle karşılaştırılır ve 1.sıraya taşınır.
```

## License
[MIT](https://choosealicense.com/licenses/mit/)
