# Veri-Yapilari-ve-Algoritmalar-Merge-Sort
## Merge Sort 

* Merge Sort çok kullanılan bir sıralama algoritmasıdır.
* Sıralama için böl ve yönet paradigmasını kullanır.
* Problemi alt problemlere böler ve onları tek tek çözer.
* Daha sonra orijinal problemin çözümünü elde etmek için alt problemlerin sonuçlarını birleştirir.
 

## Birleştirme Sıralaması Nasıl Çalışır?

* Verilen sıralanmamış diziyi sol ve sağ alt diziler olmak üzere iki yarıya böler.
* Alt diziler özyinelemeli olarak bölünür.
* Bu bölme, her bir alt dizinin boyutu 1 olana kadar devam eder.
* Her alt dizi yalnızca tek bir öğe içeriyorsa, her bir alt dizi önemsiz şekilde sıralanır.
* Ardından birleştirme prosedürü çağrılır.
* Birleştirme prosedürü, son bir sıralanmış dizi üretmek için bu önemsiz şekilde sıralanmış dizileri birleştirir.
 
## Merge Sort Proje Örneği

```
[16,21,11,8,12,22]
```
* Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
* Big-O gösterimini yazınız.
## Merge Sort algoritması şu şekilde çalışır:

```                 Sıralanmamış dizi

                   [16,21,11,8,12,22]       -------->  Sıralanmamış Dizi
                          /\
                         /  \
             [16,21,11]       [8,12,22]     -------->  Bölme
                 /\              /\
                /  \            /  \
          [16,21]  [11]     [8,12]   [22]   -------->  Bölme
            /\      |         /\      |
           /  \     |        /  \     |
        [16] [21]  [11]  [8]  [12]   [22]   -------->  Önemsiz şekilde sıralanmış
          \  /      |      \  /       |
           \/       |       \/        | 
         [16,21]  [11]    [8,12]     [22]   -------->  Birleştirme
              \  /              \  /
               \/                \/ 
             [11,16,21]     [8,12,22]       -------->  Birleştirme
                        \  /
                         \/ 
                 [8,11,12,16,21,22]         -------->  Sıralı Dizi
                 
                 
                 Big-O gösterimi :  O(nlogn)
                 Adım sayısı hep yarıya düştüğü için 2^x = n den logn .
                 Bu işlem n kez gerçekleşeceği için O(nlogn)
             
```
## Time Complexity Analizi
### Merge Sortta, diziyi iki (yaklaşık olarak) eşit parcaya  böleriz ve bunları yalnızca birleştirme sıralamasını kullanarak özyinelemeli olarak çözeriz.
             
* Adım sayısı hep yarıya düştüğü için 2^x = n den logn .
* Bu işlem n kez gerçekleşeceği için O(nlogn)

### Merge Mort algoritmasının Time Complexity Analizi : T(n) = Θ(nlogn). 
  



 

