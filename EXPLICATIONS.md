# Identité
Naël Muller ESGI2

git config user.name "Naël MULLER"
git config user.email "nael.creepa@gmail.com"

# état initial

git log --oneline

76184a8 (HEAD -> main) Ajouter le conseil de vérification du compteur
b88cc98 Mettre à jour la durée de référence des créneaux
4a266e1 Créer le portail et le simulateur de créneaux

git status
Sur la branche main
rien à valider, la copie de travail est propre

git switch feature/tutorat
Sur la branche feature/tutorat
rien à valider, la copie de travail est propre

Dans index.html : Ajouter un créneau augmente le nombre et la durée totale ; Recommencer remet le nombre et la durée totale à zéro. L'actualisation réinitialise la simulation.
1 créneau = 200 minutes
On peut ajouter les créneaux un par un.

Le commit dont je pars dans main, et donc dans feature/accueil et feature/contact, est le **76184a8 (HEAD -> main) Ajouter le conseil de vérification du compteur**


### git switch -c  feature/accueil 76184a8 

Après les modifications pour l'adresse mail cliquable:
git add index.html
git commit -m "Modification des permanences" 
git log :

commit 9dba3cec181d97a1e4982461afe2e039f7228c29 (HEAD -> feature/accueil)
Author: Naël MULLER <nael.creepa@gmail.com>
Date:   Thu Oct 15 16:20:23 2026 +0200

    Modification des permanences

    
### git switch -c  feature/contact 76184a8 

Après les modifications pour l'adresse mail cliquable:
git add index.html
git commit -m "Adresse mail de contact cliquable"
git log:
    
commit d23d8414a1821a931f0d55b2ee85269a522fe2a1 (HEAD -> feature/contact)
Author: Naël MULLER <nael.creepa@gmail.com>
Date:   Thu Oct 15 16:23:47 2026 +0200

    Adresse mail de contact cliquable




Ensuite, on switch sur main et on fait un merge :

git merge feature/accueil
git merge --continue

git merge feature/contact
git merge --continue