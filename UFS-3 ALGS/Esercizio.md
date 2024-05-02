### List Comprehension

```python
nomCom = [elem[0][:4] + elem[1][4:] for elem in zip(fauna, fauna[::-1])]
print(nomCom)
```
### Extend & List()

```python
carrello = []
pozzo = ['███','▓▓▓','▒▒▒', '░░░']  # <-- cima del pozzo
#pozzo = ['┼┼','┤├','┐┌', '╗╔', '║║']  #  ['║', '║', '╗', '╔', '┐', '┌', '┤', '├', '┼', '┼']
# scrivi qui
i = len(pozzo)
while pozzo != []:
    i-=1
    print(f"il pozzo è {pozzo}")
    print(f"Trivello lo strato {pozzo[i]} e lo divido nei blocchi {list(pozzo[i])}")
    carrello.extend(pozzo.pop())
```

### Dictionaries


```python
verdure = {'carote':5,
           'pomodori':8,
           'cavoli':3}
chiavi = verdure.keys()
chiavi
# output : dict_keys(['carote', 'pomodori', 'cavoli'])
val = verdure.value()
val
# output : dict_values([5, 8, 3])
elem = verdure.items()
elem
# output : dict_items([('carote':5), ('pomodori':8), ('cavoli':3)])
verdure['patate'] = 8
# per cambiare il valore dell'elemento con quella chiave
# se sbagliamo a mettere la chiave sbagliata ne creerà un nuovo elemento con quella chiave e quel valore
```