# design-Pattern-Strategy
Stratégie est un patron de conception comportemental qui permet de définir une famille d’algorithmes, de les mettre dans des classes séparées et de rendre leurs objets interchangeables.
 Design-Pattern-Strategy Le design pattern Strategy permet de définir une famille d'algorithme, d'encapsuler chacun et les rendre interchangeable tout en assurant que chaque algorithme puisse évolue indépendamment des clients qui l'utilisent

-- Raison d'utilisation: un objet doit pouvoir faire varier une partie de son algorithme dynamiquement 



Note: varier le comportement d'un objet de manière dynamique ne se fait qu'avec l'injection de dépendance.
====   varier = cahnger = passer a un autre. 


       la communication entre les Objets ne doit se faire qu'a travers l'injection de dépendance. 

--Résultat: le design pattern strategy permet d'isoler les algorithme  appartenant a une même famille  d'algorithme. 

--question 1: c'est quoi une famille d'algorithme?

--réponse: une famille d'algorithme est un ensemble d'algorithme qui permet de faire la même chose mais de manière différente par exemple la fonction Trier( nous avons différente version de trie => trie a bulle, Tri par tas (heap sort), Tri rapide (quicksort), Tri fusion (merge sort) ); Exemple2 fonction opération( nous avons différent algorithme opération => addition, soustraction, multiplication, division ). 

--Question 2: que veut dire encapsuler chacun(Tout ce qui est susceptible de changer encapsuler le!!)? 

--réponse: ça veut dire que chaque algorithme doit se trouver dans une classe séparer. 

--Question 3: que veut dire l'expression les rendre Interchangeable?

--réponse: ça veut tout simplement dire que le client a un moment donné(en cours d'exécution) ou bien une application peut basculer d'une version a une autre.

--Question: que veut dire les rendre Interchangeable?

--réponse: c'est le faite qu'ils implements une interface commun, et automatiquement tous c'est algorithmes peuvent être utilisé a travers l'interface.

--Particularité de ce design pattern  est d'encapsuler chaque algorithme dans des classes séparées . Chaqu'une des  classes ne devrais avoir que l'algorithme(une seul méthodes doit être présent dans chacune des classe ) à partir du moment ou vous avez deux méthodes dans une même classe => il ne s'agit plus d'une strategy   ça devient un autre DP.
Donc dans la classe il ne devrait avoir qu'une seul methodes, c'est ce qu'on appele design pattern Strategy.


--Par contre dans la logique des choses vous pouvez utiliser une classe Abstraite au lieu d'interface (strategy). Eventuellement quand vous utiliser une classe abstraite ce que vous pouvez ajouter des attributs(etc..) et dans si vous entrez dans cette logique ce que n'utilisez plus le DP strategy mais plûtot un autre pattern.
<<donc avec le DP strategy utilisez une interface qui contient une unique methodes>>.


inconvenients: l'inconvenient de ce DP est : il y'a beaucoup de classe et d'interface (l'explosion des nombre de classes).

NB: l'idéal, la meilleur conception que nous pouvons faire dans l'ingénierie logiciel c'est que chaques methodes doit-être dans une classe séparer.

