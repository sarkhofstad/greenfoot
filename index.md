# Welkom!

Op deze pagina kan je een samenvattig vinden van elke les. Verder kan je zien wat het huiswerk is en overige opmerkingen over de les.

- week 1: introductie
    - les 1: datatypen & objecten
    - les 2: methodes
- week 2: 
- week 3:
- week 4:
- week 5:

# Week 1: Introductie
## Les 1 (datatypen & objecten)

### Leerdoelen
- je kunt aan bepaalde waarde zien wat voor datatype het is
- je kunt aan een klasse/objectnaam zien of het een klasse of object is
- je maakt kennis met Greenfoot (game engine)

### Datatypes
De belangrijkste datatypen in Java zijn:
- `int`: volledig getal, dus (..., -2, -1, 0, 1, 2, ...)
- `boolean`: true/false
- `String`: Woorden/zinnen, bijv: "Hello world" (let op, dubbele aanhalingstekens)

### Objecten & Klassen
#### Objecten
- basis bouwsteen bij object oriented programmeren
- specifieke instantie van een klasse
- bijv. mijnHondTommy

#### Klassen
- beschrijft het gedrag van een categorie aan objecten
- bijv. Hond, Kat

### Huiswerk voor de volgende les
Thuis op je computer Greenfoot installeren.

## Les 2 (methodes)

### Leerdoelen
- je kan de verschillende elementen van een methode benoemen.
- je kan aan een specifieke methode zien wat de naam, return-type en  parameters zijn.
- je kan een methode aanroepen in de Greenfoot-UI.
- je kan een methode aanroepen in java code.

### Methodes

Methodes hebben 4 delen:
- return type (void, int, boolean, String)
- parameters (elke parameter heeft een type en een naam)
- naam
- code

#### Aanmaken

Een methode aanmaken ziet er zo uit:

```java
int plus(int a, int b) {
    return a + b;
}
```

#### Aanroepen (gebruiken)

Een methode aanroepen ziet er zo uit:

```java
// met parameters
plus(5,6);
// zonder parameters
move();
```

### Lescheck
- [V5in1](https://forms.gle/LqQKoRQH184xmVwu8)
- [V5in2](https://forms.gle/Thsmugy1AgHyvMc99)

### Huiswerk voor volgende les
Opdrachten les 2 (Dodo naar het ei). (De extra opgaven hoeven niet)

# Week 2: Methodes & Beslissingen
## Les 3 (methodes & javadoc)
### Leerdoelen
- je kan een eigen methode aanmaken en daarbij een bewuste keuze maken over de return-type en parameters
- je kan met simpele methodes wat meer complexe taken uitvoeren
- je kan JavaDoc schrijven van je zelfgemaakte methodes
### Javadoc
Javadoc ziet er als volgt uit:
```java
/**
* Adds two numbers.
* @param int a first number to add
* @param int b second number to add
* @return int a and b added together
*/
int plus(int a, int b) {
  return a + b;
}
```

Aan het begin is er een zin/paragraaf die beschrijft in woorden wat de methode doet. 

Daarna volgt een lijst met alle parameters. Zijn er geen parameters? Dan kan je dit weglaten. Elke parameter is als volgt: `@param <datatype> <naam> <beschrijving>`.


Als laatst volgt er een regel waarin staat wat de methode returnt. Heeft de methode als return-type `void`? Dan kan je dit weglaten. Die is als volgt: `@return <returntype> <beschrijving>`.