# Algoritma
## Menentukan angka ganjil dan genap

Algoritma ini ditulis untuk memecahkan masalah menentukan suatu bilangan ganjil atau genap.

1. Mulai
2. Siapkan (x)
3. Bilangan (x) jika dimoduluskan dengan 2 hasilnya 0 maka bilangan tersebut merupakan bilangan genap
4. Jika (x) dimoduluskan dengan 2 hasilnya lebih dari 0 maka bilangan tersebut bilangan ganjil
5. Selesai

## Flowchart

Sebuah Flowchart untuk memecahkan apakah bilangan merupakan ganjil atau genap.


```mermaid
flowchart TD

start@{shape: circle, label: "start"}
num@{shape: lean-r, label: "x"}
con@{shape: diam, label: "x % 2 == 0"}
outputGenap@{shape: lean-r, label: '"Angka merupakan bilangan genap"'}
outputGanjil@{shape: lean-r, label: '"Angka merupakan bilagan ganjil"'}
finnish@{shape: double-circle, label: "stop"}

start-->num-->con
con-- False -->outputGanjil
con-- True -->outputGenap
outputGanjil-->finnish
outputGenap-->finnish

```

```pseudo
DECLARE x: INTEGER

INPUT x

IF x % 2 == 0 THEN
    OUTPUT "Angka merupakan bilangan genap"
ELSE
    OUTPUT "Angka merupakan bilangan ganjil"
ENDIF
```