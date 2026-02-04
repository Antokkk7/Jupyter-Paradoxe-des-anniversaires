# Simplex

**Coder un algorithme du simplexe de la forme canonique à la forme standard -->**

Pour chaque contrainte du problème va introduire une variable d’écart (qui sera ⩾ 0) de sorte que l’inégalité devienne une égalité.\
Ces nouvelles variables seront appelées variables basiques.


<br>


**Par exemple :**



Maximiser : x1 + 6x2 + 13x3\
x1 ⩽ 200\
x2 ⩽ 300\
x1 + x2 + x3 ⩽ 400\
x2 + 3x3 ⩽ 600\
x1, x2, x3 ⩾ 0


</br>


**Devient :**



Maximiser : x1 + 6x2 + 13x3\
x1 + x4 = 200\
x2 + x5 = 300\
x1 + x2 + x3 + x6 = 400\
x2 + 3x3 + x7 = 600\
x1, x2, x3 ⩾ 0\
x4, x5, x6, x7 ⩾ 0


</br>


**Et finalement :**



Maximiser : x1 + 6x2 + 13x3\
x4 = 200 − x1\
x5 = 300 − x2\
x6 = 400 − x1 − x2 − x3\
x7 = 600 − x2 − 3x3\
Variables non-basiques : x1, x2, x3 ⩾ 0\
Variables basiques : x4, x5, x6, x7 ⩾ 0

