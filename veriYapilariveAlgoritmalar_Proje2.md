# Merge Sort Projesi

www.patika.dev Veri yapıları ve algoritmalar bölümünün ikinci projesi için oluşturulmuştur.

dizi = [16,21,11,8,12,22]
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
Big-O notation : O(n*log(n))
```


## License
[MIT](https://choosealicense.com/licenses/mit/)
