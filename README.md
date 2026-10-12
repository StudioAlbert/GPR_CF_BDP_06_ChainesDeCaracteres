# Pseudo valide ? — companion GPR-CF-BDP-06

Ce que nous avons tapé **ensemble en classe** pour l'exercice 3 de la séance *Chaînes de
caractères*. Le squelette tourne : il lit un pseudo et refuse le vide. Les trois règles
suivantes restent à écrire.

## Compiler et lancer

```powershell
cmake -S . -B build
cmake --build build
```

Puis `build/Exercice_3/Exercice_3.exe`.

## Où en est le code

`Exercice_3/main.cc` contient la boucle de saisie et `checkEmpty`, qui couvre la première
règle. Le message qu'elle affiche (`xxxx = input is empty`) est celui du direct, pas celui
de l'énoncé : à remplacer.

| # | Règle | Message attendu | État |
|:-:|---|---|---|
| 1 | le pseudo n'est pas vide | `Refusé : le pseudo est vide.` | écrit, message à corriger |
| 2 | au moins **3** caractères | `Refusé : trop court, 3 caractères minimum.` | à faire |
| 3 | au plus **16** caractères | `Refusé : trop long, 16 caractères maximum.` | à faire |
| 4 | aucun espace | `Refusé : pas d'espace dans un pseudo.` | à faire |
| — | toutes les règles passent | `Bienvenue, Morgane !` | à faire |

Les règles se testent **dans cet ordre**, et on s'arrête à la première qui échoue.

## Vérifier que ça marche

Chacune de ces saisies doit donner un message différent :

```text
(ligne vide)          le pseudo est vide
Zo                    trop court
LeChevalierDuNordEst  trop long
Dark Sasuke           pas d'espace
Morgane               Bienvenue, Morgane !
```
