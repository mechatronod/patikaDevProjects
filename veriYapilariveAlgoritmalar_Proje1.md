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


## 3.Time Complexity: 
Average case: Aradığımız sayının ortada olması
Worst case: Aradığımız sayının sonda olması 
Best case: Aradığımız sayının dizinin en başında olması.

## 4.Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
sadasdasdad

# [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.
sdadasdadasdadsa

## Installation

Öncelikle projeyi clonelayın. (Buraya sizin reponuzdan aldığınız link gelecek)

```bash
git clone https://github.com/cengizcmataraci/kodluyoruzilkrepo.git
```


## License
[MIT](https://choosealicense.com/licenses/mit/)
