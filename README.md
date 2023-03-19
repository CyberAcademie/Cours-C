Bienvenue au cours de base du langage C. Dans ce cours, nous allons apprendre les concepts fondamentaux du C et comment les utiliser pour créer des programmes efficaces. Nous allons couvrir les sujets suivants:

1.  Introduction à C
2.  Types de données en C
3.  Variables et constantes
4.  Opérateurs en C
5.  Instructions de contrôle de flux
6.  Fonctions en C
7.  Tableaux et chaînes de caractères
8.  Pointeurs en C
9.  Allocation dynamique de mémoire en C
10. Syntaxe de base en C

**Introduction à C**

C est un langage de programmation de haut niveau qui a été développé à Bell Labs dans les années 1970. Il est considéré comme l'un des langages les plus influents de l'histoire de l'informatique en raison de sa grande utilité et de son impact sur le développement de nombreux autres langages de programmation.

Le langage C est un langage de programmation structuré et impératif, ce qui signifie que les programmes écrits en C sont exécutés dans un ordre séquentiel et contrôlés par des instructions de contrôle de flux telles que les instructions conditionnelles et les boucles.

**Types de données en C**

En C, il existe plusieurs types de données que vous pouvez utiliser pour stocker des informations dans votre programme. Les types de données les plus courants sont:

・int (entier): pour stocker des nombres entiers

・float (flottant): pour stocker des nombres à virgule flottante

・char (caractère): pour stocker des caractères

・double (double précision flottant): pour stocker des nombres à virgule flottante avec une précision accrue

・short (entier court): pour stocker des nombres entiers courts

・long (entier long): pour stocker des nombres entiers longs

**Variables et constantes**

Les variables sont des espaces de stockage nommés dans la mémoire de l'ordinateur que vous pouvez utiliser pour stocker des informations dans votre programme. Les constantes, quant à elles, sont des valeurs fixes qui ne peuvent pas être modifiées pendant l'exécution du programme.

En C, vous pouvez déclarer une variable en utilisant le type de données approprié et un nom de variable. Par exemple:

```c
int age;
float temperature;
char lettre;
``` 
Les constantes peuvent être déclarées en utilisant le mot-clé "const". Par exemple:
 
```c
const int ANNEE = 2023;
const float PI = 3.14159;
const char NOUVELLE_LIGNE = '\n';
``` 

**Opérateurs en C**

Les opérateurs en C sont des symboles qui effectuent des opérations sur les données. Les opérateurs les plus couramment utilisés sont:

・Opérateurs arithmétiques: + (addition), - (soustraction), * (multiplication), / (division), % (modulo)

・Opérateurs de comparaison: == (égal à), != (différent de), < (inférieur à), > (supérieur à), <= (inférieur ou égal à), >= (supérieur ou égal à)

・Opérateurs logiques: && (et), || (ou), ! (non)

**Instructions de contrôle de flux**

Les instructions de contrôle de flux vous permettent de contrôler le flux d'exécution de votre programme en utilisant des structures conditionnelles et des boucles. Les structures conditionnelles vous permettent d'exécuter des instructions en fonction de certaines conditions. Les boucles vous permettent de répéter des instructions plusieurs fois.

Les instructions conditionnelles les plus couramment utilisées en C sont:

・if: exécute des instructions si une condition est vraie

・else: exécute des instructions si une condition est fausse

・else if: exécute des instructions si une autre condition est vraie

Par exemple:

```c
int age = 25;

if(age >= 18) {
  printf("Vous êtes majeur");
} else {
  printf("Vous êtes mineur");
}
```
Les boucles les plus couramment utilisées en C sont:

・for: répète un bloc d'instructions un certain nombre de fois

・while: répète un bloc d'instructions tant qu'une condition est vraie

・do-while: répète un bloc d'instructions au moins une fois, puis continue à le répéter tant qu'une condition est vraie

Par exemple:

```c
int i;

for(i=0; i<10; i++) {
  printf("%d ", i);
}

int j = 0;

while(j<10) {
  printf("%d ", j);
  j++;
}

int k = 0;

do {
  printf("%d ", k);
  k++;
} while(k<10);
```
**Fonctions en C**

Les fonctions en C sont des blocs de code qui peuvent être appelés à partir d'autres parties de votre programme. Les fonctions sont utiles pour réutiliser du code et pour organiser votre programme en blocs plus petits et plus facilement gérables.

Une fonction en C se compose d'une signature de fonction et d'un bloc de code. La signature de la fonction spécifie le type de données que la fonction renvoie (ou void si elle ne renvoie rien), ainsi que les paramètres d'entrée de la fonction.

Par exemple:

```C
int addition(int a, int b) {
  return a+b;
}
```
Cette fonction prend deux entiers en entrée et renvoie leur somme.

**Tableaux et chaînes de caractères**

Les tableaux et les chaînes de caractères sont des structures de données utiles en C pour stocker plusieurs valeurs dans une seule variable.

Un tableau est une collection ordonnée d'éléments du même type. Vous pouvez accéder à chaque élément du tableau en utilisant son indice.

Par exemple:
```C
int tableau[5] = {1, 2, 3, 4, 5};

printf("%d", tableau[2]); // affiche 3
```
Une chaîne de caractères est une collection de caractères terminée par un caractère nul ('\0'). Les chaînes de caractères sont souvent utilisées pour stocker du texte dans un programme.

