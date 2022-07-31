# Merge Sort Projesi
## Proje 2

[16,21,11,8,12,22] -> Insertion Sort

---
1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
- İlk olarak dizi ikiye bölünür.<br />
[16,21,11] ----- [8,12,22]<br /><br />
- Elde edilen iki dizi de ikiye bölünür ve bu işleme dizilerde tek eleman kalana kadar devam edilir.<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[16] - [21,11] ----- [8] - [12,22]<br />
[16] - [21] - [11] ----- [8] - [12] - [22]<br /><br />
- En küçük parçaya kadar ayırdığımız dizi elemanları aynı şekilde sıralayarak yeniden birleştirilir.<br />
[16] - [11,21] ----- [8] - [12,22]<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[11,16,21] ----- [8,12,22]<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[8,11,12,16,21,22] 

---
1. Big-O gösterimini yazınız.<br />
- Big-O gösterimi:
$$O(n \ . \ log \ n)$$