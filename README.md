# design-Pattern-Strategy
Stratégie est un patron de conception comportemental qui permet de définir une famille d’algorithmes, de les mettre dans des classes séparées et de rendre leurs objets interchangeables.
 Design-Pattern-Strategy Le design pattern Strategy permet de définir une famille d'algorithme, d'encapsuler chacun et les rendre interchangeable tout en assurant que chaque algorithme puisse évolue indépendamment des clients qui l'utilisent

-- Raison d'utilisation: un objet doit pouvoir faire varier une partie de son algorithme dynamiquement 

--Résultat: le design pattern strategy permet d'isoler les algorithme  appartenant a une même famille   d'algorithme. 

--question 1: c'est quoi une famille d'algorithme?

--réponse: une famille d'algorithme est un ensemble d'algorithme qui permet de faire la même chose mais de manière différente par exemple la fonction Trier( nous avons différente version de trie => trie a bulle, Tri par tas (heap sort), Tri rapide (quicksort), Tri fusion (merge sort) ); Exemple2 fonction opération( nous avons différent algorithme opération => addition, soustraction, multiplication, division ). 

--Question 2: que veut dire encapsuler chacun(Tout ce qui est susceptible de changer encapsuler le!!)? 

--réponse: ça veut dire que chaque algorithme doit se trouver dans une classe séparer. 

--Question 3: que veut dire l'expression les rendre Interchangeable?

--réponse: ça veut tout simplement dire que le client a un moment donné(en cours d'exécution) ou bien une application peut basculer d'une version a une autre.

--Particularité de ce design pattern  est d'encapsuler chaque algorithme dans des classes séparées . Chaqu'une des  classes ne devrais avoir que l'algorithme(une seul méthodes doit être présent dans chacune des classe ) à partir du moment ou vous avez deux méthodes dans une même classe => il ne s'agit plus d'une strategy   ça devient un autre DP.
