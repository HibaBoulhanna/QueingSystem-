# QueingSystem-
 Développement d'un simulateur flexible de réseaux de files d'attentes qui produit de la Data exploitable. • Etude de la performance du trafic sur différents horizons temporels. • Etude de la robustesse et la fiabilité des données produites via la réalisation des tests statistiques. • Calcul des métriques de dimensionnement &amp; Elaboration des visuels.  Langage utilisé : Python
Ce mini-projet consiste en la résolution du problème ci-après représentant un bureau de poste constitué de deux guichets. Pour cela décrivez comment fonctionne ce système en indiquant clairement quels sont les variables d'état et quels sont les événements. Aussi, pour chaque événement provoqué, indiquez clairement l’action que le modèle de simulation prendra (idéalement sous la forme d’un logigramme ou d’un pseudo-code).

Le rapport contient :

•	La liste des événements retenus et la logique globale de chaque événement. Fournir 
•	Le  logigramme du modèle de simulation.
•	Liste de toutes les variables utilisées en précisant la définition et le rôle de chacune d'elle.
•	Listing du programme de simulation.
•	La réponse aux questions, et les interprétations.

# # # # # # # # # # # #

Système à étudier :

Considérons un bureau de poste constitué de deux guichets (1 et 2) occupés respectivement par les employés E1 et E2. Deux catégories de clients (A et B) entrent dans ce bureau. Les autres caractéristiques de ce système ainsi constitué sont données ci-après :

•	Les clients A arrivent chez l’employé 1 avec un taux de λ1.
•	Les clients B arrivent chez l’employé 2 avec un taux de λ2.
•	Les arrivées chez les deux employés sont indépendantes.
•	Les taux de service sont µ1 et µ2, respectivement, pour l’employé 1 et pour l’employé 2.
•	Chaque client, de catégorie A, qui termine son service au guichet 1 quitte le système avec la probabilité p1. Il se dirige vers le guichet 2 - pour recevoir un deuxième service – avec la probabilité de 1-p1. Dans ce cas, il va rejoindre la dernière place dans la file du guichet 2.
•	Chaque client, de catégorie B, qui termine son service au guichet 2 quitte le système avec la probabilité p2. Il se dirige vers le guichet 1 - pour recevoir un deuxième service – avec la probabilité de 1-p2. Dans ce cas, il va rejoindre la dernière place dans la file du guichet 1.
•	La discipline est FIFO.
•	Chaque guichet a sa propre file d’attente.
•	La capacité de chaque file est infinie.

Ecrire un programme (Python ) pour simuler ce système. La fonction utilisée pour générer les temps inter-arrivée doit gérer, selon une loi Exponentielle, 
 
De même, pour  la fonction utilisée pour générer les temps de service.


•	Horizon de simulation : T=500 Unts de temps.
•	Les temps d'inter-arrivée sont exponentiels avec : λ1= 8 clients par heure, λ2= 17 clients par heure.
•	Les temps de service sont exponentiels avec : µ1 = 20 clients par heure, µ2 = 30 clients par heure.
•	Les probabilités de quitter le système sont : p1 = 0.5, p2 = 0.75.

Thèmes :

1)	Donner le taux d’occupation de chaque employé.
2)	Donner le nombre moyen de clients dans le système pour chaque catégorie.
3)	Donner le nombre moyen de clients dans chaque file d’attente.
4)	Donner la durée moyenne de séjour d'un client dans le système.
5)	Prendre T=4. Donner le graphique d’évolution du nombre de client dans le système en fonction du temps des deux catégories de clients : NA(t) et NB(t).
6)	Test sur les nombres générés par l’algorithme.
