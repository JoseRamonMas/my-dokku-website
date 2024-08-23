# Índex de continguts

- [UT1.2 Tipus de dades simples](#ut12-tipus-de-dades-simples)
- [Manipulació de dades](#manipulació-de-dades)
- [Tipus de dada](#tipus-de-dada)
- [Tipus de dades estàndard](#tipus-de-dades-estàndard)
- [Tipus de dada enter](#tipus-de-dada-enter)
- [Tipus de dada real](#tipus-de-dada-real)
- [Tipus Enter vs Real](#tipus-enter-vs-real)
- [Tipus booleà](#tipus-booleà)
- [Tipus de dada caràcter](#tipus-de-dada-caràcter)
- [Operacions amb dades primitives](#operacions-amb-dades-primitives)
- [Operacions amb enters](#operacions-amb-enters)
- [Operadors divisió entera (/) i mòdul (%)](#operadors-divisió-entera--i-mòdul-)
- [Operadors amb enters](#operadors-amb-enters)
- [Operacions amb reals](#operacions-amb-reals)
- [Operacions entre caràcters](#operacions-entre-caràcters)
- [Operacions amb booleans](#operacions-amb-booleans)
- [Construcció d'expressions](#construcció-dexpressions)
- [Avaluació d'expressions](#avaluació-dexpressions)
- [Desbordament i errors de precisió](#desbordament-i-errors-de-precisió)

---

## UT1.2 Tipus de dades simples

En aquesta unitat estudiarem els tipus de dades simples en programació, centrant-nos en la seua manipulació i característiques principals.

---

## Manipulació de dades

La manipulació de dades és un concepte fonamental en programació. És important entendre:

- El procés pel qual s'ordena a la memòria guardar o recuperar dades.
- Les dades són tota la informació que l'ordinador utilitza en les execucions de programes.
- Cada dada es tracta per separat. Per exemple, un programa que suma 2 nombres treballa amb tres dades diferents (els dos sumands i el resultat).

---

## Tipus de dada

Un **tipus de dada** es defineix com:

1. El conjunt de valors vàlids que pot prendre una dada.
2. El conjunt d'operacions (transformacions) que se li poden aplicar.

**Exemples de dades numèriques:**
- Una ciutat està a 8.25 km d'una altra
- Una persona té 30 anys
- Han passat 15 dies des d'un esdeveniment

**Exemples de dades alfabètiques:**
- El meu gat es diu Milo
- Estudie a l'IES Poeta Paco Mollà
- Visc al Carrer del castell

És important recordar que els valors que pot prendre cada dada són limitats, ja que utilitzem la memòria de l'ordinador, que és finita.

---

## Tipus de dades estàndard

Els tipus de dades estàndard són aquells que, d'una manera o altra, tots els llenguatges de programació suporten:

- **Enter**: Representa valors numèrics sense decimals.
- **Real**: Representa valors numèrics amb decimals.
- **Caràcter**: Representa una unitat fonamental de text.
- **Booleà**: Representa valors lògics (veritat o falsedat).

---

## Tipus de dada enter

- Representa un valor numèric, positiu o negatiu, sense decimals.
- Exemples de literals enters: 3, 0, -345, etc.
- En la majoria de llenguatges, el rang típic és de -2,147,483,648 a 2,147,483,647.
- S'utilitza per representar dades com: edat, dia del mes, any, quantitat de fills, etc.

```java
int edat = 30;
int anyNaixement = 1992;
int numeroFills = 2;
```

En Java, tenim quatre tipus de dades que representen valors enters:
- `byte`: 8 bits (-128 a 127)
- `short`: 16 bits (-32,768 a 32,767)
- `int`: 32 bits (-2,147,483,648 a 2,147,483,647)
- `long`: 64 bits (-9,223,372,036,854,775,808 a 9,223,372,036,854,775,807)

Per a literals `long`, s'afegeix una "L" al final:

```java
long poblacioMundial = 7800000000L;
```

---

## Tipus de dada real

- Representa un valor numèric, positiu o negatiu, amb decimals.
- Exemples de literals: 2.25, 4.0, 45, 3., 100.3, .5, etc.
- S'utilitza per representar dades com: un preu en euros, el rècord mundial dels 100m llisos, la distància entre ciutats, etc.

En Java, tenim dos tipus principals per a representar valors reals:
- `float`: 32 bits de precisió simple
- `double`: 64 bits de precisió doble (més precís)

```java
float preuProducte = 19.99f;
double distanciaEstrella = 1.5e8; // 150 milions de km
```

---

## Tipus Enter vs Real

És important entendre per què existeix el tipus enter si es pot representar el mateix valor amb tipus real:

1. **Precisió**: Els enters són exactes, mentre que els reals poden tenir errors d'arrodoniment.
2. **Eficiència**: Les operacions amb enters solen ser més ràpides.
3. **Memòria**: Els enters ocupen menys espai en memòria.
4. **Semàntica**: Alguns conceptes són inherentment enters (com el número de persones).

<img src="PRG_UT12_val_images/imatge2.jpg" alt="Imatge 2" />

---

## Tipus booleà

- Representa un valor de tipus lògic per establir la veracitat o falsedat d'un estat o afirmació.
- Només té dos valors possibles: `true` / `false`
- Exemples d'ús: interruptor (On / Off), casat (Sí / No), dret a vot, contrasenya és correcta, etc.

```java
boolean llumEncesa = true;
boolean esMajorEdat = false;
boolean passwordCorrecta = true;
```

---

## Tipus de dada caràcter

- Representa una unitat fonamental de text usada en qualsevol alfabet, un nombre o signe de puntuació o exclamació.
- Exemples de literals: 'a', 'A', '4', '>', '?', 'Γ' (lletra grega gamma majúscula), etc.
- S'utilitza per representar símbols individuals de l'alfabet, dígits, signes, etc.

```java
char lletra = 'A';
char digit = '7';
char signe = '+';
```

---

## Operacions amb dades primitives

Cada tipus de dada admet únicament una sèrie d'operacions concretes. Per exemple, no es pot sumar una dada de tipus enter amb una dada de tipus booleà.

Tipus d'operacions:
- **Unàries**: Només un operand (ex: negació)
- **Binàries**: Dos operands (ex: suma, resta)

---

## Operacions amb enters

**Operadors aritmètics:**
- Unaris: `-` (Canvi de signe)
- Binaris: `+`, `-`, `*`, `/`, `%`

```java
int a = 10;
int b = 3;
int suma = a + b;      // 13
int resta = a - b;     // 7
int multiplicacio = a * b;  // 30
int divisioEntera = a / b;  // 3
int modul = a % b;     // 1
```

---

## Operadors divisió entera (/) i mòdul (%)

La divisió entera (`/`) retorna el quocient sense decimals, mentre que l'operador mòdul (`%`) retorna el residu.

```java
int dividend = 17;
int divisor = 4;

int quocient = dividend / divisor;  // 4
int residu = dividend % divisor;    // 1
```

---

## Operadors amb enters

**Operadors relacionals o de comparació:**
- `==` (igual)
- `!=` (diferent)
- `>` (major que)
- `<` (menor que)
- `>=` (major o igual)
- `<=` (menor o igual)

Aquests operadors sempre retornen un valor booleà (`true` o `false`).

```java
int x = 5;
int y = 10;

boolean iguals = (x == y);      // false
boolean diferent = (x != y);    // true
boolean major = (x > y);        // false
boolean menor = (x < y);        // true
boolean majorIgual = (x >= y);  // false
boolean menorIgual = (x <= y);  // true
```

---

## Operacions amb reals

Les operacions amb reals són similars a les dels enters, excepte que no s'apliquen les operacions de mòdul (`%`) i els operadors de bits.

```java
double a = 5.5;
double b = 2.0;

double suma = a + b;      // 7.5
double resta = a - b;     // 3.5
double multiplicacio = a * b;  // 11.0
double divisio = a / b;   // 2.75
```

---

## Operacions entre caràcters

Amb caràcters, principalment s'utilitzen operacions relacionals:

```java
char c1 = 'A';
char c2 = 'B';

boolean diferent = (c1 != c2);  // true
boolean igual = (c1 == c2);     // false
boolean menorQue = (c1 < c2);   // true (basat en el codi ASCII)
```

---

## Operacions amb booleans

**Operadors lògics:**
- `&&` (AND)
- `||` (OR)
- `!` (NOT)

**Operadors relacionals:**
- `==` (igual)
- `!=` (diferent)

```java
boolean a = true;
boolean b = false;

boolean andResult = a && b;  // false
boolean orResult = a || b;   // true
boolean notA = !a;           // false

boolean sameValue = (a == b);  // false
boolean differentValue = (a != b);  // true
```

---

## Construcció d'expressions

Una expressió és una combinació d'operadors i operands. Ha de ser correcta sintàctica i semànticament.

Regles sintàctiques:
1. Un literal per si mateix és una expressió.
2. Una expressió entre parèntesis és una expressió vàlida.
3. Una expressió precedida per un operador unari és una expressió vàlida.
4. Dues expressions separades per un operador binari formen una expressió vàlida.

Exemples:
- `6`
- `(6 + 5)`
- `-4`
- `6 + 5`
- `(6 + 5) * -4`

Regles semàntiques:
1. Les operacions han de ser entre dades del mateix tipus (o tipus compatibles).
2. L'operació ha d'existir per al tipus de dada operat.

---

## Avaluació d'expressions

En avaluar expressions, cal tenir en compte l'ordre de precedència dels operadors. En cas d'empat, es resol d'esquerra a dreta.

Exemple d'avaluació:

```java
boolean resultat = ((3 + 4) == 7) && !(12.3 > 2.11) || ('a' == 'B');
```

Passos d'avaluació:
1. `(3 + 4)` → `7`
2. `7 == 7` → `true`
3. `12.3 > 2.11` → `true`
4. `!(true)` → `false`
5. `'a' == 'B'` → `false`
6. `true && false` → `false`
7. `false || false` → `false`

Resultat final: `false`

---

## Desbordament i errors de precisió

El desbordament ocorre quan intentem emmagatzemar un valor més gran del que pot contenir el tipus de dada escollit.

Exemple de desbordament:

```java
int valorGran = 2147483647;  // Valor màxim per a int
valorGran = valorGran + 1;   // Això causarà desbordament
System.out.println(valorGran);  // Imprimirà -2147483648
```

Per evitar aquest problema, hem d'escollir el tipus de dada adequat:

```java
long valorGran = 2147483647L;
valorGran = valorGran + 1;
System.out.println(valorGran);  // Imprimirà 2147483648
```

És important seleccionar el tipus de dada apropiat per a cada situació per evitar errors de precisió i desbordament.