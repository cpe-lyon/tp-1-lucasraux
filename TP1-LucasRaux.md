##Tp 1 – Bash prise en main

#  Manuel
1.	La commande which permet de trouver le ou les chemins d’un exécutable dans les différents répertoires listés dans la variable PATH

2.	 Pour rechercher un terme dans un manuel on utilise la commande : man which /option

3.	Pour quitter le manuel on utilise la touche q

4.	La section 6 du manuel parle des jeux ainsi que les petits programs amusant disponibles sur le système avec la commande man 6 intro


# Navigation dans l'arborscence des fichiers

1.	Pour aller dans le dossier /var/log on utilise la commande cd /var/log

2.	Pou remonter dans le dossier parents on utilise la commande cd /var ou cd ..

3.	Pour retourner dans le dossier personnel on utilise la commande cd

4.	Pour revenir au dossier précédent on utilise la commande cd –

5.	On ne peut pas accéder au dossier root car nous n’avons pas les droits 

6.	La commande est introuvable, car il faut au préalable s’accorder les droits avec la commande sudo, puis exécutez la commande cd /root

7.  ddd

8.	Il est possible de supprimer le Fichier1, grâce à la commande rm Dossier1/Fichier1 mais il n’est pas possible de supprimer le Dossier1

9.	C’est la commande rmdir qui permet de supprimer un dossier à la condition qu’il soit vide

10.	Si on essaye la commande rmdir sur le Dossier2, on ne pourra pas le supprimer car il n’est pas vide

11.	Pour supprimer le Dossier2 et son contenu on utilise la commande rm –r


# Commands importantes

1.	Pour afficher l’heure on utilise la commande date, la commande time permet de lancer un programme avec des arguments et de définir le moment de l’arrêt du programme.

2.	Ls permet d’afficher les fichiers dans un dossier alors que la permet d’afficher les dossiers cacher (commencent par un point).

3.	Le programme ls se situe dans le dossier /user/bin/ls

4.	Il n’y a pas d’entrer dans le manuel pour la commande ll. 

5.	Pour afficher les fichiers dans le dossier /bin on utilise la commande ll 

6.	La commande ls .. , permet de lister les fichiers du répertoires parents du dossier dans lequel on se trouve

7.	C’est la commande pwd qui donne le chemin complet du dossier courant

8.	La commande echo ‘bip’ > plop permet de créer un fichier plop, ainsi que d’écrire le mot ‘bip’ dans le fichier. L’lorsque l’on exécute deux fois la commande, elle supprime le contenue du fichier 

9.	La commande echo ‘bip’ >> plop permet d’ajouter le mot ‘bip’ au fichier 

10.	La commande sleep 10 | echo 'toto' met en pause le shell pendant 10 secondes en affichant toto

11.	La commande file permet de déterminer le type d’un fichier

12.	L’lorsque l’on ajoute du contenu dans le fichier original après un lien_sym le contenue est également ajouter dans le fichier lié. Si on supprime l’original, le fichier liée reste intact.

13.	Lorsque l’on modifie lien_phy, lien_sym est également modifier, et inversement. D’autre part lorsque lien_phy est supprimer lien_sym deviens rouge et impossible à ouvrir.

14.	Les raccourcis ctrl + S permet d’interrompre le défilement et ctrl + q permet de le reprendre 

15.	La commande head 5 /var/log/syslog permet d’afficher les 5 premières lignes du fichier
La commande tail -n 15 /var/log/syslog permet d’afficher les 15 dernières ligne du fichier
La commande tail –n 20 /var/log/syslog | head 10 permet d’afficher les lignes 10 à 20
16.	La commande dmesg | less affiche un caractère en continue 

17.	Ce fichier contient les utilisateurs du système et leurs informations, le manuelle est accessible depuis man /etc/passwd

18.	

19.	 La commande qui nous permet de savoir combien d’utilisateurs on un compte sur cette machine est : wc –l /etc/passwd

20.	La commande man -k conversion | wc -l nous permet de voir que 141 pages de manuel comportent le mot-clé conversion dans leur description.

21.	La commande find / -iname "passwd" nous permet de trouver les fichiers se nommant passwd

22.	Afin d'enregistré les fichiers trouvés dans un fichier précis il faut faire find / -iname "passwd" >> list_passwd_files.txt. Pour rediriger les erreurs on utilise la commande find / -iname "passwd" >> /dev/null 

23.	Q

24.	Le fichier history.log se trouve dans /var/log/apt/history.log


# Exercice 3 : Découverte de l'éditeur de texte nano

1.	![GitHub Logo](/assets/ex3.1.png)

2.	![GitHub Logo](/assets/ex3.2.png)
  
3.	Pour d’déplacer les 10 première ligne il faut faire ctrl+K pour cut les 10 première ligne, par la suite avec ctrl+ flèche du bas on colle les lignes à la fin du fichier.
Pour annuler on utilise Alt+U ou sortir sans sauvegarder
 

# Exercice 4 : Personnalisation du shell
1.	On créer une copie du fichier .bashrc avec la commande cp .bashrc .bashrc_bak
2.	![GitHub Logo](/assets/ex4.1.png) 
3.	![GitHub Logo](/assets/ex4.3.png)
4.	![GitHub Logo](/assets/ex4.4.png)

