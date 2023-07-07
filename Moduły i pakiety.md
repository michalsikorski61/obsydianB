## Wprowadzenie
Umieszczanie wszystkiego w jednym pliku nie jest jedyną drogą jaką możemy obrać. Znając programowanie obiektowe, wiemy jak używać klas, metod, mechanimów dziedziczenia, polimorfizmu, harmetyzacji i przeciążania w celu tworzenia oprogramowania modularnego, w którym skupiamy się nie tyle na wyrażeniach i instrukcjach, ale na obiektach które wchodzące ze sobą w interakcje, przy okazji, realizują wspomniane wyrażenia i instrukcje, celem przetwarzania danych istotnych z punktu widzenia działania programu, no i interesów jego użytkowniaka. 

![[Pasted image 20230507040847.png]]

Język py korzysta z czegoś co nazywamy modułami i pakietami. Gdzie modułem najczęściej nazywamy po prostu pojedynczy plik o rozszerzeniu py, który nie jest skryptem, ale deklaruje szereg funkcji, klas, metod i danych, które mają , mniej lub bardziej ściśle określoną funkcjonalność., którą możemy wykorzystać w skrypcie lub w tworzonym progrmie.

Pakietem natomiast nazywamy folder zawierający pojedyncze moduły. Struktura hiararchi pakietów i modułów przyjmuje formę swoistego drzewa, ktÓre nazywamy w py przestrzenią nazw, która pozwala zapanować nad zależnościami między konkretnymi modułami oraz pakietami.

NIemniej można wyróżnić 3 główne rodzaje modułów i pakietów w  py:
- wbudowane w środowisko py (np. math, statistics)
- Usera - nic nie stoi na przeszkodzie, aby w zależności od potrzeb i złożoności tworzonego oprogramowania, tworzyć własne moduły i pakiety, które będą w sposób celowany i precyzyjny zapewniały pożądaną funkcjonalność.
- Zewnętrzne - z wykorzystaniem dedykowanych narzędzi do zarządzania pakietami, takich jak pip czy też conda, możemy przebierać spośród tysięcy modułów i pakietów tworzonych przez innych programistów, po czym oczywiście instlować je w zależności od potrzeb na naszych komputerach, celem wykorzystania ich w naszych implementacjach. Np. numpy, matplotlib,scikit-learn. 

## Programowanie skryptowe vs obiektowe

W którym z tych podejść znajduje zastosowanie wykorzystanie modułów i pakietów?
Oczywiście w obu podejściach wykorzystujemy moduły i pakiety. 

[[Tworzenie i wykorzystywanie modułów]]
[[Tworzenie i wykorzystywanie pakietów]]

