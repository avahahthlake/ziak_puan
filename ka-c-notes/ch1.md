# chapter 1 a ka notes siam ho 🕐️

## Program hmasa ber chu 🌛

A hnuaia mi code hi eng programming language pawh kan zir a kan bul tanna a ni tlangpui a...
```c
#include <stdio.h>

int main() {
    printf("Chibai le, aw khuavel!\n");
    return 0;
}
```

```output
Chibai le, aw khuavel!
```

> Windows system i neih chuan
>   1. gcc i download ang a
>   2. i install ang a
>   3. environment variables ah gcc chhunga bin folder path kha i add ve ang a
>   4. cmd hmangin khimi program i save na folder ah i va lut ang a.
>   5. gcc program-hming.c -o program-hming.exe (hei hi i chhu lut anga)
>   6. error a awm loh chuan program-hming.exe tih a lo awm belh ang a
>   7. chu chu i chhu lut ang a a ouput a lo lang mai ang

> Linux system i neih chuan
>   * hei chu mamawh dan azirin ka fill up tawh mai ang.

> Mac system i neih chuan
>   * hei pawh linux zulin

### Program hmasa ber bih chianna...🕵️

```c
#include <stdio.h>                      // hei hian standard input output library a kan thil mamawh tur a la

int main() {                            // hei hi eng kan program bul tanna a ni, function a ni, chu function hming chu 'main' a ni
    printf("Chibai le, aw khuavel!");   // hei hi function tho printf tih hmanna a ni, argument ah string ka pass thei a, kan pass reng bawk a
    return 0;                           // function tin hian return type an nei vek a, hemi program ah hian kan return type hi integer (int) a nia, chuan ka program a kal tluang chuan 0 a return (pe let) mai dawn a ni
}                                       // kan program main block tawp kharna a nih hi
```

### Hlam leh kutphah

Mizo te thil teh dan ah chuan hlam khat hi kutzung tang hmawr pakhat atanga a hmawr lehlam thleng a nia. Chu chu ka'n teh vel chhin a, keimahah chuan hlam sawm vel chiah chiah a nia. Chu mi zul deuh chuan program ziak dawn chhin ila...

    * kan logic hman tur ber chu hlam-khat = kutphah 10

```c
#include <stdio.h>

int main() {
    int kutphah = 0;
    int hlam = 0;
    
    for (int hlam = 0; hlam < 10; hlam++) {
        kutphah = hlam * 10;
        printf("Hlam %d chuan kutphah %d a tluk a ni\n", hlam, kutphah);
    }

    return 0;
}
```

```output
Hlam 0 chuan kutphah 0 a tluk a ni
Hlam 1 chuan kutphah 10 a tluk a ni
Hlam 2 chuan kutphah 20 a tluk a ni
Hlam 3 chuan kutphah 30 a tluk a ni
Hlam 4 chuan kutphah 40 a tluk a ni
Hlam 5 chuan kutphah 50 a tluk a ni
Hlam 6 chuan kutphah 60 a tluk a ni
Hlam 7 chuan kutphah 70 a tluk a ni
Hlam 8 chuan kutphah 80 a tluk a ni
Hlam 9 chuan kutphah 90 a tluk a ni
```

## C data type hrang hrang te

Tah hi chuan, Maths kan zir thin kha ngaihtuah let la, number chi hrang hrang an awm kha.

    * Integers an awm a
    * Rational/fractional/decimal numbers an awm a
  
Hetiang deuh chiah hian programming ah chuan computer ah hian data kan store thin tih kan hriat a tha, data chu chi hrang hrang an awm...C ah chuan heng pathum hi hriat a tha e...

    * Integers
        * int kan ti mai zel
        * number point nei lo ang chi kha
        * entir nan 1 te, 23, te 3000 te
  
    * Floating point numbers
        * float kan ti mai zel
        * number point nei ho
        * entir nan 3.14 te, 2.10 te, 0.11 te pawh
  
    * Characters
        * char kan ti mai zel
        * ascii characters ho kha
        * entir nan 'a' te, 'z' te, '1' te pawh, '!' te pawh a tel ve vek
        * ascii corresponding number an nei theuh bawk