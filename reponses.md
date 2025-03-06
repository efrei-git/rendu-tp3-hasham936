# Réponses TP3
Réponses aux questions du TP3

Exercice 1

git branch feature-1
git branch feature-2
git branch
git checkout feature-1
echo "Modification dans feature-1" >> README.md
git add README.md
git commit -m "Modification dans feature-1"
git checkout main
cat README.md

Exercice 2

git branch dev
git checkout dev
echo "Contenu des notes" > notes.txt
git add notes.txt
git commit -m "Ajout du fichier notes.txt"
git checkout main
git merge dev
ls
git branch -d dev

Exercice 3

git branch conflit-test
git checkout main
echo "# Projet d'exercice - Version Main" > README.md
git commit -am "Mise à jour README sur main"
git checkout conflit-test
echo "# Projet d'exercice - Version Test" > README.md
git commit -am "Mise à jour README sur conflit-test"
git checkout main
git merge conflit-test

Exercice 4

git checkout -b feature-rebase
echo "Contenu feature" > feature.txt
git add feature.txt
git commit -m "Ajout feature.txt"
git checkout main
echo "Autres modifications" > autre.txt
git add autre.txt
git commit -m "Ajout autre.txt dans main"
git checkout feature-rebase
git rebase main

Exercice 5 

git checkout feature-a
echo "A" > a.txt
git add a.txt
git commit -m "Ajout de a.txt"

git checkout feature-b
echo "B" > b.txt
git add b.txt
git commit -m "Ajout de b.txt"

git checkout feature-c
echo "C" > c.txt
git add c.txt
git commit -m "Ajout de c.txt"

Exercice 6

echo "Contenu des réponses" > reponses.md
git add reponses.md
git commit -m "Solution TP3"




