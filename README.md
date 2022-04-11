<!--
2022-04-11.12:46:15, Création :
    ~/prj/20200626.taxonomie-matrices-carrees/README.md
-->

# Taxonomie des matrices carrée

- [Introduction](#introduction)
- [Contribution](#contribution)

## Introduction

L’algèbre linéaire est livrée avec un bestiaire de matrices dont les noms sont toujours intuitifs (diagonalisable, inversible, symétrique, diagonale, scalaire), ou pas (normale, idempotente, involutive, hermitienne, positive, …)  
En apprenant l’algèbre linéaire, on a l’impression que ce bestiaire est un ensemble fourre-tout de matrices aux propriétés diverses et sans structure globale (du moins pour mon expérience).  
Cette impression s’estompe quand on découvre l’excellent diagramme suivant dans l’article [*List of named matrices*](https://en.wikipedia.org/wiki/List_of_named_matrices) de la wikipédia anglaise :

<p align="center">
  <img
    src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d1/Taxonomy_of_Complex_Matrices.svg/800px-Taxonomy_of_Complex_Matrices.svg.png"
    alt="Taxonomie des matrices complexes, Wikipédia"
  />
</p>

Ce diagramme est une version plus exhaustive et détaillé de ce dernier.

Ces diagrammes sont inspirés des [diagrammes de classes](https://fr.wikipedia.org/wiki/Diagramme_de_classes) de la [programmation orientée objets](https://fr.wikipedia.org/wiki/Programmation_orient%C3%A9e_objet), cette inspiration est pertinente car il y a une forte analogie entre [inclusion](https://fr.wikipedia.org/wiki/Inclusion_%28math%C3%A9matiques%29) et [héritage](https://fr.wikipedia.org/wiki/H%C3%A9ritage_%28informatique%29) :

|                        Héritage de classes                        |              Inclusion d’ensembles             |
|:-----------------------------------------------------------------:|:----------------------------------------------:|
|                    `A <- B` : `B` hérite de `A`                   |              `A <- B` : *A* ⊃ *B*              |
|           `b = B()` possède les attributs de `A` et `B`           | *B* ∋ *b* possède les propriétés de *A* et *B* |
| Il y a moins de trucs représentés par `B` que `A`<sup>**1**</sup> |           *B* est plus petit que *A*           |

[**1**]: Par exemple avec `Vehicules <- Train`, il existe moins de trains que de véhicules.

La notion importante et commune est que si `A <- B`, alors `B` possède plus de propriétés/attributs que `A` ; et par conséquent représente une population/ensemble/… plus petit.


## Contribution

J’ai réalisé ce diagramme avec l’excellent logiciel [IPE](https://ipe.otfried.org/) (développé intégralement en C++ par *Otfried Cheong*, [otfried/ipe](https://github.com/otfried/ipe)).  
En gros, c’est un *Inkscape* léger et modal, il gère nativement le LaTeX et est idoine pour ce genre de diagrammes.

Tout commentaire, proposition d’amélioration, ajout, etc. est bienvenu 🤓 !