Par exemple:
```C
char nom[10] = "UtiliseMan";
printf("%s", nom); // affiche "UtiliseMan"
```
**Pointeurs en C**

Les pointeurs en C sont des variables qui contiennent l'adresse d'une autre variable. Les pointeurs sont utiles pour manipuler des données en mémoire et pour allouer de la mémoire dynamiquement.

Pour déclarer un pointeur en C, utilisez l'opérateur * suivi du nom de votre pointeur. Pour accéder à la valeur de la variable pointée, utilisez l'opérateur * avant le nom de votre pointeur.

Par exemple: 
```C
int nombre = 42;
int *pointeur = &nombre;

printf("%d", *pointeur); // affiche 42
```
Dans cet exemple, nous déclarons une variable "nombre" avec la valeur 42. Nous déclarons ensuite un pointeur "pointeur" qui pointe vers la variable "nombre". En utilisant l'opérateur * devant le nom de notre pointeur, nous accédons à la valeur de la variable pointée.

**Allocation dynamique de mémoire en C**

L'allocation dynamique de mémoire en C vous permet d'allouer de la mémoire à un programme en cours d'exécution. C'est utile lorsque vous ne connaissez pas à l'avance la taille de la mémoire dont vous avez besoin.

La fonction "malloc" en C vous permet d'allouer de la mémoire dynamiquement. La fonction "free" vous permet de libérer la mémoire allouée dynamiquement.

Par exemple:
```C
int *tableau = malloc(5 * sizeof(int));

tableau[0] = 1;
tableau[1] = 2;
tableau[2] = 3;
tableau[3] = 4;
tableau[4] = 5;

free(tableau);
```
Dans cet exemple, nous allouons de la mémoire pour un tableau d'entiers de taille 5 à l'aide de la fonction "malloc". Nous initialisons ensuite chaque élément du tableau avec une valeur. Enfin, nous libérons la mémoire allouée avec la fonction "free".

**Syntaxe de base en C**

La syntaxe de base en C est relativement simple. Elle se compose d'une série d'instructions qui sont exécutées dans l'ordre dans lequel elles sont écrites. Les instructions sont généralement séparées par des points-virgules (;). Voici un exemple de programme C qui affiche "Hello, World!" à l'écran :
```C
#include <stdio.h> // directive de préprocesseur

int main() // fonction principale
{
    printf("Hello, World!"); // instruction d'affichage
    return 0; // instruction de retour
}
```
Dans ce programme, la directive de préprocesseur `#include <stdio.h>` permet d'inclure la bibliothèque standard `stdio.h`, qui contient les définitions de fonctions d'entrée/sortie standard.

La fonction `main()` est la fonction principale du programme. Tous les programmes en C doivent avoir une fonction `main()`, qui est appelée automatiquement au démarrage du programme. Cette fonction doit être définie avec un type de retour `int`.

Dans la fonction `main()`, l'instruction `printf("Bonjour, monde!");` affiche le message "Bonjour, monde!" à l'écran. La fonction `printf()` est une fonction d'entrée/sortie standard qui permet d'afficher des données à l'écran.

Enfin, l'instruction `return 0;` indique la fin du programme et renvoie une valeur de 0 à l'ordinateur. Cette valeur de retour est généralement utilisée pour indiquer si le programme s'est exécuté avec succès ou non.

Voici un exemple d'exercice pour pratiquer la syntaxe de base en C :

Exercice : Écrivez un programme en C qui demande à l'utilisateur de saisir son nom et qui affiche "Bonjour, [nom]!" à l'écran.

Voici une solution possible à cet exercice :

#include <stdio.h>
```C
int main()
{
    char nom[50];

    printf("Entrez votre nom : ");
    scanf("%s", nom);
    printf("Bonjour, %s!\n", nom);

    return 0;
}
```
Dans ce programme, la fonction `main()` demande à l'utilisateur de saisir son nom en utilisant la fonction `scanf()`, qui permet de lire des données depuis l'entrée standard. Le nom est stocké dans un tableau de caractères de taille 50 appelé `nom`.

Ensuite, le programme affiche le message "Bonjour, [nom]!" à l'écran en utilisant la fonction `printf()`, qui permet d'afficher des données à l'écran. Le `%s` dans le format de chaîne est remplacé par le contenu de la variable `nom`.

Enfin, le programme se termine avec l'instruction `return 0;`.

**Vous avez aussi à votre disposition des exercices, qui vous feront avancer en C.**
**Les exercices présentés viennent de la Piscine de** [42](https://42.fr/)
[EXERCICE](https://github.com/CyberAcademie/Cours-C/tree/main/Exercice%2C%20Piscine%2042%20%20(%20C%20))

Résumé : Ce cours de bases du C présente les concepts fondamentaux de la programmation en C, y compris la syntaxe de base, les types de données, les opérateurs, les structures de contrôle, les fonctions, les pointeurs et l'allocation dynamique de mémoire. Il est important de suivre les bonnes pratiques de programmation et de tester soigneusement votre code en raison de la nature bas niveau de la langue. La pratique régulière est essentielle pour améliorer vos compétences en programmation en C. `0x470, Cyber Academie`.
