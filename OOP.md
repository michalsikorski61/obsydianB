wszystko w py jest obj, a sam jezyk jest oparty o OOP, ale co to znaczy? Co znaczy, że coś jest  obiektem, albo, że py jest językiem Object oriented programing? Jak się ma programowanie skryptowae do oop?

czym jest obj?
Wyobraźmy sobie, że chcemy zbudować dom
tworzymy więc projekt, który w terminologi progrmistycznej będzie klasą, natomiast konkretny dom na podstawie projektu, to obiekt.
![[Pasted image 20230504031350.png]]
tzn. klasą nazywamy schemat, na bazie którego tworzymy obiekty. Obiekt jest instancją danej klasy i jest to namacalny twór, który możemy wykorzystywać w programie do realizacji określonych zadań. Tak więc obj i instancje to w gruncie rzeczy, to samo, z tą różnicą, że słowo instancja, wskazuje na związek danego obj z daną klasą. Analogicznie, na podstawie jednego projektu architektonicznego , czyli klasy, może powstać wiele domów, czyli obiektów, ale tylko jeden z tych domów jest nasz, czyli jest instancją - konkretnym obiektm stworzonym na bazie danej klasy. 

Programowanie obiektowe, to najogólniej, koncepcja progrmistyczna, w której, tworzone przez nas programy są, tak naprawdę, jedynie zbiorem obiektów realizujących określone zadania i wchodzących ze sobą w ciągłe interakcje podczas działania programu.

np samochów. user nie zastanawia się najczęściej, jak działają jego elementy składowo, ale po prostu z niego korzysta. Korzystając jedynie z namacalnego interfrejsu urzytkownika, np kierownicy, pedałó, dźwigni zmiany biegów itp. Tak też działa większość programów, napisanych w większości języków progrmowania. Tzn. user ma kontakt jedynie z powierzchowną warstwą reprezentacji kodu, zaprezentowaną w odpowiedni sposób. np z wykorzystaniem GUI. Tak traktując auto jako program, możemy sobie wyobrazić, że poszczególne jego elementy takie jak silnik czy radio, są obiektami realizującymi poszczególne zadania, gdzie obj te mogą, ale nie muszą wchodzić ze sobą w interakcje. Idąc dalej, róznież same obj mogą składać się z innych obj, np. takie radio w aucie składa się z anteny, detektora itp. 

Ogólny morał - OOP - to podejście oparte o pisanie programów składających się z obj, posiadających określone atr oraz fn, które zostały zdefiniowane w klasach., na bazie których wspomniane obj są tworzone. 
![[Pasted image 20230504032658.png]]
programowanie skryptowe i oop często się uzupełniają i przeplatają, więc nie ma jasnej granicy.

[[Klasy]]
[[Dziedziczenie i polimorfizm]]
[[hermetyzacja i modyfikatory dostępu]]
[[Przeciążanie funkcji i operatorów]]
[[Moduły i pakiety]]