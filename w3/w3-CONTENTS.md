## Vidéo 1 (Les fichiers)
### NIVEAU: BASIC
### Compléments Vidéo 1
* parler de l'encodage des fichiers et du lien avec str et bytes
  (j'en parle rapidement dans la vidéo, mais il faut plus
  d'exemple).

Pour mémoire, notebook du précédent MOOC sur Python 2

* `Complement-fichiers.ipynb`
* `Complement-utilitaires-sur-fichiers.ipynb`
* `Complement-format-json-et-autres.ipynb` : parler de json, pickle,
  csv ...
* `Complement-fichiers-systeme.ipynb` :
* DROPPED *montrer que sys.stdout n'est qu'une variable qui peut référencer un autre fichier.
  Comme print écrit dans sys.stdout, c'est un moyen simple de rediriger
  les print vers un fichier. (c'est très sale cette façon de faire..)

## Quizz Vidéo 1

## Exercices Vidéo 1

* `Exercice-fichiers.ipynb`


## Vidéo 2 (Les tuples)
### NIVEAU: BASIC
### Compléments Vidéo 2
* extended sequence unpacking - montrer qu'on peut mettre des trucs au début ou à la fin mais qu'on ne doit mettre qu'un seul *arg
* xxx un complément sur `namedtuple`

Pour mémoire, notebook du précédent MOOC sur Python 2

* `Complement-tuple-et-virgule.ipynb` : les différentes syntaxes (avec ou sans parenthèses, avec ou sans virgule terminale
xxx ajouter ceci
il y a quelques contextes dans lesquels il faut mettre les parenthèses
x=1,
type(x)
type(1,)
type((1,))

* `Complement-sequence-unpacking.ipynb` :
  a,b = tuple
  je parle aussi de retrouver 3 dans ['abc', [(1,2), ([3], 4)], 5]
  xxx insister dans le extended unpacking, le fait qu'on peut mettre exactement une variable avec *

### Quizz Vidéo 2
Pour mémoire, quizz du précédent MOOC sur Python 2

* `W2-S5-E1-tuples.quiz`

### Exercices Vidéo 2
Pour mémoire, quizz du précédent MOOC sur Python 2


## Vidéo 3 (Tables de hash)
### NIVEAU: BASIC
### Compléments Vidéo 3
* donner des pointeurs vers le fonctionnement des tables de hash et
  la gestion des collisions. Donner également un pointeur vers
  l'implementation en Python des tables de hash.
  https://docs.python.org/3.6/faq/design.html#how-are-dictionaries-implemented

Pour mémoire, notebook du précédent MOOC sur Python 2

### Quizz Vidéo 3
Pour mémoire, quizz du précédent MOOC sur Python 2

### Exercices Vidéo 3
Pour mémoire, quizz du précédent MOOC sur Python 2


## Vidéo 4 (Les dictionnaires)
### NIVEAU: BASIC
### Compléments Vidéo 4
* faire un complément sur les objets hashable.  Partir de
  https://docs.python.org/3.6/glossary.html#term-hashable est de la
  fonction built-in hash
* parler des ordereddict
* est-ce que ça vaut le coup de parler de ça :
  https://docs.python.org/3/whatsnew/3.6.html#new-dict-implementation

* xxx il faudra vérifier qu'on dit bien quelque part
  qu'on ne peut pas modifier l'objet d'un for au milieu du for
  qui s'applique donc au dictionnaire

Pour mémoire, notebook du précédent MOOC sur Python 2

* `Complement-dictionnaires.ipynb` - recapitulatif sur comment
  utiliser un dict + url vers la doc python
* `Complement-cles-immuables.ipynb` - types immuables et clés
  globalement immuables
* `Complement-record-et-dictionnaire.ipynb` - une utilisation
  standard du dictionnaire pour faire un struct

### Quizz Vidéo 4

Pour mémoire, quizz du précédent MOOC sur Python 2

* `W3-S2-E1-dicts.quiz` - un quiz sur les dictionnaires

## Exercices Vidéo 4

Pour mémoire, quizz du précédent MOOC sur Python 2

* `Exercice-marine-dictionnaire.ipynb` - premier morceau de code un peu réel avec data/marine*.json -- assez simple - data et corrections


## Vidéo 5 (Les ensembles)
### NIVEAU: BASIC
### Compléments Vidéo 5

* introduire les frozensets (je n'en parle plus dans la vidéo)

Pour mémoire, notebook du précédent MOOC sur Python 2

* `Complement-ensembles.ipynb` : recap. fonctions/methodes sur les
   ensembles

### Quizz Vidéo 5

Pour mémoire, quizz du précédent MOOC sur Python 2

### Exercices Vidéo 5

Pour mémoire, quizz du précédent MOOC sur Python 2

* `Exercice-marine-ensembles.ipynb` - avec le même genre de données de marine traffic
* NICETOHAVE : un quiz qui met l'accent sur le choix judicieux du
  type de base en fonction du probleme posé entre tuple, liste,
  dict, set (et pourquoi pas aussi frozenset si il faut hacher)


## Vidéo 6 (Les exceptions)
### NIVEAU: BASIC
NOTE TP: cette liste semble concerner la vidéo, je sais pas si ça a été fait ou pas dans le scénario, je laisse tel quel

* parler de finally et else
* parler des arguments des exceptions avec une
  capture du style "except ZeroDivisionError as e"
* expliquer ce qu'est la pile d'exécution

## Compléments Vidéo 6

sujets possibles:

* module traceback; parler de la pile, montrer comment l'afficher
  donner la référence de la documentation de toutes les exceptions built-in
  https://docs.python.org/3/library/exceptions.html#bltin-exceptions
  et du tutorial Python sur les exceptions
  https://docs.python.org/3/tutorial/errors.html

  montrer except Exception as e:
     comme dernière clause pour tout attraper et montrer alors print_exc()

* assert

* NICETOHAVE un complement sur le debugger, la pile, traceback, etc.
  la pile; montrer la pile lorsqu'on attrape une exception
  pourquoi ne pas mentionner le debugger ?

* NICETOHAVE parler des Warning et du module warning ?
  https://docs.python.org/2.7/library/warnings.html#module-warnings

### Quizz Vidéo 6
Pour mémoire, quizz du précédent MOOC sur Python 2

### Exercices Vidéo 6
Pour mémoire, quizz du précédent MOOC sur Python 2


## Vidéo 7 (Les références partagées)
### NIVEAU: BASIC
### Compléments Vidéo 7
Pour mémoire, notebook du précédent MOOC sur Python 2

* `Complement-operateur-is-et-fonction-id.ipynb` : function id(), operateur is,  les entiers implementes comme des singletons
* `Complement-references-circulaires.ipynb` : une liste infinie; un exemple + utile de reference circulaire
* `Complement-les-differentes-copies.ipynb` - make sure this comes after is-id
* `Complement-instruction-del.ipynb` *del a;  del L[i:j:k]; del d[clef]
* `Complement-affectation-simultanee.ipynb`   a = b = []
* BOF gc.ipynb peut-etre plus tard mais je vois ca comme un truc super scabreux (si on veut le faire correctement)
  en plus sys.getrefcount c'est un detail d'implementation; je sais pas si pypy a ça par exemple
* BOF sys.getrefcount()

## Quizz Vidéo 7
Pour mémoire, quizz du précédent MOOC sur Python 2

* `W3-S4-E1-multiply.quiz` liste=[[1]]*5 et demander une solution
  pour ne pas avoir de ref. partagées  

### Exercices Vidéo 7
Pour mémoire, quizz du précédent MOOC sur Python 2

* DROPPED* exo pour voir jusqu'à quelle taille de chaîne de
  caractères (et quelle taille d'entier) Python arrête
  de faire des références partagées pour optimiser la
  mémoire.  je laisse tomber car la fonction
  is_singleton se comporte de maniere bizarre

* NICETOHAVE essayer d'écrire un bout de code buggé et
  demander aux gens detrouver l'erreur en rajoutant une
  copie


## Vidéo 8 (Introduction aux classes)
### NIVEAU: INTERMÉDIAIRE
### Compléments Vidéo 8
Pour mémoire, notebook du précédent MOOC sur Python 2

* **TODO** un notebook sur pathlib, permet de manipuler le filesystem avec des vraies classes par opposition au vieil os.path

### Quizz Vidéo 8
Pour mémoire, quizz du précédent MOOC sur Python 2

### Exercices Vidéo 8
Pour mémoire, quizz du précédent MOOC sur Python 2
