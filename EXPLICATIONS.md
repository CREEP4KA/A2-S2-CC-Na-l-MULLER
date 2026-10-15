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

git switch -c  feature/accueil 76184a8 
git switch -c  feature/contact 76184a8 