# Списъци (Lists)
Списъкът е структура от данни, която служи за запазване на много стойности под една променлива. Има различни функции, които помагат с работата със списъци, като всяка функция се извиква в формат `var.func() `, където var e името на променливата, а func e функцията.
```python
# Дефинираме списък с квадратни скоби:
names = ["Petar", "Ivan", "Ogi", "Nasko"]
# Достъпът до елементи става чрез индекса, като броим от 0
names[0] # Result: Petar
# Отрицателен индекс
names[-1] # Result: Nasko
# range(обхват) - не включва елемента на затварящия индекс, в случая 3
names[1:3] # Result: ["Ivan", "Ogi"] 
# добавяне на елемент
names.append("Boyan") # Result: ["Petar", "Ivan", "Ogi", "Nasko", "Boyan"]
# Премахване на елемент по стойност
names.remove("Ogi") # Result: ["Petar", "Ivan", "Nasko", "Boyan"]
# Премахване на елемент по индекс
names.pop(0) # ["Ivan", "Nasko", "Boyan"]
```

# For цикъл
Синтаксис
```python
names = ["Petar", "Ivan", "Ogi", "Nasko"]
for i in names:
    # Ключова дума for следвана от променливата която ще приема всяка стойност(i), ключова дума in и променлива за обхождане(в случая списъка names)
    print(i)
# Petar
# Ivan
# Ogi
# Nasko
```
## range фунцкия
```python
# Генериране на числата от 0 до 99(100-1)
for i in range(100):
    print(i)
# Генериране на числата от 5 до 9
for i in range(5,10):
    print(i)
# Генериране на числата от 50 до 100 със стъпка 3
for i in range(50,101):
    print(i)
```

## Излизане от цикъл(break)
Излизането от цикъл става с ключова дума break, най-често използвана при някакво условие(if)
```python
names = ["Petar", "Ivan", "Ogi", "Nasko"]
for i in names:
    print(i)
    if i == "Ogi":
        # Когато достигне елемента със стойност Ogi ще излезем от цикъла
        break
    
```

## Продължава на цикъла(continue)
Като горният пример, само че тук не изпълняваме оставащият код в цикълния блок
```python
for i in names:
    if i == "Ogi":
        # Когато достигне елемента със стойност Ogi ще пропуснем изпълнението на print-a
        continue
    print(i)
```
