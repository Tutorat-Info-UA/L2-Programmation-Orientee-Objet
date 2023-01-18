
_Tous les codes pourront être en Java ou LOLO celon vos préférences_
# ⚔️  TP - RPG  ⚔️  

## 1️⃣
Une Arme est un objet avec un poids une valeur de dégâts physique et une puissance magique qui sont des valeurs entières, un constructeur permettra en plus de construire des objets de cette classe en initialisant tous les champs. Fournir le code correspondant.

## 2️⃣
```txt 
┌———————————————————————————┐
│ Personnage                │
├———————————————————————————┤
│ vie :entier               │
│ vie_max :entier           │
│ arme :Arme                │
├———————————————————————————┤
│ Personnage(entier,entier) │ 
│ attaquer(Personnage):void │ 
│ encaisser(entier):void    │ 
│ equipper(Arme):void       │
│ toString():String         │
│ vivant():booléen          │
└———————————————————————————┘
```
> Le champ `arme` sera initialisé à `null` en Java.

> `attaquer` fait encaisser 1 dégats sur le personnage en paramètre.

> `encaisser` retranche de la vie au joueur.

> `equipper` change l'arme courante

>  `vivant` indique si la vie est supérrieur à 0

Fournir le code complet de cette classe


## 3️⃣
Un Guerrier est une sorte de personnage qui peut utiliser une arme pour ajouter ces dégâts physique lors d'une attaque. Fournir le code de la classe.

## 4️⃣
Un Berserk est une sorte de guerrier qui fait deux fois plus de dégâts s'il est à moins de 20% de ses points de vie. Fournir le code de la classe.

## 5️⃣
Un Paladin est un guerrier qui a une chance sur deux de bloquer une attaque et donc de ne pas subir des dégâts. Fournir le code de la classe.

## 6️⃣
Un Mage est un personnage qui utilise une arme pour ajouter des dégâts magique s'il a encore de la mana et une attaque retire `1` de mana, il a aussi deux attributs suplémentaire qui sont `mana` et `mana_max` qui sont des entiers à initialiser. Fournir le code de la classe.

## 7️⃣
Un Archimage est un mage qui peut absorber une attaque avec 10% de chance, il ne subira alors aucun dégât qui seront reporté dans un champ `buffer` à créer qui sera de base à 0. Lorsqu'il attaque le `buffer` est remis à 0 et la valeur est ajouter au dégâts de l'attaque.

## 8️⃣
Fournir un schéma (UML si vous le pouvez, sinon semblable à la question 2) des classes des précédentes questions.

## 9️⃣
Faire un programme principal d'un combat entre deux joueurs et afficher les informations dans le terminal, en Java on aura pour base :
```java

public class Arene {
	public void main() {
		// Votre code ici...
	}
}
```

## *️⃣
Pour la partie aléatoire, la fonction `Math.random()` retourne un nombre aléatoire entre 0 et 1, si on a donc besoin d'un tirage à 75% on fera :
```java
if( Math.random() < 0.75 ) {
	// ...
}
```