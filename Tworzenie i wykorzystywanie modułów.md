Są sytuacje, w których nasz kod źródłowy jest tak rozbudowany i złożony, że warto jest wtedy pójść o krok dalej i pomyśleć o wydzieleniu części zaimplementowanej funkcjonalności do oddzielnego modułu. Zobaczmy jak to może wyglądać w praktyce. Załóżmy bowiem, że nasz kod źródłowy składa się z jednego pola, jednej fn oraz jednej klasy. MOże to wyglądać następująco. 
![[Pasted image 20230507042724.png]]
Moglimyśmy po prostu zacząć pisać i wykorzystywać zadeklarowane konstrukcje w tym samym pliku, jednak celem zwiększenia czytelności kodu i zadbania o jego odpowiednią organizacje, możemy wydzielić napisany kod źródłowy do oddzielnego modułu i użyć go w nowo utworzonym skrypcie. 

W pierwszym kroku zmieniamy nazwę Skrypt.py na geometria.py
Następnie tworzymy nowy plik, w którym będziemy kontynuować naszą pracę, nowy plik będie nazywał skrypt.py.
I teraz załózmy, że chcemy skorzystać z funkcjonalności z pliku geometria.py, który od teraz będziemy nazywać modułem.
Środowisko py pozwala nam to zrobić, za pomocą dedykowanych słów kluczowych i instrukcji, możemy importować wybrane funkcjonalności:

import geometria

użycie import i nazyw modułu, można rozumieć jako ekwiwalent tworzenia instancji klasy, bowiem podobnie jak w przypadku tworzenia instancji klasy, mamy teraz dostęp do całej funkcjonalności zadeklarowanej w modula, z poziomu słowa geometria. Gdzie dostęp do tej funkcjonalności uzyskujemy po kropce, postawionej po nazwie modułu. Można bowiem dla przykładu napisać:
![[Pasted image 20230507043917.png]]

Co ciekawe, jeśli potrzebujemy wybranych funkcjonalnośi z modułu, możemy importować je pojedynczo
![[Pasted image 20230507044107.png]]
Z posiomu naszego pliku mamy teraz dostęp jedynie do klasy Okrąg, zadeklarowanej w module geometria. Przyjemnym jest również to, że nie musimy używać pełnych nazw używanych modułów lub elementów występujących w tych modułach, ale możemy przypisać je do zmiennych, w tym celu korzystamy z trzeciej instrukcji (i słowa kluczowego) , a mianowicie instr. i słowa kluczowego 'as', przy jego użyciu możemy sprawić, że będziemy się odwoływać do klacy Okrąg przy użyciu jakiegoś skrótu, np. Ok
![[Pasted image 20230507044518.png]]

Co więcej, możemy dokonać w ten sposób importu więcej niż jednego modułu, korzystając z wyszczególnienia interesujących nas elementów po przecinku, czyli dla przykładu. 
![[Pasted image 20230507044709.png]]

Jak widać, wykorzystywanie modułów rozszerza nasze możliwości w sposób wręcz niepojęty. Wykorzystanie modułów, wrac z OOP, powoduje że towrozny przez nas kod źródłowy, nie tylko odznacza się wysokim poziomem estetyki, ale przede wszystkim jest łatwiejszy w utrzymaniu, modyfikacji, oraz dalszym rozwijaniu. Modularność sprawia również. że zmniejszamy niebezpieczeństwo wpłynięcia zmianami w jenym pliiku, na całość tworzenia oprogramowania. 


