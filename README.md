

Yanis  Mansouri

# Exercice 2. Prise en main de l’interpréteur de commandes

# Manuel

## 1. A l’aide du manuel, identifiez le rôle de la commande which
Avec la commande which nous pouvons trouver le chemins d’accès au commandes exécutables
## 2. Quand on consulte une page du manuel, comment peut-on rechercher un terme (par exemple, chercher
le terme option dans la page de manuel de which ?
On peut recherchez un terme spécifique avec : /nom_rechercher
## 3.	Comment quitte-t-on le manuel ?
Avec la touche q nous pouvons quitter le manuelle immédiatement
## 4. Chaque section du manuel a une première page, qui présente le contenu de la section. Afficher la
première page de la section 6 ; de quoi parle cette section ?
L’introduction de la section 6 nous informe que des jeux et des programmes de jeux sont disponible sur le système

# Navigation dans l’arborescence des fichiers
## 1. allez dans le dossier /var/log
```
cd /vag/log
```
## 2. remontez dans le dossier parent (/var) en utilisant un chemin relatif
```
cd ..
```
## 3. retournez dans le dossier personnel
```
cd
```
## 4. revenez au dossier précédent (/var) sans utiliser de chemin
```
cd -
```
## 5.	essayez d’accéder au dossier /root ; que se passe-t-il ?
On ne peut pas accéder au dossier root pour des problèmes de permissions
## 6. essayez la commande sudo cd /root ; que se passe-t-il ? Expliquez
Nous n’avons pas accès à cette commande car nous somme pas connecter en tant que ‘admin’ donc nous avons pas les droit pour utiliser les commande sudo.
## 8.	revenez dans votre dossier personnel ; à l’aide de la commande rm, essayez de supprimer Fichier1, puis
Dossier1 ; que se passe-t-il ?
Le fichier a été supprimer avec succès alors que le dossier 1 ne peut pas être supprimer car c’est un dossier vide.
## 9.	quelle commande permet de supprimer un dossier ?
Pour le supprimer il faut utiliser la commande rmdir.
## 10. que se passe-t-il quand on applique cette commande à Dossier2 ?
Cette commande ne marche pas sur le dossier 2 car celui-ci n’est pas vide.
## 11. comment supprimer en une seule commande Dossier2 et son contenu ?
Pour supprimer un dossier et son contenue il faut utiliser la commande rm -r nom_dossier.

# Commandes importantes
## 1. Quelle commande permet d’afficher l’heure ? A quoi sert la commande time ?
Nous pouvons afficher la date avec la commande : date. L’une des fonctionnalités de la commande time est de nous indiquer le temps de la réalisation d’une commande.
## 2. Dans votre dossier personnel, tapez successivement les commandes ls puis la ; que peut-on en déduire
sur les fichiers commençant par un point ?
La commande ‘la’ permet de lister les fichiers dit cacher, les fichiers cacher commence par un point
## 3. Où se situe le programme ls ?
Le programmes ls si situe dans /usr/bin/ls
## 4. Essayez la commande ll. Existe-t-il une entrée de manuel pour cette commande ? Utilisez les commandes alias ou alias pour en savoir plus sur la nature de cette commande.
Il n’existe pas de manuel pour la commande ‘ll’, la commande alias permet de retrouver la commande d’origine.
## 5. Quelle commande permet d’afficher les fichiers contenus dans le dossier /bin ?
La commande ls /bin permet d’afficher les différents fichiers.
## 6. Que fait la commande ls .. ?
La commande ls . .  permet d’afficher le contenu du dossier n-1
## 7. Quelle commande donne le chemin complet du dossier courant ?
La commande pwd permet d’afficher le chemin du dossier courant.
## 8. Que fait la commande echo 'bip' > plop exécutée 2 fois ?
echo 'bip' > plop permet de crée un fichier s’intitulent plop avec comme contenue bip, réaliser une seconde fois le fichier sera écraser et le contenue mis à jour avec la nouvelle commande.
## 9. Que fait la commande echo 'bip' >> plop exécutée 2 fois ?
echo 'bip' >> plop cette commande permet de crée un fichier et de  rajouter du contenue sans écraser l’ancien si celle-ci est exécuter plusieurs fois.
## 10.	Interprétez le comportement de la commande sleep 10 | echo 'toto' ?
sleep 10 | echo 'toto' elle impose un temps en secondes avant l’exécutions total de la commande
## 11. A quoi sert la commande file ? Essayez la sur des fichiers de types différents
file permet de nous afficher le type du fichier demander
## 12.	Créez un fichier original qui contient la chaîne Hello Toto ! ; créer ensuite un lien lien_phy vers
ce fichier avec la commande ln original lien_phy. Modifiez à présent le contenu de original et
affichez le contenu de lien_phy : qu’observe-t-on ? Supprimez le fichier original ; quelle conséquence
cela a-t-il sur lien_phy ?
En modifiant le fichier original le fichier lien_phy subit les mêmes modifications, une fois le fichier original supprimer, le fichier lien_phy subit aucune modification.
## 13.	Créez à présent un lien symbolique lien_sym sur lien_phy avec la commande ln -s lien_phy lien_sym.
Modifiez le contenu de lien_phy ; quelle conséquence pour lien_sym ? Et inversement ? Supprimez le
fichier lien_phy ; quelle conséquence cela a-t-il sur lien_sym ?
Les fichiers sont mis à jour si l’un de ses fichier subit une modification, en supprimant le fichier lien_phy, le fichier lien_sym devient inutilisable.
## 14.	. Affichez à l’écran le fichier /var/log/syslog. Quels raccourcis clavier permettent d’interrompre et
reprendre le défilement à l’écran ?
Le combo ctrl + s permet de stopper le défilement des logs
## 15.	Affichez les 5 premières lignes du fichier /var/log/syslog, puis les 15 dernières, puis seulement les
lignes 10 à 20.
Pour afficher un certain nombvre de ligne il faut utiliser tail –nx /var/log/syslog.
## 16.	Que fait la commande dmesg | less ?
dmesg | less cette commande permet de voir les message du tampon circulaire du noyau
## 17.	Affichez à l’écran le fichier /etc/passwd ; que contient-il ? Quelle commande permet d’afficher la page
de manuel de ce fichier ?
Cette commande permet d’afficher différentes informations sur un utilisateur comme son login, son mot de passe remplacer par un x, l'identifint du systeme de l'utilisateur, le groupe principal de l'utilisateur, un commentaire textuelle sur l'utilisateur(Nom et Prénom par exemple), le répertoire home de l'utilisateur sur le système  et l'interpréteur shell par défaut de l'utilisateur. la commande pour le manuelle est man 5 passwd
## 19.	Quelle commande nous donne le nombre d’utilisateurs ayant un compte sur cette machine (pas seulement les utilisateurs connectés) ?
Il y’a 34 utilisateur, on peut le savoir avec la commande wc –l /etc/passwd

