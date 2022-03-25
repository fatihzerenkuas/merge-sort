## **Sorular**
[16,21,11,8,12,22] -> Merge Sort

1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.

## **Cevaplar**
1. 
    * ### Dizide 6 eleman olduğu için 3-3 bölünecek 
        * **[16,21,11]** - **[8,12,22]**
    * ### Daha sonra 3 elemanı olan dizinler de tek eleman kalana kadar bölünecek. 
        * **[16]** - **[21,11]** -------------------- **[8]** - **[12,22]**
        * **[16]** - **[21]** - **[11]** ----------------- **[8]** - **[12]** - **[22]**
    * ### Daha sonra sol ve sağdaki elemanlar küçükten büyüğe olacak şekilde birleşecek.
        * **[16,21]** - **[11]** --------------------- **[8,12]** - **[22]**
    * ### Soldan başlayarak ilk elemanı yanındaki elemanla karşılaştırıp en küçükten başlayarak yeniden sıralamaya başlıyoruz.  
        * **[11,16,21]** ------------------------- **[8,12,22]**
    * ### Son adımda da sol ve sağdaki dizinlerdeki ilk elemanlardan başlayarak karşılaştıra karşılaştıra küçükten büyüğe sıralıyoruz.
        * **[8,11,12,16,21,22]**
___
2. Elemanlar her seferinde n kadar sıralanıyor. Bu sıralama her seferinde yarıya indiği için 2^x=n logn=x dolayısıyla

     Time Complexity'si **O(nlogn)** olarak gösterilir.

