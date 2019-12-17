---
title: "Formulaire de réponse pour le test 2"
output: pdf_document
---

** **

##### Prénom Nom Groupe



##### Question 1

* Calculer la probabilité de battre un record à l'épreuve $m$

###### Réponse : 

** 1/m **

##### Question 2

* Donner l'espérance de $N$ pour $n = 27$. 

###### Réponse : 

** 3.89 **

##### Question 3

* Calculer ${\rm E}[Y_n]$.


###### Réponse : 

** P(U1<U2) = intégrale[x=0, x=1](1-x)
            = 1 - 1/2
            = 1/2
  De la même manière P(U1<U2<U3) = 1/6
  
  ${\rm E}[Y_n]$ = sum[i=1, i= n-1](${\rm E}[X_i]$
                 = (n-1)*${\rm E}[X_1]$ (car les Xi ont même loi et donc même espérance.)
                 = (n-1)/2**

##### Question 4

* Calculer la valeur de la variance Var$[Y_3]$.

###### Réponse : 

** Var(X1) = ${\rm E}[(X_1)²]$ - (${\rm E}[X_1]$)²
           = ${\rm E}[(X_1)²]$ - 1/4
           = 1/2
   Cov(X1,X2) = ${\rm E}[X_1X_2]$ - ${\rm E}[X_1]$${\rm E}[X_2]$
              = ${\rm E}[X_1X_2]$ - 1/4
              = 1/6 - 1/4 en considérant que la variable X1X2 est un variable de bernoulli de probabilité P(U1<U2<U3)
              = -1/12
   Var(Y3) = ${\rm E}[(X_1 + X_2)²]$ - (${\rm E}[X_1 + X_2]$)²
           = ${\rm E}[(X_1)²]$ + ${\rm E}[(X_2)²]$ + 2${\rm E}[X_1X_2]$ - 1
           = 1/3**

##### Question 5

* Calculer Var$[Y_n]$ pour tout $n \geq 2$.

###### Réponse : 

** Pour démontrer la formule on procède par récurrence : 
      Var(X1 + X2) = Var(X1) + Var(X2) +2Cov(X1,X2) d'après le cours
      Supposons que la propriété est vraie au rang n :
            On a alors Var[Y n] = ∑i=1n−1Var[X i]+2∑i=1n−2Cov[Xi,Xi+1]
                 On passe au rang (n+1), ainsi
                  Var[Y (n+1)] = Var(Y_n + X_n)
                               = Var(Y_n) + Var(X_n) +2Cov(Y_n,X_n)
                            = ∑i=1,n−1(Var[X i]) + Var(X_n) + 2∑i=1,n−2(Cov[Xi,Xi+1]) + 2Cov(Y_n, X_n)
                               = ∑i=1,n(Var[X i]) + 2∑i=1,n−2(Cov[Xi,Xi+1]) + 2∑i=1,n−1(Cov(Xi, X_n))
                               = ∑i=1,n(Var[X i]) + 2∑i=1,n−1(Cov[Xi,Xi+1])
                               On a bien la formule au rang n+1
      La propriété est vraie pour tout n.
      Tous les Xi ont la même loi. Ainsi en ayant Var(X1) = 1/2 et Cov(Xi, Xi+1) = -1/12
            D'où : Var(Y_n) = (n-1)/2 + 2*(n-2)*(-1/12)
                            = [3(n-1) - (n-2)]/6
                            = (2n -1)/6**


##### Question 6

* Combien de tirages suffisent pour qu'avec une probabilité supérieure à 0.99, $A_{n-1}$ soit proche de la valeur 1/2 à $10^{-2}$ près. 

###### Réponse : 

** **


##### Question 7

* Déterminer la valeur de $c$.



###### Réponse : 

** ** 


##### Question 8

* Déterminer la fonction de répartition de la variable $Y$. Donner sa valeur au point $t = 2/3$. 

###### Réponse : 

** **


##### Question 9


* Ecrire un algorithme de simulation d'un couple de densité $f(x,y)$.  

###### Réponse : 

** **

##### Question 10


* On pose $Z =  X Y$. Déterminer la densité de la loi de la variable $Z$.
   
###### Réponse : 


** ** 