## 20.	Combien de pages de manuel comportent le mot-clé conversion dans leur description ?
il y'a 141 page de manuel disponible pour le mot conversion. La commande est la suivante man -k conversion | wc -l
## 21. A l’aide de la commande find, recherchez tous les fichiers se nommant passwd présents sur la machine
On peut compter 17 fichierss passwd avec la commande sudo find / type -f -name 'passwd' | wc -l
## 22. Modifiez la commande précédente pour que la liste des fichiers trouvés soit enregistrée dans le fichier
~/list_passwd_files.txt et que les erreurs soient redirigées vers le fichier spécial /dev/null
Pour enregistré des fichiers trouvé dans un fichier précis il faut faire " find / -iname "passwd" >> list_passwd_files.txt ". Pour redirifer les erreurs la commande est " find / -iname "passwd" 2>> /dev/null "
## 24. Utilisez la commande locate pour trouver le fichier history.log.
le fichier history.log se trouvre dans l'arboressance suivant /var/log/apt/history.log
## 25. Créer un fichier dans votre dossier personnel puis utilisez locate pour le trouver. Apparaît-il ? Pourquoi ?
Cela ne marche pas car la bdd n'est pas a jour, celle-ci sera a jour a 7h30 du matin si les machines sont allumér sinon 5 minutes apres le demarrage de la machine.
 
# Exercice 3. Découverte de l’éditeur de texte nano

## 2.La combinaison est ctrl +alt + 8 :
 ![image](https://user-images.githubusercontent.com/77662970/189535280-39e4c73f-1135-4c94-8ac8-4a2d4c0bcf22.png)
  
  
## 3. Déplacer les 10 premières lignes à la fin du fichier
Dans un premier tamps on selection les 10 premieres lignes avec alt + a, ensuite on les coupe avec ctrl +k ensuite on se place a la fin du fichier avec alt + shift + / ce qui nous emmene a la fin du fichier, on colle les 10 lignes avec ctrl + u.
## 4. Annulez cette action
 Pour annuler les anciennes action on fait alt + u
## 5. Enregistrez le fichier avant de quitter nano
 On enregistre avec crtl +s et on quitte avec crtl + x

# Exercice 4 

## 1.Commencez par créer une copie de ce fichier, que vous appellerez .bashrc_bak 
Pour copier le fichier on utilise la commande ```cp``` suivie par le fichier cible et le nom de la copie

## 2.Editez le fichier .bashrc avec nano et décommentez la ligne force_color_prompt=yes pour activer
la couleur. Enregistrez le fichier et quittez nano

![image](https://user-images.githubusercontent.com/77662970/194298540-aae3d863-4fc5-4408-b94c-e2fcf8b1257c.png)

## 4.Les couleurs par défauts (surtout celle du dossier courant) ne sont pas très visibles. Dans .bashrc,
cherchez les lignes commençant par PS1= ; elles indiquent la mise en forme de l’invite de commande
(selon que l’on est en couleurs ou non).
Sur cette ligne, on peut distinguer un certain nombre de raccourcis :

![image](https://user-images.githubusercontent.com/77662970/194298770-90e9a301-948a-4e90-9db4-44a1d90c7f08.png)
## Résultat
![image](https://user-images.githubusercontent.com/77662970/189540480-3f467930-542f-4998-b6d7-de174be09d7e.png)

