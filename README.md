[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-c66648af7eb3fe8bc4f294546bfd86ef473780cde1dea487d3c4ff354943c9ae.svg)](https://classroom.github.com/online_ide?assignment_repo_id=8409768&assignment_repo_type=AssignmentRepo)
Yanis  Mansouri

1.	Avec la commande which nous pouvons trouver le chemins d’accès au commandes exécutables
2.	On peut recherchez un terme spécifique avec : /nom_rechercher
3.	Avec la touche q nous pouvons quitter le manuelle immédiatement
4.	L’introduction de la section 6 nous informe que des jeux et des programmes de jeux sont disponible sur le système
5.	On ne peut pas accéder au dossier root pour des problèmes de permissions
6.	Nous n’avons pas accès à cette commande car nous somme pas connecter en tant que ‘admin’ donc nous avons pas les droit pour utiliser les commande sudo.
7.	 Le fichier a été supprimer avec succès alors que le dossier 1 ne peut pas être supprimer car c’est un dossier vide.
8.	Pour le supprimer il faut utiliser la commande rmdir.
9.	Cette commande ne marche pas sur le dossier 2 car celui-ci n’est pas vide.
10.	Pour supprimer un dossier et son contenue il faut utiliser la commande rm -r nom_dossier.

Commandes importantes
1	Nous pouvons afficher la date avec la commande : date. L’une des fonctionnalités de la commande time est de nous indiquer le temps de la réalisation d’une commande.
2	La commande ‘la’ permet de lister les fichiers dit cacher, les fichiers cacher commence par un point
3	Le programmes ls si situe dans /usr/bin/ls

4	Il n’existe pas de manuel pour la commande ‘ll’, la commande alias permet de retrouver la commande d’origine.

5	La commande ls /bin permet d’afficher les différents fichiers.

6	La commande ls . .  permet d’afficher le contenu du dossier n-1

7	La commande pwd permet d’afficher le chemin du dossier courant.

8	echo 'bip' > plop permet de crée un fichier s’intitulent plop avec comme contenue bip, réaliser une seconde fois le fichier sera écraser et le contenue mis à jour avec la nouvelle commande.

9	echo 'bip' >> plop cette commande permet de crée un fichier et de  rajouter du contenue sans écraser l’ancien si celle-ci est exécuter plusieurs fois.

10	sleep 10 | echo 'toto' elle impose un temps en secondes avant l’exécutions total de la commande

11	file permet de nous afficher le type du fichier demander

12	En modifiant le fichier original le fichier lien_phy subit les mêmes modifications, une fois le fichier original supprimer, le fichier lien_phy subit aucune modification.

13	Les fichiers sont mis à jour si l’un de ses fichier subit une modification, en supprimant le fichier lien_phy, le fichier lien_sym devient inutilisable.

14	Le combo ctrl + s permet de stopper le défilement des logs

15	Pour afficher un certain nombvre de ligne il faut utiliser tail –nx /var/log/syslog.

16	dmesg | less cette commande permet de voir les message du tampon circulaire du noyau



17	Cette commande permet d’afficher différentes informations sur un utilisateur comme son login, son mot de passe remplacer par un x, l'identifint du systeme de l'utilisateur, le groupe principal de l'utilisateur, un commentaire textuelle sur l'utilisateur(Nom et Prénom par exemple), le répertoire home de l'utilisateur sur le système  et l'interpréteur shell par défaut de l'utilisateur. la commande pour le manuelle est man 5 passwd

18	

19	Il y’a 34 utilisateur, on peut le savoir avec la commande wc –l /etc/passwd

20	il y'a 141 page de manuel disponible pour le mot conversion. La commande est la suivante man -k conversion | wc -l

21 On peut compter 17 fichierss passwd avec la commande sudo find / type -f -name 'passwd' | wc -l
22 
23
24 le fichier history.log se trouvre dans l'arboressance suivant /var/log/apt/history.log
25 Cela ne marche pas car la bdd n'est pas a jour, celle-ci sera a jour a 7h30 du matin si les machines sont allumér sinon 5 minutes apres le demarrage de la machine
 
Exercice 3

2.La combinaison est ctrl +alt + 8 :
 ![image](https://user-images.githubusercontent.com/77662970/189535280-39e4c73f-1135-4c94-8ac8-4a2d4c0bcf22.png)
  
  
  
3 Dans un premier tamps on selection les 10 premieres lignes avec alt + a, ensuite on les coupe avec ctrl +k ensuite on se place a la fin du fichier avec alt + shift + / ce qui nous emmene a la fin du fichier, on colle les 10 lignes avec ctrl + u.

4 Pour annuler les anciennes action on fait alt + u

5 On enregistre avec crtl +s et on quitte avec crtl + x



Exercice 4 

