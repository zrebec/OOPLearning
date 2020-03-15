# Triedy
Java je celá objektovo orientovaná. Znamená to, že čokoľvek je objekt. Už aj keď
vytvárame základný výpis **Hello, World!**, kde pri neobjektových jazykoch stačí
väčšinou napísať niečo v zmysle, 
```
print ("Helllo, World!")
```
tak v Jave na toto potrebuje najskôr vytvoriť objekt (obyvkle by mal aj v 
nejakom) balíčku a následne v metdóde ```main``` (hlavná metóda z celého 
balíčku alebo triedy), môžeme vypísať naše **Hello, World!**. Teda správny
zápís by mal byť:

```
package com.example.javalearning.classes;

class HelloWorld {

    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }

}
```

Prvý riadok určuje teda balíček v ktorom sa naša trieda nachádza. Následne
prichádza deklarácia triedy (je dobré dodržiavať štábnu konvenciu, kde názov
triedy začíname veľkým písmenom a každé slovo ktoré určuje názov triedy je tiež
veľkým písmenom), v našom prípade teda ```HelloWorld``` a následne prichádza
deklarácia metódy našej triedy. Keďže chceme iba vypísať **Hello, World!**,
stačí nám metóda main, ktorá však musí byť ```public```, ```static``` (pojmy 
vysvetlíme neskôr) a nevracia žiadnu hodnotu (to je to označenie ```void```).
Následne v zátvorkách určujeme vstupné parametre. Metóda main má vstupné 
argumenty pole textových reťazcov, ktoré uvádzame pri štarte programu. Ak, by
sme chceli vypísať nie, **Hello, World!**, ale iný text, ktorý určime ako 
vstupný parameter metódy, tak by sme našu triedu upravili iba minimálne. 
Konkrétne riadok výpisu by sme zmenili na

```
System.out.println("Hello, " + args[0]);
``` 

Keďže polia sa indexujú od 0, znamená to, že prvá vstupná hodnota v poli je 
práve označovaná ako **index 0**.