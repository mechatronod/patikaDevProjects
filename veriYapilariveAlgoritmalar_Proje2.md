# Merge Sort Projesi

www.patika.dev Veri yapıları ve algoritmalar bölümünün ikinci projesi için oluşturulmuştur.

dizi = [16,21,11,8,12,22]
## 1.Yukarı verilen dizinin sort türüne göre (merge sort) aşamalarını yazınız.
örnek bir dizi için Wikipedia merge-sort animasyonu

![https://en.wikipedia.org/wiki/Sorting_algorithm](https://upload.wikimedia.org/wikipedia/commons/c/cc/Merge-sort-example-300px.gif)

dizi = [16,21,11,8,12,22] için aşamalar:

liste( veya dizi ) eleman sayısı 1 olana kadar iki parçaya ayrılır.
1 elemanlı diziler (sol ve sağ tarafta kalanlar) sırayla karşılaştırılarak en küçük sayı en sola gelecek biçimde tekrar birleştirilir.
Kodlamada en etkin yöntem rekürsif yapılı fonksiyon kullanmaktır.




Sıralama aşamalarında dizinin değerleri:
```linux
[16,21,11]            ---       [8,12,22]
[16,21]     -- [11]   ---       [8,12]      -- [22]
[16] - [21] -- [11]   ---       [8] - [12]  -- [22]
[16,21]     --[11]    ---       [8,12]      -- [22]
[11,16,21]            ---       [8,12,22]

[8,11]          ---> Sonraki karşılaştırmada kullanılacak diziler{ [16,21] [12,22] }
[8,11,12]       ---> Sonraki karşılaştırmada kullanılacak diziler{ [16,21] [22] }
[8,11,12,16]    ---> Sonraki karşılaştırmada kullanılacak diziler{ [21] [22] }
[8,11,12,16,21] ---> Sonraki karşılaştırmada kullanılacak diziler{ [22] }
[8,11,12,16,21,22]
```

## 2.Big-O gösterimini yazınız. 
not(Tr) : Big-O gösteriminde n harfi girdi sayısını (dizi eleman sayısı vb.) ve N harfi ise işlem sayısını ifade etmektedir.

not(En) : (O is the order of growth and n is the length of the input.)

```
Big-O notation : O(n*log(n))
```


## License
[MIT](https://choosealicense.com/licenses/mit/)
