funkcja - blok instrukcji zagnieźdzony pod słowem kluczowym def, jest to twór niezależny, możemy ją umieszczać w jakimkolwiek miejscu kodu i wywoływać niezależnie od innych obj. Natomiast metoda to blok kodu zagnieźdzony pod instr def, który jest wywoływany z użyciem nazwy zapewnionej po tej instrukcji. Jednak w odróznieniu od fn, metody deklarujemy w blokach klas, a nie gdzie nam się podoba. I wywołujemy je na klasach lub instancjach klas, a nie "luzem". Dodatkowo wyrózniamy 3 rodzaje metod.

Medoty instancyjne, klasowe i statyczne
metody instancyjne - najpopularniejsze, najczęściej wykorzystywane. Stanowią trzon oprogramowania tworzonego obiektowo.

class MojaKlasa:
	def metoda_instancyjna(self):
		return 'cos'

każda metoda instancyjna, musi mieć zadeklarowany przynajmniej jeden, obligatoryjny parametr, króry wedle konwencji powinien nosić nazwę 'self'. (samego siebie). Obligatoryjność - związana z niejawnym i automatycznym przekazywaniem do metody instancyjnej, argumentu będącego instancją klasy, na której to instancji taką metodę wywołujemy. Stąd też nazwa - metoda instancyjna

instancja = MojaKlasa()
print(instancja.metoda_instancyjna())
![[Pasted image 20230504050429.png]]

znaczenie tego, że metoda instancyjna pracuje ze swoją instncją klasy jest ogromne - dzięki temu możemy sterować zachowaniem konkretnej instancji klasy i możemy dowolnie modyfikować jej atrybuty.

Metoda klasowa - pozwala modyfikować atrybuty na poziomie klasy, np. wartości bez konieczności modyfikowania deklaracji klasy. Jest to metoda instancyjna, ale z dwoma różnicami.
 - zamiast self, używamy cls - skrót od class - podobnie jak metoda instancyjna, metoda klasowa otrzymuje niejawnie obligatoryjny argument., który tutaj nie jest instancją klasy, ale samą klasą. Dzięki temu można modyfikować atrybuty całej klasy globalnie, c o będzie miało wpływ na wszystkie instancje. 
 - koniecznonść wstawienia przed nagłówkiem linijki informującej interpreter o tym, że ma do czynienia z metodą klasową

@classmethod
def metoda_klasowa(clas,x,y):
	clas.x = x
		cls.y = y

metoda statyczna - metoda, którą możemy wywoływać bezpośrednio na klasie, a nie na jej instancji. Dodatk. podobnie jak przy metodzie klasowej, używamy przy jej deklaracji dekoratora specyficznego, ale już nie używamy żadnych obligatoryjnych parametrów. 

@staticmethod
def statyczna():
	return 'metoda statyczna to jest'

możemy wywoływać na klasie lub jej instancji