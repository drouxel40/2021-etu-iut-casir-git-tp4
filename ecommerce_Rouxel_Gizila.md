Comme convention de nommage on a choisie pour ce TP de commencé chaque commit par "TP4_", ensuite on ajoute le numéro du commit.
La commande git tag est utilisée pour ajouter des vérsions aux comités qui en format similaire comme V1.1 ou V1.2 etc

q1.
Un fork est une copie d'un dépôt qui vous permet d'effectuer les changements sans affecter le projet d'origine. 
Un dépôt forké diffère d'un clone en ce qu'une connexion existe entre votre fork et le dépôt d'origine lui-même. 

q2. Download zip est détaché, git clone est connecté avec vérsion distant
q3. git log
q4. 
commit 5651629bb4da4aa2298339d7daa58247d25c4bfb
Author: gbesset <guillaume.besset.pro@gmail.com>
Date:   Thu Jan 21 16:34:42 2021 +0100

    The truth clean
	
q5.

Voici la commande pour commit num 4:
git diff-tree -p e91dd630a76d23c37754d626d6c3326fea7b94f7

e91dd630a76d23c37754d626d6c3326fea7b94f7
diff --git a/theTruthaboutDev b/theTruthaboutDev
index d05cb32..a557edc 100644
--- a/theTruthaboutDev
+++ b/theTruthaboutDev
@@ -1 +1 @@
-La vérité du développeur :
\ No newline at end of file
+On n'apprend bien qu'à force de se tromper
\ No newline at end of file

Voici la commande pour commit num 3:
git diff-tree -p 5bf2b0e7ce93189056af052a731a1207b36254fa

5bf2b0e7ce93189056af052a731a1207b36254fa
diff --git a/theTruthaboutDev b/theTruthaboutDev
new file mode 100644
index 0000000..d05cb32
--- /dev/null
+++ b/theTruthaboutDev
@@ -0,0 +1 @@
+La vérité du développeur :
\ No newline at end of file

Sinon, pour plus d'informations: 
git log -p -3 et git log -p -4

q6.
git status -> affichage des fichiers modifié (contenu de son prochain commit)

q7.
La deuxième personne doit résoudre les conflits de merge  soit avec gitkraken, soit manuellement, 
sinon cette personne doit attendre que la 1er personne validé ses modifications, faire pull et apporter ses  modifications.

q8.
Convention de nommage. 

q9.
On localise un conflit et on adapte/choisi une version qui nous convient et on la régistre.

q10.
git pull  et git status pour vérifier si on a des chemins qui n'ont pas été mergés à cause d'un confilt.

q11.
Modif de script.js

 Q12:
git reset --hard  5ed46d8d80219c0464c99d6ec90df358361d9e64


Q13
$ git status
On branch old-state
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        src/images/items/computer.jpeg

nothing added to commit but untracked files present (use "git add" to track)

Un fichier n'est pas commit

Q14

git add src/images/items/computer.jpeg

git commit --amend --no-edit

Les commit partagés ne sont plus sur la même branche et d'autre personnes peuvent travailler dessus, on évite donc de les modifier.

Q15

5 commit supplémentaire se sont ajouter

git checkout (dernier commit avant le script)

On ne peut pas revenir sur un commit ayant déjà été push



Q16

Les branches permettent de travailler librement sur une partie d'un projet sans affecter celles des autres participant du projet.

Q17 
La branche par défaut est master




