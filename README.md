# m3-uf1-exc1
## Exercici 1: Variables, tipus de dades primitius i operadors a Java

En aquest exercici haureu de respondre les següents preguntes, substituint allà on posi //TODO per la vostra resposta.

Haureu d'utilitzar el jshell per a testejar tot el codi relacionat amb cada pregunta, i al final de l'exercici haureu d'incloure en aquest repositori els fitxers _history_ i _snippets_ (seguint el patró de noms establert a l'exercici 0) corresponents a aquest exercici, **directament al directori arrel del repositori**.

### Criteris de qualificació:
* Si no s'incorporen els fitxers _history_ i _snippets_ amb els seus continguts que demostrin que l'alumne ha treballat en les respostes a cadascuna de les preguntes, la qualificació serà de 0.
* Cada pregunta val un punt, i la seva qualificació podrà ser de 0, 0.5 o 1, depenent de si la resposta és errònia o molt poc encertada (0), si és parcialment correcte (0.5) o de si és totalment correcte (1).
* Hi ha 10 preguntes, i la qualificació mínima per a superar aquest exercici és de 5/10.
* S'avaluarà la correctesa en la resposta, així com la seva **claredat** (que no presenti ambigüitats).
* Tot i que l'enunciat està redactat en català, l'alumne pot respondre, a banda de en català, en anglès o en espanyol. Faltes d'ortografia en el redactat penalitzarà la nota.

### Preguntes

#### Pregunta 1

Declara dues variables de tipus _byte_, **b0** i **b1**, i assigna-lis respectivament els valors 122 i 14:
```
byte b0 = 122; byte b1 = 14;
```

Suma les dues variables, sense assignar el resultat a cap variable (jshell l'assignarà automàticament a un variable temporal, que comença per _$_):
```
b0 + b1
```
Quin resultat obtenim? Per què? De quin tipus de dada és la variable temporal creada per jshell?

El resultat que obtenim és 136. La dada temporal creada per jshell és un integer.

#### Pregunta 2

Declara una variable de tipus _char_ anomenada c, i assignali el valor 'a':
```
char c = 'a';
```
Declara una variable de tipus _int_, anomenada n, i assigna-li el valor de la variable c:
```
int n = c;
```
Quin resultat obtens? Per què?

El resultat que obtenim és 97, perquè és el número que li correspon a la a en la taula ascii i perquè el jshell està programat per assignar-l'ho

Ara, declara una variable de tipus _short_, anomenada s, i assigna-li el valor de la variable c:
```
short s = c;
```
Per què ara el resultat obtingut és diferent que en el cas anterior?

Perquè és //TODO

#### Pregunta 3

Continuant amb les variables de tipus _char_ i _short_ declarades a l'exercici 2, ara executeu:
```
short s = (short)c;
```
Com s'anomena això que estem fent amb la variable c? Quin resultat obtenim ara? Per què (què està passant)?

Aquest procès s'anomena "casting". El resultat que obtenim és 97 perquè la variable "c" ha sigut forçada, és a dir, que la variable "c" es com si fos una variable de tipus short (forçada per el casting).


#### Pregunta 4

Executa el següent codi amb el jshell:
```
short s = (short)32000;
```

```
short s = (short)35000;
```

Quins resultats obtens? Per què?

A la primera execució obtenim s = 32000 (és a dir, que l'agafa perquè el tipus de dada de short té un interval i aquest resultat esta dins d'aquest interval), a la segona execució obtenim -30536 perquè el 35000 està fora del interval del short, al fer el casting estem ficant un integer a un short travès d'un casting. Quan fem el casting estem fent 

#### Pregunta 5

Executa el següent codi amb el jshell:
```
var v = 5.0;
```

```
var v0 = 5;
```

De quin tipus de dada són les variables v i v0?

//TODO

Ara, executa:
```
var v1 = v + v0;
```

De quin tipus de dada és la variable v1? Per què (què està passant en fer-se la suma)?

//TODO

#### Pregunta 6

**Operadors bitwise**

Executeu el següent codi amb jshell:

```
4 & 4;
4 | 4;
4 ^ 4;
~4;
```

Què retorna en cada cas? Per què?

//TODO

**Hint**: Per ajudar a visualitzar el què està passant, podeu usar la instrucció _intToBin()_. Exemple:
```
intToBin(4);
intToBin(4 & 4);
```

#### Pregunta 7

**Operadors shift**

Executeu el seguent codi amb jshell:

```
4<<2
4<<28
4<<29
4<<30
4<<31
```

Què retorna en cada cas? Per què?

//TODO

**Hint**: Per ajudar a visualitzar el què està passant, podeu usar la instrucció _intToBin()_. Exemple:
```
intToBin(4);
intToBin(4 << 2);
```

#### Pregunta 8

Declareu dues variables de tipus _char_ de la següent manera:
```
char c = 'a', c1 = 1;
```

L'objectiu d'aquest exercici és assignar el valor 'b' en una tercera variable de tipus _char_, però sense usar el literal 'b', sinó fent la suma de les variables c i c1, és a dir:
```
char c2 = c + c1;
```

Què està passant? Com ho podem solucionar per tal d'aconseguir l'objectiu d'aquest exercici?

//TODO

#### Pregunta 9

Executa la següent expressió i assigna-la a una variable h:
```
var h = 4 * 4f + (4.0 + 4);
```

Ara, assigna el valor guardat a la variable h, a una altra variable de tipus _float_:
```
float f = h;
```

Què obtenim? Per què?

//TODO

Ara escriu el canvi que cal fer en l'expressió inicial (_4 * 4f + (4.0 + 4)_) per tal que l'assignació del valor d'h a f sigui reeixit.

//TODO

#### Pregunta 10

A partir de les següents variables i assignacions:
```
byte b0 = 4, b1 = -4, b2 = 12;
```

Executa el següent codi:
```
boolean bol1 = b0 == b2 / 3;
boolean bol2 = b0 + b1;
boolean bol3 = b0 + b1 > b2;
```

Explica el resultats obtinguts en cada cas:

//TODO

## DATA LÍMIT DE LLIURAMENT: DIMARTS 26 DE NOVEMBRE DE 2019
