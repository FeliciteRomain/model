# Commandes GIT de base :
# Git config
   On l’utilise pour configurer les préférences de l’utilisateur : 
   son mail, le nom d’utilisateur et le format de fichier etc
      ex : git config --global user.email example@google.com
# Git init
   Cette commande est utilisée pour créer un nouveau dépôt GIT :
      ex : git init
# Git add
   La commande git add peut être utilisée pour ajouter des fichiers à l’index.
     ex : git add temp.txt
# Clone git
   La commande git clone est utilisée pour la vérification des dépôts. Si le dépôt se trouve sur un serveur distant, utilisez:
      ex : git clone example@93.188.160.58:/chemin/vers/dépôt
   Inversement, si une copie de travail d’un dépôt local doit être créée, utilisez:
      ex : git clone /chemin/vers/dépôt
# Git commit
   La commande git commit permet de valider les modifications apportées au HEAD. Notez que tout commit ne se fera pas dans le dépôt distant.
      ex : git commit –m “Description du commit”
# Git status
   La commande git status affiche la liste des fichiers modifiés ainsi que les fichiers qui doivent encore être ajoutés ou validés. Usage:
      ex : git status
# Git push
   Git push est une autre commandes GIT de base. Un simple push envoie les modifications locales apportées à la branche principale associée :
      ex : git push origin master
# Git checkout
   La commande git checkout peut être utilisée pour créer des branches ou pour basculer entre elles. Par exemple nous allons créer une branche:
      ex : command git checkout -b <nom-branche>
   Pour passer simplement d’une branche à une autre, utilisez:
      ex : git checkout <nom-branche>
# Git remote
   Cette commande remote permet à un utilisateur de se connecter à un dépôt distant. La commande suivante répertorie les dépôts distants actuellement configurés:
      ex : git remote –v
   Cette commande permet à l’utilisateur de connecter le dépôt local à un serveur distant:
     ex : git remote add origin <93.188.160.58>
# Branch git
   La commande git branch peut être utilisée pour répertorier, créer ou supprimer des branches. Pour répertorier toutes les branches présentes dans le dépôt, utilisez:
      ex : git branch
   Pour supprimer une branche:
      ex : git branch –d <nom-branche>
# Git pull
   Pour fusionner toutes les modifications présentes sur le dépôt distant dans le répertoire de travail local, la commande pull est utilisée. Usage:
      ex : git pull
# Git merge
   La commande git merge est utilisée pour fusionner une branche dans la branche active. Usage:
      ex : git merge <nom-branche>
# Git diff
   La commande git diff permet de lister les conflits. Pour visualiser les conflits d’un fichier, utilisez
      ex : git diff --base <nom-fichier>
   La commande suivante est utilisée pour afficher les conflits entre les branches à fusionner avant de les fusionner:
      ex : git diff <branche-source> <branche-cible>
   Pour simplement énumérer tous les conflits actuels, utilisez:
      ex : git diff
# Git log
   L’ exécution de cette commande génère le log d’une branche. Un exemple de sortie :
      ex : commit 15f4b6c44b3c8344caasdac9e4be13246e21sadw 
      ex : Author: Alex Hunter <alexh@gmail.com> 
      ex : Date: Mon Oct 1 12:56:29 2016 -0600
# Git reset
   Pour réinitialiser l’index et le répertoire de travail à l’état du dernier commit,
      ex : git reset --hard HEAD
# Git rm
   Git rm peut être utilisé pour supprimer des fichiers de l’index et du répertoire de travail. Usage:
      ex : git rm nomfichier.txt
# Git show
   Pour afficher des informations sur tout fichier git, utilisez la commande git show . Par exemple:
      ex : git show
# Git fetch
   Git fetch permet à un utilisateur d’extraire tous les fichiers du dépôt distant qui ne sont pas actuellement dans le répertoire de travail local. Exemple d’utilisation:
      ex : git fetch origin
# Git ls-tree
   Pour afficher un fichier arborescent avec le nom et le mode de chaque élément, et la valeur SHA-1 du blob, utilisez la commande git ls-tree . Par exemple:
     ex : git ls-tree HEAD
# Git grep
   Git grep permet à un utilisateur de rechercher dans les arbres de contenu des expressions et / ou des mots. Par exemple, pour rechercher www.hostinger.com dans tous les fichiers, utilisez:
      ex : git grep "www.hostinger.com"
# Git gc
   Pour optimiser le dépôt en supprimant les fichiers inutiles et les optimiser, utilisez:
     ex : git gc
# Git archive
   La commande git archive permet à un utilisateur de créer un fichier zip ou tar contenant les composants d’un arbre du dépôt. Par exemple:
     ex : git archive --format=tar master
# Git rebase
   La commande git rebase est utilisée pour la réapplication des commits sur une autre branche. Par exemple:
     ex : git rebase master

