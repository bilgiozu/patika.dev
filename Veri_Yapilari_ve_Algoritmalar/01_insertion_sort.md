# Insertion Sort Projesi
## Proje 1

[22,27,16,2,18,6] -> Insertion Sort

---
1. Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.<br />
- Burada dizinin ilk elemanı 22'dir. Dizi küçükten büyüğe doğru sıralanacağı için dizi içerisindeki en küçük eleman bulunarak ilk eleman ilk yer değiştirilir. Bu işlemden sonra dizi aşağıdaki şekle gelir.<br />
[2,27,16,22,18,6] -> İlk adımda 2 ve 22 elemanları yer değiştirdi.<br /><br />
- İkimci aşamada artık en küçük eleman olan ilk eleman sabit kalır ve dizi içerisinde sonraki küçük eleman ikinci eleman ile yer değiştirir.<br />
[2,6,16,22,18,27] -> İkinci aşamada 6 ve 27 elemanları yer değiştirdi.<br /><br />
- Üçüncü aşamada aynı şekilde 16'dan sonraki büyük eleman olan 18, 22 ile yer değiştirir.<br />
[2,6,16,18,22,27] -> Üçüncü aşamada 18 ile 22 elemanları yer değiştirdi.<br /><br />
- Bu şekilde dizinin tüm elemanları küçükten büyüğe tam olarak sıralanmış olduğundan işlem tamamlanmış olur.

---
2. Big-O gösterimini yazınız.<br />
- n elemanlı böyle bir dizide ilk adımda n tane değer kontrol edilir. En küçük eleman olan ilk eleman yerini aldıktan sonra da ikinci elemanın tespiti için kalan (n-1) eleman kontrol edilir. Aynı şekilde işlem tekrarlanarak en sondaki elemana kadar ilerler. Bu durumda tüm adımlarda toplamda;<br />
n + (n-1) + (n-2) + ... + 1 sayıda işlem gerçekleştirilmiş olur. 1'den n'e kadar olan sayıların toplam formülü;
$n.(n+1)\over2$ olduğundan $n^2+n\over2$ sonucu elde edilir. Çok büyük n değerleri için "$1\over2$" ve "n" değerleri ihmal edilebileceğinden Big - O gösterimi $n^2$ olarak ifade edilebilir.
$$O(n^2)$$

---
3. Time Complexity;<br />
   **Average case:** Aradığımız sayının ortada olması,<br />
   **Worst case:** Aradığımız sayının sonda olması,<br />
   **Best case:** Aradığımız sayının dizinin en başında olması.<br />
Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
- Dizi sıralandıktan sonra dizi içerisinde bulunduğu konumdan dolayı "18" elemanı **average case** kapsamına girer.
---
[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.<br />
1. Adım --> [**2**,3,5,8,**7**,9,4,15,6]<br />
2. Adım --> [2,3,**4**,8,7,9,**5**,15,6]<br />
3. Adım --> [2,3,4,**5**,7,9,**8**,15,6]<br />
4. Adım --> [2,3,4,5,**6**,9,8,15,**7**]