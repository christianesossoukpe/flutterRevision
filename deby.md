Séance de revision Dart(2024-10-15 "session matinale").
Formatteur : Tiburce K.

### declaration de variables
numbers:
num y=55;
int x =2;=entier
double e = 1.55;=decimal

### log flutter
print();

### string(chaine de caractère)
** String txt = "hello";
  String tt = "salut sur une place. $txt"; // concatenation
boolean

##  list(array) **:
List<String>s2 =["tabi","agui"];
    print(s2.last);
    print(s2.first);
      print("le tableau $s2 contient  ${s2.length} elements.");

### set
elements unique ,ne se duplique pas.
Set<int> s3 = [1,2,3,2,3,4,5]"le set supprime les doublons d'un tableau "

### map
ensemble de clé _valeur = tout type(string ,number).
les clés sont uniques.
## null
variable qui peut etre null:


#### const bs final
const: utillisé pour lees constantes dont la valeur est determin"é à la compilation
les simples types de variables_

final : utilisé pour les constantes dont lavaleur ne peut etre determine que pendant l'execution du code.

** date,heure **
            final date = DateTime.now();
  print(date);

###  Fonctions
En dart, vous ne pouvez pas utiliser la syntaxe flèchée "=>" , car elle est reservée aux fonctions qui ont une seule expression.

@@ Parametres positionnels
int mult(int a, int b, int c){
    return a*b*c;
}

@@ Parametres nommés
int mult({int a =4, int b =5, int c = 5}) {
  return a * b * c;
}
