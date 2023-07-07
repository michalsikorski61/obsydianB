fn może przyjmować dane wejściowe właśnie dzięki param
np fn wyświetlająca iloczyn dwu liczb
def iloczyn(a,b):
	c = a + b
	print(f"wynik: {c}")

param fn wymieniamy po przecinku, w nawiasie, w nagłówku fn, a ich wykorzystanie umieszczamy w floku fn

wywołanie fn natomiast będzie teraz następujące
iloczyn(1,2)
gdzie liczba 1 zostanie podstwiona pod parametr a, a liczba 2 pod param b

! parametrami fn są definiowane w nagłówku, w nawiasie, zmienne, natomiast argumentami - przekazywane do fn w momęcie jej wywołania

domyślnie fn przyjmuje tyle argumentów, ile zdefiniowaliśmy parametrów - jeśli w def są 4 parametry, to w wywołaniu musimy podać 4 argumenty (tzw. arg pozycyjne)

domyślnie argumenty są przypisywane do parametrów pozycynie, czyli w kolejności, możemy to zmienić oznaczając je w wywołaniu

iloczyn(b=1,a=2) tzw. keyword - argument (argumenty kluczowe?)

argumenty kluczowe, powinny być przekazywane PO arg. pozycyjnych

arg domyślne
możemy zdefiniować domyślną wartość parametru, przekazywaną do niego, nawet gdy nie podamy wartości argumentu w wywołaniu

def fn(a,b=9):
	print(a,b)

fn(2)

Nieokreślona liczba arg pozycyjnych

def pole_kola(* r ,pi=3.14):
	wynik = pi * r ** 2
	print(wynik)

* -asteryx 
wszystkie arg jakie zostana przekazane w sposob pozycyjny
do fn, zostana spakowane w tuple
![[Pasted image 20230503115213.png]]

Nieokreślona licz. arg. będących słowami kluczowymi

![[Pasted image 20230503142542.png]]
arg będące słowami kluczowymi, są pakowane do słownika
![[Pasted image 20230503142852.png]]
kwargs - key word arguments

podsumowując 
- interpreter przypisuje arg niebędące key words arg zgodnie z pozycją
- przypisuje kwargs poprzez dopasowanie nazw, tj. szuka par param=arg
- przypisuje dodatkowe args niebędące kwargs do kolekcji będącej krotką
- przypisuje dodatkowe kwargs do kolekcji będącej słownikiem
- przypisuje do param z nieprzypisanymi args wartości domyślne z nagłówka fn
![[Pasted image 20230503174740.png]]

użycie pojedynczego asteryksu w nagłówku fn to postawienie granicy między param do których przypisywane  są wartości pozycyjne, a param do których przypisywane są argumenty będące kwargs
![[Pasted image 20230503175247.png]]
-