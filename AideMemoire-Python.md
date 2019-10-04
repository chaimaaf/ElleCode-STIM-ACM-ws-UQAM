Aide-Mémoire: Python3
===

Bases
---

- Écrire un commentaire dans le code: 
  ```
       # Voici mon commentaire
   ```
- Créer une variable: 
  ```
       ma_variable = 'bonjour'
   ```
- Imprimer `ma_variable` à l'écran: 
  ```
       print(ma_variable)  # imprime bonjour à l'écran.
   ```
- Imprimer une variable accompagnée d'une phrase à l'écran:
  ```
       print('Ma variable est: {}'.format(ma_variable)) # imprime à l'écran: Ma variable est: bonjour
   ```



Validations
---
_Prenons en considération que `ma_variable` est toujours égal à `2` comme le présente la première ligne du tableau_.

| Mathématique | Informatique | Exemple |
| ---: | :---: | :--- |
| assignation de valeur | `=` | `ma_variable = 2` |
| addition | `+` | `1 + ma_variable` donne `3`. |
| soustraction | `-` | `1 - ma_variable` donne `-1`. |
| multiplication | `*` | `2 * ma_variable` donne `4`. |
| division | `/` | `4 / ma_variable` donne `2`. |
| restant de la division (modulo) | `%` | `9 % ma_variable` donne `1`. |
| plus grand | `>` | `ma_variable > 4` donne `False` |
| plus grand ou égal | `>=` | `ma_variable >= 4` donne `False` |
| plus petit | `<` | `ma_variable < 4` donne `True` |
| plus petit ou égal | `<=` | `ma_variable <= 4` donne `True` |
| égal à | `==` | `ma_variable == 2` donne `True` |
| *assignation et addition | `+=` | `ma_variable += 1 # équivaut à ma_variable = ma_variable + 1` donne 2 + 1 = `3`|
| *assignation et soustraction | `-=` | `ma_variable -= 1 # équivaut à ma_variable = ma_variable - 1` donne 2 - 1 = `1` |
| et | `and` | `ma_variable < 10 and ma_variable > 1` donne `True` |
| ou | `or` | `ma_variable == 2 or ma_variable == 3`  donne `True` |
| non | `not` | `not True` donne `False`, `not False` donne  `True` |

### Si

_Forme:_
```
   if <condition>:
       print('Condition remplie')
```

_Exemple fonctionnel:_
```
   x = 1
   if x == 1:
       print('x est égal à 1') # imprime à l'écran x est égal à 1.
```

### Si et sinon

_Forme:_
```
   if <condition>:
       print('condition remplie')
   else:
       print('condition non remplie')
```

_Exemple fonctionnel:_
```
   x = 1
   if x == 0:
       print('x est égal à 0.')
   else:
       print('x n'est pas égal à 0.') # imprime à l'écran x n'est pas égal à 0.
```

### Si et sinon si

_Forme:_
```
   if <condition 1>:
       print('condition 1 remplie')
   elif <condition 2>:
       print('condition 2 remplie')
```

_Exemple fonctionnel:_
```
   x = 1
   if x == 0:
       print('x est égal à 0.')
   elif x > 0:
       print('x est un nombre positif.') # imprime à l'écran x est un nombre positif.
```

#### À retenir
1. Le `si` peut être seul.
2. Le `sinon` et le `sinon si` doit être accompagné d'un `si`
3. Le `sinon si` peut être suivi d'un `sinon`

_Forme générale:_
```
   if <condition 1>:
       print('condition 1 remplie')
   elif <condition 2>:
       print('condition 2 remplie')
   elif <condition 3>:
       print('condition 3 remplie')
   ...
   elif <condition n>:
       print('condition n remplie')
   else:
       print('aucune condition précédente remplie')
```

Boucles
---

### Boucle for

_Exemple pour une liste:_
```
   liste = ['arbre', 'berceau', 'cercle']
   for item in liste:
       print(item)
   # imprime à l'écran:
   # arbre
   # berceau
   # cercle
```

_Exemple pour un compteur:_
```
   for n in range(1, 4):
       print(n)
   # imprime à l'écran:
   # 1
   # 2
   # 3
```

_Exemple pour une liste énumérée:_
```
   liste = ['allo', 'bonjour']
   for indice, valeur in enumerate(liste):
       print('À l\'indice {} se trouve {}.'.format(indice, valeur))
   # imprime à l'écran:
   # À l'indice 0 se trouve allo.
   # À l'indice 1 se trouve bonjour.

```

### Boucle while

_Forme:_
```
   while <condition>:
       print('condition remplie')
```

_Exemple fonctionnel:_
```
   x = 1
   while x < 4:
       print('x est plus petit que 4')
       x = x + 1
      
   # imprime à l'écran:
   # x est plus petit que 4
   # x est plus petit que 4
   # x est plus petit que 4
```

Intéractions avec l'utilisateur
---

_Forme:_
```
   input(<message adressé à l'utilisateur>)
```
retourne ce que l'utilisateur entre au clavier

_Exemple fonctionnel:_
```
   n = input("Entrer un nombre positif : ")
   # l'utilisateur entre: 42
   print(n)
   # affiche: 42
```


