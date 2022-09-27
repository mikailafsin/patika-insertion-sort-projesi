# Insertion Sort Projesi

Merhaba, [Patika](https://www.patika.dev)'nın [Veri Yapıları Ve Algoritmalar](https://app.patika.dev/courses/veri-yapilari-ve-algoritmalar) eğitimi kapsamındaki 1. Projesini tamamladım.

## [22,27,16,2,18,6] -> Insertion Sort

**1. Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.**

***Cevap***

1. [16,22,27,2,18,6]
2. [2,16,22,27,18,6]
3. [2,16,18,22,27,6]
4. [2,6,16,18,22,27]

---

**2. Big-O gösterimini yazınız.**

***Cevap***

= (n-1) + (n-2) + (n-3) + .... + 1
= ( n * (n-1) ) / 2
= ( n^2 - n ) / 2
= n^2 - n
= n^2

=> **O(n^2)**

---

**3. Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.**

***Cevap***

* Dizimizin küçükten büyüğe doğru sıralı olduğunu varsayarsak bu durumu Best Case senaryosu olarak ele alabiliriz. Dizimizin her elemanını karşılaştırırken her adımda sadece 1 karşılaştırma yapacağımız ve ilk elemanımızı karşılaştırmaya dahil etmeyeceğimiz için zaman karmaşıklığının sonucu olarak n-1 sonucuna ulaşmış oluruz. Bunu Big O notasyonu şeklinde gösterecek olursak da O(n) sonucuna varırız.
* Average Case = O(n^2)
* Dizimizin büyükten küçüğe doğru sıralı olduğunu varsayarsak bu durumu Worst Case senaryosu olarak ele alabiliriz. Bu durumda dizimizin eleman sayısını n olarak düşünürsek her elemanı doğru yere yerleştirmek için her adımda n'in 1 eksiği kadar karşılaştırma yapmış olacağız. Bu karşılaştırmaların sonucunda 1'den (n-1)'e kadar karşılaştırmada bulunacağız. Yani toplamda (n * (n-1) ) / 2 karşılaştırmada bulunmuş olacağız. Big O notasyonu olarak ifade edeceğimiz zaman dominant olan değeri göz önüne almamız gerektiği için O(n^2) sonucuna varırız.

---

**4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer?**

***Cevap***

Average Case kapsamına girer.

---

## [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

1. [3,7,5,8,2,9,4,15,6]
2. [3,5,7,8,2,9,4,15,6]
3. [2,3,5,7,8,9,4,15,6]
4. [2,3,4,5,7,8,9,15,6]
