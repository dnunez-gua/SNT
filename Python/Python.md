# Python
## Variables et affectations

Une variable est une zone de la mémoire de l'ordinateur dans laquelle une valeur est stockée.  
En Python, la déclaration d'une variable et son initialisation (c'est-à-dire la première valeur que l'on va stocker dedans) se font en même temps.  

``` python
departement =29
print(departement)
```
Ligne 1. Dans cet exemple, nous avons déclaré, puis initialisé la variable departement à la valeur 29
Ligne 2. Nous avons demandé l'affichage de la valeur de departement.  

Le programme aurait donné un autre résultat s'il avait été :  
``` python
departement =29
print('departement')
```
 
# Opérations sur les variables 

``` python
a=5
b=8
somme = a+b
produit = a*b
print("la somme de ",a," et ",b," est ", somme)
print("le produit de ",a," par ",b," est ", produit)
```

## input 

l'instruction input permet de demander à l'utilisateur d'entrer une valeur qui sera stockée dans une variable

``` python
nom=input("Quel est ton nom ?")
print("Bonjour ",nom) 
```

!!! note "Remarque"  
    Pour obtenir des résultats d'opérations sur des variables, il faut convertir la chaine de caractère entrée par l'utilisateur par des entiers ou des réels  
    
    ``` python
    from math import *
    a=int(input("Donner un premier nombre"))
    b=int(input("Donner un deuxième nombre"))
    c=float(input("Donner un nombre réel"))
    print("la somme de ",a," et ",b," est ", a+b)
    print("La racine carrée de ",c, " est ",sqrt(c)) 
    ```

    
