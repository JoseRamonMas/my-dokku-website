# UT1 - Problema 4: Resolució de Sistemes d'Equacions amb la Regla de Cramer

**Agrupament:** Individual

<img src="./UT1Problema4.jpg" alt="Problema 4" width="200" />

### **Pregunta guia**

**Com podem desenvolupar un programa que ajude a resoldre sistemes d'equacions lineals utilitzant la regla de Cramer i a verificar els resultats per a aplicacions en àlgebra i càlcul matemàtic?**

### **Objectius d'aprenentatge**

En completar aquesta pràctica, sereu capaços de:

- Implementar càlculs matemàtics utilitzant variables i constants adequades.
- Utilitzar la regla de Cramer per resoldre sistemes d'equacions lineals.
- Verificar els resultats obtinguts per a garantir la seua exactitud.
- Practicar la formatació adequada d'eixida per a presentar resultats numèrics de manera estructurada.
- Documentar el codi amb comentaris per millorar la seua llegibilitat i mantenibilitat.

### **Context i descripció del problema**

Els sistemes d'equacions lineals són una part fonamental de les matemàtiques i tenen aplicacions en diverses àrees com l'enginyeria, l'economia i les ciències naturals. Per a resoldre sistemes d'equacions, una tècnica eficaç és la regla de Cramer, que proporciona una solució directa sempre que el sistema tinga un determinant no nul.

Un enginyer de software d'una empresa de simulacions científiques ens ha demanat desenvolupar un programa que implemente aquesta regla i verifique els resultats.

### **El problema a resoldre**

En aquesta activitat, utilitzarem la regla de Cramer per resoldre el següent sistema d'equacions lineals:

$$
\begin{cases}
3.4x + 50.2y = 44.5 \\
2.1x + 0.55y = 5.9 \\
\end{cases}
$$

Desenvolupar un programa que calcule els valors de \(x\) i \(y\) utilitzant la regla de Cramer i verifique els resultats obtenint el valor de \(y\) a partir de \(x\) a les equacions originals. Els resultats es mostraran amb dos xifres decimals. És important que el programa funcione de la mateixa manera per a tots els usuaris, per la qual cosa el format d'eixida ha de ser consistent en tots els casos.

### **Què necessites per a fer aquesta activitat?**

- Ordinador amb editor de text i el compilador "javac" funcionant. (Pots utilitzar NetBeans si ho prefereixes).
- Accés a recursos en línia per investigar la regla de Cramer i millors pràctiques de programació.

### **Requisits del programa**

1. **Entrada de dades:**
   - No cal entrada de dades per part de l'usuari, es treballa amb dades fixes per a aquesta simulació. Utilitza les **constants** i **variables** que cregues més adequades.

2. **Processament:**
   - Utilitzar la regla de Cramer per a calcular els valors de \(x\) i \(y\).
   - Verificar els resultats substituint els valors de \(x\) en les equacions originals.

3. **Eixida de dades:**
   - Mostrar el sistema d'equacions, la solució obtinguda per la regla de Cramer i la verificació dels resultats amb el format especificat.
   - **Important:** El format d'eixida ha de ser consistent per a tots els usuaris. Això vol dir que has de respectar el format que es presenta a continuació.

### **Exemple de funcionament del programa:**

```
SISTEMA D'EQUACIONS LINEALS
---------------------------
3.4x + 50.2y = 44.5
2.1x + 0.55y = 5.9

SOLUCIÓ PER CRAMER
------------------
x = 2.62
y = 0.71

COMPROVACIÓ DONADA LA 'x'

y = 0.71
y = 0.71
```

### **Instruccions**

1. **Investigació preliminar:**
   - Investiga la regla de Cramer i com es poden resoldre sistemes d'equacions lineals.
   - Cerca exemples de programes similars per entendre com estructurar el codi.

2. **Desenvolupament del programa:**
   - Escriu el codi en un editor de text senzill (bloc de notes, gedit, xed, nano...).
   - Utilitza la funció `System.out.printf` per assegurar que el format d'eixida és el correcte.
   - Afig comentaris al codi per explicar cada pas i facilitar la comprensió.

3. **Proves i depuració:**
   - Corregeix qualsevol error de compilació que aparega. Recorda anotar els problemes que trobes al informe final.

4. **Reflexió i documentació:**
   - Escriu un informe breu que incloga:
      - Una explicació del teu procés de desenvolupament.
      - Els reptes que has enfrontat i com els has superat.
      - Com aquest programa pot ajudar en l'estudi de l'àlgebra i altres aplicacions.
      - Suggeriments per a futures millores o funcionalitats addicionals.

### **Entrega**

- Envia el fitxer del codi font (`UT1Problema4.java`) i l'informe en un document PDF.
- Recorda seguir la convenció de noms.
- **Important:** Afig el teu nom i cognoms sempre com a comentari al principi dels fitxers JAVA (En NetBeans després de @author).

### ***Extensió opcional***
Per als estudiants que acaben abans o vulguen un repte addicional:

- Modifica el programa per permetre a l'usuari introduir les seues pròpies dades per a les constants \(a\), \(b\), \(c\), \(d\), \(e\), i \(f\).
- Implementa la resolució de sistemes 3x3 utilitzant la regla de Cramer.