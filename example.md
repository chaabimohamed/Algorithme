Algorithme is a simple Python package that I created to learn how packages work in Python.
[pypi](https://pypi.org/project/Algorithme/0.1/)
[github](https://github.com/chaabimohamed/Algorithme)

## Installation

```bash
pip3 install Algorithme
```

```python
from Algorithme import algo
```
___
Exercice 1 : Somme, Produit
- Écrire un algorithme qui lit 2 nombres entiers au clavier, qui calcule et affiche leur somme et leur produit.

```python
nomb1 = int(input("Entre le nomber 1"))
nomb2 = int(input("Entre le nomber 2"))

#calcule et affiche somme
som = algo.somme(nomb1,nomb2)
print(som)

#calcule et affiche produit
prod = algo.produit(nomb1,nomb2)
print(prod)
```
___
Exercice 2 : Maximum, Minimum
- Écrire un algorithme qui lit trois variables au clavier et affiche le maximum des trois.

```python
maximum = algo.plusGrand(11,10,9)
print(maximum)
```
```python
minimum = algo.plusGrand(11,10,9,inverser=True)
print(minimum)
```
____
Exercice 3 : Puissance
- Écrire une fonction qui permet de calculer la puissance de 2 nombres entiers passés en paramètres. Écrire un programme qui saisit deux nombres entiers positifs et calcule le premier à la puissance du second. Il affiche le résultat.

```python
puissan = algo.puissance(11,19)
print(puissan)
```
___
Exercice 4 : Impair, Pair
- Affichez les nombres pairs entre 0 et 50. Affichez la table de multiplication d’un nombre entré par l’utilisateur

```python
for i in range(0,51):
    if algo.nomberPair(i):
        print(i)
        
nomb=4

# nomber 4 est pair: true or false
resu = algo.nomberPair(nomb)
if resu: #true
    print('Nomber pair')
else: #false
    print('Nomber pas pair')

# nomber 4 est impair: true or false
resu = algo.nomberImpair(nomb)
if resu:
    print('Nomber impair')
else:
    print('Nomber pas Impair')
```
___
Exercice 5 : Triangle de Pascal
- Écrire une procédure qui permet d’afficher le triangle de Pascal de degré n. (n sera donnée en paramètre)
- Exemple : pour n=5
-   1
-   1 1
-   1 2 1
-   1 3 3 1
-   1 4 6 4 1

```python
n=5
algo.triangledePascal(n)
```
___
Exercice 6 : Nombre Parfaits
- Écrire un programme qui affiche tous les nombres parfaits inférieurs à une limite donnée par l’utilisateur un nombre est dit parfait s’il est égal à la somme de ses diviseurs stricts.
- Exemple : 6 est parfait car 6=1+2+3

```python
n = 6

resu = algo.nomberParfait(n)
if resu:#true
    print('nomber parfait ')
else:
    print('nomber non parfait ')
```
___
Exercice 7 : ValeurAbsolue
 
```python
x = algo.valeurAbsolue(-4)
print(x)
x = algo.valeurAbsolue(2)
print(x)
```
___
Exercice 8 : Factorielle

```python
a = algo.factorielle(9)
print(a)
```
___
Exercice 9 : Tout les Deviseur d'un nomber

```python
nomber=20
toutdevieur= algo.toutlesDevi(nomber)
print(toutdevieur)
```
___
Exercice 10 : Double
- Calcule et affiche le double de nombre 10

```python
d = algo.doublenomber(10)
print(d)
```
___
Exercice 11 : Nomber Premier
- Ecrire un programme qui vérifie si un nombre entier saisi par l’utilisateur est un nombre premier ou pas. Un nombre premier est un nombre qui ne permet la division que sur 1 et lui-même.
- Exemples de nombre premier : 2, 5, 7, 11, 13

```python
a = 13
resu = algo.nomberPremier(a)
if resu:#true
    print('nomber premier')
else:
    print('nomber non premier')
```
___
Exercice 12 : PGCD
- Ecrire un algorithme qui calcule le PGCD de deux entiers a et b en utilisant l’algorithme d’Euclide. Cet algorithme calcule le reste de la division entière de a par b tant que le reste n’est pas nul, et remplace a par b et b par le reste. Le PGCD est le dernier reste non nul. On supposera que a et b sont positifs.

```python
a=100
b=310

pgcd = algo.PGCD(a,b)

print(pgcd)
```
___
Exercice 13 : Nombres frères nombres amis
- Deux entiers n1 et n2 sont dits « amis » si les sommes des chiffres les composants sont identiques (Ex : n1=65 et n2=56). Ils sont dits « frères » si chaque chiffre constituant le premier nombre entier n1 apparaît au moins une fois dans le deuxième nombre n2 et respectivement, si chaque chiffre constituant le deuxième nombre entier n2 apparaît au moins une fois dans le premier nombre n1 (n1=25 et n2=522).

```python
n1=65
n2=56
out = algo.nombresAmis(n1,n2)
if out: #true
    print('n1 est n2 : amis')
else:
    print('n1 est n2 : sont pas amis')

n1=25
n2=522
out = algo.nomberFrere(n1,n2)
if out: # true
    print('n1 est n2 : frere')
else:
    print('n1 est n2 : sont pas frere')
```
___
Exercice 14 : PrixTTC à payer
- Ecrire un algorithme qui demande à l’utilisateur le prix hors taxe d’un article, le taux de TVA et le taux de remise , puis calcule et affiche le prix TTC

```python
nomber=int(input("Entre le nomber d'element : "))
prixHors = int(input("Entre le prix hors taxe de article: "))
tva = int(input("Entre le taux de tva (%) : "))
remise= int(input("Remise: (%)"))

prixTtc = algo.prixTTC(nomber,prixHors,tva,remise)
print(prixTtc)
```
___
Exercice 15 : suite de fibonacci
```python
u0=0
u1=1

lessuite=algo.suitedeFibonacci(5,0,1)
```
___
Exercice 16 : Bissextile.
- Ecrire un programme qui demande a l'anne bissextile ou non

```python
annee = 2004
res=algo.anneBissextile(annee)
if res:#true
    print('bissextile')
else:
    print('non')
```
___
Exercice 17 : Nombre Palindrome
- Ecrire un programme qui verifie si un nombre est plindrom ou non.

```python
n=161
res = algo.nombresPalindrome(n)
if res:
    print('nombre est plindrome')
else:
    print('non')
```
___