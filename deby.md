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
element unique ,ne se duplique pas.
Set<int> s3 = [1,2,3,2,3,4,5]"le set supprime les doublons d'un tableau "

### map
ensemble de clé _valeur = tout type(string ,number).
les clés sont uniques.
## null
variable qui peut etre null:


#### const vs final
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

### class
void main() {
Point  somme = Point(2,5) ;
  print(somme.ages);
}

class Point{
  
//   String nom = "deby";
//   String prenom = "debyarah";
//   int  age = 50;
 
  int  ages ;
  int  note;
 Point(this.ages,this.note){
    
  }
}
<!-- constructeur par defaut -->


<!-- constructeur nommé -->
image.asset;
Point p1=Point(2,3);
Point p1=Point.origin();

<!-- constructeur standard -->
normal

### liste d'initialisation
Animal(int legs):this.legs=legs{}

ou ça( int legs;
  Animal(this.legs);)
### appel au constructeurs du parent
super();

void main() {
  Dog pattes = Dog();
  Bird pate = Bird();//instanciation de classe
  
  
  pate.makeNoise();//appel de la methode makeNoise de la classe Dog
  pattes.makeNoise();
  
  print(pate.fly());//appel de la methode fly de la classe Bird
  print(pattes.legs);
  print(pate.legs);
  
  
}

### 
// heritage de classe et instanciation

class Animal{
  
  int legs;
  
  makeNoise(){
    print('???');
  }  
  Animal(this.legs);
}

  class Dog extends Animal{
//   int legs;
        Dog():super(4);
    @override
    makeNoise(){
      print("woof");
    }
  }
  
 class Bird extends Animal{
//   int legs;
       Bird():super(2);
   @override
   makeNoise(){
     print("Chirp");
   }

   @override
   fly(){
     print("Flying");
   }
     
  }


### exercice
// ## Instructions :
// 1. Créez une classe `Animal` avec :

// - Un attribut `int legs` pour le nombre de pattes.
// - Une méthode `makeNoise()` qui affiche `'???'`.
// - Un constructeur qui prend le nombre de pattes en paramètre.

// 2. Créez deux sous-classes qui héritent de `Animal` :

// - **Dog** : Représente un chien.
//     - Le constructeur doit appeler le constructeur de la classe parente avec `4` pattes.
//     - La méthode `makeNoise()` doit afficher `'Woof'`.  
// - **Bird** : Représente un oiseau.
//     - Le constructeur doit appeler le constructeur de la classe parente avec `2` pattes.
//     - La méthode `makeNoise()` doit afficher 'Chirp'.
//     - Ajoutez une méthode spécifique à la classe Bird appelée `fly()`, qui affiche `'Flying!'`.

// 3. Créez un programme principal qui fait les choses suivantes :

//     - Crée un objet de type `Dog` et `Bird`.
//     - Affiche le nombre de pattes pour chaque animal.
// - Appelle la méthode `makeNoise()` pour chaque animal.
// - Appelle la méthode `fly()` pour l'objet `Bird` (et essayez de l'appeler pour `Dog` pour voir l'erreur de compilation).