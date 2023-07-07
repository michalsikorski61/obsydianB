mamy sobie wbudowaną metodę instancyjną o nazie init, która jest wywoływana automatycznie, gdy klasa jest wykorzystywana do stworzenia jej instancji, co pozwala w tym momencie ustawić jej parametry. Metoda init może być traktowana jako swoisty konstruktor klasy, który ustawia początkowy stan tej instancji tej klasy, nazwa _ _ init _ _ to bowiem skrut od initialization - inicjalizacja
![[Pasted image 20230504071614.png]]

ofc tak jak inne metody metoda init, jako pierwszy parametr deklaruje self, a następnie parametry, które będą wiązane z arg przekazywanymi do klasy podczas tworzenia jej instancji

![[Pasted image 20230504071951.png]]

ofc użycie kwargs nie jest wymagane i możemu użyć arg pozycyjnych

zaimplementujmy metody
![[Pasted image 20230504080051.png]]

Wiemy jednak, że kwadrat jest tak naprawdę szczególnym przypadkiem prostokąta - tutaj na scenę wchodzi dziedziczenie, pozwalające nam unikać pisania po kilka razy tego samego

funkcja super() pozwala nam korzystać z dobrodziejstw klasy dziedziczonej, w klasie dziedziczącej

fn super() pozwala nam niejako nawiązać połączenie z klasą nadrzędną, dzięki czemu możemy w niej wywołać metodę init i niejako stworzyć istancję klasy nadrzędnej, w klasie podrzędnej

![[Pasted image 20230504081027.png]]


mozna teraz założyć. że chcemy skonstruować klasę sześcian, wraz z metodami do boliczania jego pp oraz ob
w tej sytuacji najlepiej będzie jeśli sześcian będzie dziedziczył po kwadracie

![[Pasted image 20230504081343.png]]
w sześcianie wykorzystujemy super do korzystania z dobrodziejsct całej drabinki dziedziczenia, tj. z atr dziedziczonej klasy kwadrat,a także atr klasy prostokąt po której dziedziczy kwadrat. Dodatkowo wprawdzailiśmy polimorfizm - mechanizm pozwalający wykorzystywać nazwy atrybutów z istniejącej drabiny hierarchi dziedziczenia i zmieniać ich charakterystykę. np. możemy wykorzystać nazwę metody inst. która pochodzi z klasy Prostokat i zmienić jej zachowanie tak, by była użyteczna z poziomu klasy sześcian

