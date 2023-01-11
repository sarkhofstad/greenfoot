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

# Week 3: logische operatoren & overriding

## Les 5 (logische operatoren)

### Leerdoelen
- Je kunt logische operatoren toepassen
- Verder oefenen met beslissingen

### Logische operatoren

Er zijn drie belangrijke logische operatoren:
- `&&` - en/and
- `||` - of/or
- `!` - niet/not

### Huiswerk voor volgende les
[Operatoren opdracht](Operatoren.md) + Informatica-Actief, opgave 3.10 t/m, 3.12

## Les 6 (overerving & overriding)

### Leerdoelen
- Je kan een klassendiagram maken.
- Je kan overriding toepassen in Java.
- Je kan het verschil tussen overerving en overriding uitleggen.
- Je kan een subklasse aanmaken.


### Overerving
Bij overerving erft een subklasse methodes en velden over van diens superklassen. De klasse `Kitty` erft bijvoorbeeld de methode `move()` van Animalklasse en de velden `x` en `y` van de Actorklasse. Dit omdat `Kitty` een subklasse is van `Animal` én van `Actor`.

Kijk naar het onderstaande voorbeeld:

```java
class Kat {
    void saySomething() {
        System.out.println("Meow!");
    }
}

class HuisKat extends Kat {

}
```

In het voorbeeld hierboven is `HuisKat` een subklasse van `Kat` (dit kan je zien aan het stukje `extends Kat`). Als ik de code hieronder run, zal de output van mijn programma `"Meow!"` zijn. Dit komt doordat de huiskat de methode `saySomething()` *overerft* van de klasse `Kat`.

```java

HuisKat huisKat = new HuisKat();

huisKat.saySomething();

```


### Overriding
Bij overerving overschrijft een methode in een subklasse een methode die overerfd is uit een superklasse. In het voorbeeld hieronder is `HuisKat` een subklasse van `Kat` (dit kan je zien aan het stukje `extends Kat`). De methode `saySomething()` in `HuisKat` *overschrijft* de methode `saySomething()` in `Kat`.  

```java
class Kat {
    void saySomething() {
        System.out.println("Meow!");
    }
}

class HuisKat extends Kat {
    void saySomething() {
        System.out.println("Woof!");
    }
}
```

Als ik de code hieronder run, krijg ik de output `"Woof!"`. Dit komt doordat de klasse `HuisKat` de methode `saySomething()` *override*. De implementatie van `saySomething()` in `HuisKat` neemt prioriteit over de implementatie in `Kat`.

```java

HuisKat huisKat = new HuisKat();

huisKat.saySomething();

```

### Huiswerk voor volgende les
Informatica-Actief inhoud 4: opdracht 4.1 t/m 4.5


## Les 7: Herhaling

Deze les was een herhaling. Er hoorde geen nieuwe stof bij deze les

## Les 8: Variabelen

### Leerdoelen
- Je kan het verschil tussen een lokale variabele en een veld uitleggen.
- Je kan het verschil tussen een public en private variabele uitleggen.
- Je kan een variabele en veld gebruiken in Java-code.
- Je kan wiskundige operatoren toepassen op variabelen & velden.

### Variabelen

Een variabele is een soort vakje waar je een bepaalde waarde in kan opslaan. Deze waarde kan je later veranderen. Een variabele kan je gebruiken om bijvoorbeeld op te slaan hoeveel vijanden de speler heeft verslaan. 

Er zijn een aantal dingen om te onthouden over variabelen:

- De naam en datatype van een variabele kan je niét veranderen.
- De waarde van een variabele kan je wél veranderen.

#### Een variabele aanmaken
Met deze code maak je een variabele aanmaken. Je geeft de datatype, naam, én de initiële waarde van de variabele. (vergeet niet de `;`!)

``` java
// In het algemeen
<datatype> <naam> = <initiele_waarde>;

// Voorbeeld 
int a = 5;
```

#### De waarde van een variabele veranderen
Met deze code kan je de waarde van een *bestaande* variabele veranderen. Je geeft alleen de naam aan, want de computer weet al welke datatype die heeft. Geef dus ***NIET*** de datatype!

```java
// In het algemeen
<naam> = <nieuwe_waarde>;

// Voorbeeld
a = 10;
```

#### De waarde van een variabele gebruiken
Je kan de waarde van een variabele gebruiken met de naam. Dit kan bijvoorbeeld in een if-statement, maar ook om de waarde van een nieuwe variabele te geven!

```java
// Voorbeeld if-statement
if (a == 5) {
    // doe iets
}

int b = a;
```

### Lokale variabele
Een lokale variabele kan alleen in 1 specifieke code-blok gebruikt worden. Als de computer klaar is met die code blok uitvoeren, dan verdwijnt de variabele. Je kan het daarna dus niet meer gebruiken/veranderen.

Een code-blok wordt aangeduid met accolades `{`, `}`, dit kan dus een if-statement zijn, maar ook bijvoorbeeld een methode! Bij klassen werkt het iets anders: dan noemen we het een veld (dat zie je in het kopje hieronder).

```java
// Voorbeeld met een if-statement
if (a == 5) {
    int b = 5;
    // Binnen de if-statement kan ik de variabele b gebruiken.
}
// Hier kan ik het dus niet meer gebruiken! Als ik het probeer te gebruiken, krijg ik een error!
```

```java
// Voorbeeld met een methode, hier kan de variabele alleen in de methode gebruikt worden.
public void foo() {
    int c = 10;

    // hier kan ik c dus gebruiken
}

// maar buiten de methode niet!
```

### Velden
Velden zijn variabelen die je kan gebruiken door de hele klas heen. De waarde van die variabele blijft dus opgeslagen, ook nadat je een methode uit hebt gevoerd. Een veld maak je aan buiten de methodes, maar in de klasse. 

In een veld kan je informatie opslaan die je langer nodig hebt dan alleen in 1 blokje code; denk bijvoorbeeld aan de x en y coördinaten van een speler.

```java
// Voorbeeld
class Person {
    int age = 10;
    String name = "SARK";

    void sayHello() {
        // TO DO
    }
}
```

#### Huiswerk voor de volgende les
Informatica-Actief: Inhoud 5 (t/m opdracht 5.6)