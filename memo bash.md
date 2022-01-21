
# Commandes Bash de base :

# Commandes de gestion des fichiers et repertoires
• ls : Liste le contenu d’un repertoire. S
Options :
· -a : liste egalement les fichiers et repertoires caches (i.e., dont le nom commence par un point).
· -l : liste en plus les attibuts des fichiers.
· -h : avec -l donne les tailles des fichiers sous forme plus lisible.

• cd (Change Directory) : Change le dossier/repertoire courant. Commande interne.
Exemples :
· cd <rep> : se deplace dans le repertoire indique en parametre.
· cd : se deplace dans le repertoire personnel (/)
· cd .. : remonte dans le repertoire superieur/parent.
· cd - : se deplace dans le dernier repertoire visite.

• mkdir <rep1> <rep2> ... (Make Directory) : cree les repertoires indiques en parametre (au moins
un). 
Option :
· -p : si les repertoires peres n’existent pas, ils sont egalement crees.

• rmdir <rep1> <rep2> ... (Remove Directory) : Supprime les repertoires indiques (au moins 1). Les
repertoires doivent etre vides.

• rm <fich1> <fich2> ... (Remove) : supprime les fichiers passes en parametres. ATTENTION :
aucun moyen de les recuperer ensuite. Options :
· -i : demande confirmation avant chaque effacement.
· -f : ne demande jamais de confirmation
· -r : effacement recursif. Ex : rm -r <rep1> <rep2> ... permet d’effacer les repertoires indiques
et tout ce qu’ils contiennent.

• cp (Copy) : Copie de fichiers et de repertoires.
Utilisation :
· cp <fich1> <fich2> : cree un nouveau fichier de chemin <fich2> et copie dedans le contenu de
<fich1>. Si <fich2> existait deja, il est ecrase.

• mv (Move) : Deplacer/renommer des fichiers et des repertoires.
Utilisation :
· mv <fich1> <fich2> : deplace le fichier <fich1> pour que son chemin devienne <fich2>.

• ln <fich1> <fich2> (Link) : Cree un lien physique du fichier <fich1> vers <fich2>.
Option :
· -s : cree un lien symbolique au lieu d’un lien physique. On peut creer un lien symbolique d’un
repertoire vers un autre.

• touch <fich1> <fich2> ... : Cree des fichiers vides. Si les fichiers existent deja, alors leur date de
derniere modification est mise a la date courante.


# Commandes sur les fichiers
• wc <fich> (Word Count) : Compte le nombre de lignes, mots et caracteres d’un texte.
Options :
· -l (Line) : le nombre de lignes.
· -c (Character) : le nombre de caracteres.
· -w (Word) : le nombre de mots.

• head -n <nb> <fich> : Extraire les <nb> premieres lignes.

• tail -n <nb> <fich> : Extraire les <nb> dernieres lignes. Si <nb> est de la forme +n, alors extraire a
partir de la n-ieme ligne.

• grep <motif> <fich> (Global Regular Expression Print) : Afficher les lignes contenant le <motif>.
Options :
· -c : afficher le nombre de lignes contenant le <motif>.
· -n : afficher en plus le numero de la ligne.
· -v : afficher les lignes qui ne contiennent pas le <motif>.

• cut <colonnes> <fich> : Extrait certaines parties dans chaque ligne.
Options :
· -c : indique la ou les positions des parties a extraire.
· -f : indique un numero de champ.
· -d : indique un caractere delimiteur de champ.

• sort <fich> : Trie les lignes par ordre alphabetique croissant.
Options :
· -r : tri decroissant.
Options :
· -c : affiche en plus le nombre d’occurence de chaque ligne.
· -u : affiche seulement les lignes n’apparaissant qu’une seule fois.
· -d : Affiche seulement les lignes repetees.

• more : Affiche le contenu d’un fichier page par page. La touche espace permet de passer a la
page suivante La touche q permet de quitter.

• less : Affiche le contenu d’un fichier page par page. Les touches ↑ et ↓ permettent de se deplacer
dans le texte . La touche / permet de rentrer au clavier une chaıne a rechercher dans le texte et les
touches n et N permettent de se deplacer sur les differentes occurences de la chaıne. La touche
q permet de quitter.


# Aide
• man <section> <commande> : affiche la page du manuel de la commande <commande>. Le parametre
<section> est facultatif et permet de specifier la section du manuel ou recherche la commande.

• info : presente les pages d’infos qui sont en general plus detaillees et plus lisibles que les pages du
manuel. Ces pages sont structurees en arbre.


