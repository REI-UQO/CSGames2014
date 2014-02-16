Petit tuto pour bien commencer avec GitHub sur Windows
﻿======================================================


Installation
============
Telecharger et installer ces logiciels:
	- http://windows.github.com/
	- *http://git-scm.com/downloads

	*Il se pourrait que le premier installe automatiqement le deuxieme.
	*Verifier si les programmes "GitHub", "Git GUI" et "Git Bash" sont installe en les recherchant dans le menu "Demarrer"
	*SVP modifier cette partie du tuto en consequence!


Cloner un repo de Github.com sur votre machine
==============================================
Trouver votre Repo sur le site
	Ex: https://github.com/REI-UQO/CSGames2014

Clic sur le bouton "Clone in Desktop" a droite
Il sera cloner par defaut dans "Mes Documents/GitHub/CSGames2014"



Envoyer vos modifications de votre machine vers GitHub
======================================================
La suite d'etapes habituelle est:
	- Pull:	On met les fichiers a jour sur notre machine

	- Repeter tant qu'il reste des fichiers unstaged:
		- - Ajout : On ajoute des fichiers qui seront commit
		- - Commit: On indique un message qui resume les modifications faites
	
	- Push:	On envoie les modifications vers GitHub


Console Git Bash
----------------
Dans le Dossier "Github":
	- Clic-droit sur le dossier "CSGames2014"
	- Choisir "Git Bash"

Supposons que je veux ajouter des fichiers, je fais:
	
	git pull	#Je met les fichiers de ma machine a jour
	git status	#Affiche etat du repo, on voit plusiers fichiers en rouges
		
		git add TutoGitHubWindows.txt	#Ajoute ce tutoriel
		git commit -m "Tuto pour GitHub sur Windows"	#Breve explication du commit

		git add "*.txt"		#Ajoute tous les fichiers .txt
		git commit -m "Beaucoup d'autres tutoriels"

		git add "Screenshots/*.jpg"	 #Ajoute tous les fichiers .jpg du dossier "Screenshots"
		git commit -m "Screenshots du programme"

		git add -A #Ajoute tout le reste des fichiers
		git commit -m "Ajout d'un systeme qui ecrit du code magiquement"
		
	git status 	#Je verifie que j'ai bien tout commit les fichiers que je voulais
	
	git push 	#Envoyer mes modifications vers le repo sur GitHub
	#Remplir votre username Github et mot de passe

Git Gui
-------
Avantage: 
	- Permet de visualiser les modifications faites aux fichiers.

Desavantages
	- Plus lent qu'en console parce qu'il faut utiliser la souris.
	- Moins de commandes qu'en console. On ne peut pas mettre d'options

GitHub (programme installe precedemment)
----------------------------------------
Avantage:
	- Permet de cloner a partir du site GitHub en un seul clic

Desavantages
	- Plus lent qu'en console parce qu'il faut utiliser la souris.
	- Moins de commandes qu'en console. On ne peut pas mettre d'options



Bonnes pratiques
----------------
- Éviter les commits messages du genre "Voici tout le travail que j'ai fait dimanche".
	Si vous vous retrouver à faire ça, vous devez commit plus souvent vos changements.
	Vous devez avoir un commit par bloc logique de changement.
	Ex: "BUG RESOLU: Le programme crashait lorsqu'on cliquait trop vite sur le bouton 'OK' " 

- Lorsque vous écrivez vos messages commits, pensez à la personne qui vient de se réveiller et qui va le lire. 
	Parfois ce sera vous-même dans 1 an.












