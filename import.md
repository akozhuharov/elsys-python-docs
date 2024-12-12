# Библиотеки/модул
В python има голям брой включени в езика библиотеки, които могат да бъдат ползвани и също така публично достъпни за инсталация чрез инструмента pip

## Включване в текущата програма
Ако искате да използвате функции/класове от друг модул става по следният начин:
```python
import math # Включва се целият модул
print(math.sqrt(4))  # Функцията се извиква с името на модула преди името на функцията



from math import sqrt  # Включва се само функцията
print(sqrt(4))  # Може да се извика директно с нейното име
```

Примерни полезни библиотеки вградени в езика:
* math - математичски функции
* os - интерфейс към операционната систем
* email - работа и изпращане на имейли
* datetime - работа с време(години/месеци/дни/часове)
* zipfile - работа с архиви

Пълен списък може да намерите тук:
[Python standard library](https://docs.python.org/3/library/index.html)  

Публични модули може да намерите тук:  
[PYPI](https://pypi.org/)