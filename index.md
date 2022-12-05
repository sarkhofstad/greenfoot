# Welkom!

Op deze pagina kan je een samenvattig vinden van elke les. Verder kan je zien wat het huiswerk is en overige opmerkingen over de les.

- week 1: introductie
    - les 1: datatypen & objecten
    - les 2: methodes
- week 2: methodes & beslissingen
    - les 3: methodes (vervolg)
    - les 4: beslissingen
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

### Lescheck 1
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
* @param a first number to add
* @param b second number to add
* @return a and b added together
*/
int plus(int a, int b) {
  return a + b;
}
```

Aan het begin is er een zin/paragraaf die beschrijft in woorden wat de methode doet. 

Daarna volgt een lijst met alle parameters. Zijn er geen parameters? Dan kan je dit weglaten. Elke parameter is als volgt: `@param <naam> <beschrijving>`.


Als laatst volgt er een regel waarin staat wat de methode returnt. Die is als volgt: `@return <beschrijving>`. Heeft de methode als return-type `void`? Dan kan je dit weglaten. 

### Huiswerk voor volgende les
[Opdrachten les 3](Opdrachten_les3.md) (niet de EXTRA opgaven).

## Les 4 (beslissingen)
### Leerdoelen
- Je kan de verschillende onderdelen van een if/else statement benoemen.
- Je kan een stroomdiagram maken die een beslissing weergeeft.
- Je kan van een stroomdiagram Java code schrijven die een beslissing maakt.

### if-statements

If-statements zien er zo uit:

```java
if (voorwaarde) {
    // Code die moet uitgevoerd worden als voorwaarde waar (true) is.
}
```

If-else statements zien er zo uit:

```java
if (voorwaarde) {
    // Code die moet uitgevoerd worden als voorwaarde waar (true) is.
} else {
    // Code die moet uitgevoerd worden als voorwaarde niet waar (false) is.
}
```

### Lescheck 2
[V5in1](https://forms.gle/xGuRdef3sgGBQbW18)
[V5in2](https://forms.gle/j9fSBjFdLyMiXZqm9)

### Huiswerk voor volgende les
Informatica-Actief, inhoud 3: opdracht 3.1 t/m opdracht 3.5