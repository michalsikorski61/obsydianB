klasy to też obj
do tworzenia klasy, wykorzystujemy instr class

class Klasa:
	pass

podobnie jak def, instrukcja class to instr. wykonywalna. Znaczy to tyle, że gdy interpreter dotrze do tego słowa, to jego wykonanie spowoduje stworzenie nowego obj typu type i przypisanie nazwy - to jest utworzenie obj reprezentującego deklaracje klasy, nie jest to utorzenie jej instancji

Dzięki temu, podobnie jak w przyadku deklaracji funkcji, możemy korzystać z deklaracji klas, jak z obiektów. 

klasa = Klasa
print(type(klasa))

w ten sposób można przypisać do obj reprezentującego deklaracje klasy, zmienną o nazwie klasa. I możemy zobaczyć, że nasza klasa jest typu type - jest to metatyp, czyli typ który jest klasą którego instancje są klasami


wywołanie klasy, podobnie jak funkcje 
instancja_klasy = Klasa()
print(type(instancja_klasy)) - przedrostek main bo nadrzędna klasa jest zadeklarowana w module main

funkcjonalność klasie możemy nadawać poprzed deklaracje w ich ciałach tzw. atrybutów czyli zmiennych, metod i innych zagniżdzonych klas, które pozwolą instncją klasy pełnić jakąś sensowną rolę w programie.

zmienne w klasie

class Klasa:
	liczba_uczniow = 30

dla kazdej instancji klasy, moge uzyskac dostęp do zmiennej liczba_uczniow i wykoorzystac obj, na który wskazuje ta zmienna. Co ważne każda nowa instancje będzie miała tą samą predefiniowaną wartość int. 

dostęp do predefiniowanych atr danej klasy - po kropce, po nazwie instancji
liczba_uczniow = instancja_klasy.liczba_uczniow

na razie atrybut liczba_uczniow, jest taki sam dla każdej instancji
