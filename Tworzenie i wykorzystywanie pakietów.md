Pakiety czyli zbiory modułów i innych pakietów , zacznijmy od stowrzenia dwu modułów, przechowujących po jednym, banalnie prostym, polu liczbowym. 
![[Pasted image 20230507050523.png]]

![[Pasted image 20230507050543.png]]

Jeżeli teraz chcielibyśmy skorzystać z każdego z 2 stworzonych modułów, to musiałoby to przyjąć następującą formę.
![[Pasted image 20230507050655.png]]

ofc, jeśli korzystamy z wyłącznie dwu modułów, to nie jest jakoś szczególnie problematycznym importowanie ich jeden po drugim. Wyobrażmy sobie jednak, że liczba modułów do zaimportowania wynosi 100. Czy w takiej sytuacji chcielibyśmy importować wszystkie po kolei? 
Tutaj z pomocą przychodzą nam pakiety, które pozwalają na tematyczną i hierarchiczną organizację wielu modułów , w spójne organizacyjnie struktury, które w sposób intuicyjny i łatwy można następnie wykorzystywać w twrozonych programach. 
Co ważne tworzenie pakietów w py jest niewiarygodnie proste.
Wystarczy utworzyć nowy folder.
np. o naziw pakiet
i stworzymy w niem _ _ init _ _ .py - plikt ten ma dwa główne zastosowania, po pierwsze jest wymagany dla py do 3.3, aby folder w którym się znajduje był traktowany przez środowisko py jako pakiet. (bez tego nie będzie widoczny pakiet i moduły). Pod drugie kod w plliku inita będzie dostępny z poziomu pakietu po dokananiu jego importu. Można więc potraktować ten plik jako odpowiednik metody init, z której korzystamy przy okazji pracy z klasami. W gruncie rzeczy nie jest pozbawione sensu traktowanie importowania pakietu z plikiem init , jako swoistej inicjalizacji pakietu i tworzenia jego instancji, gdzie w pliku init możemy zadeklarować bazowe dane i zachowanie pakietu, do których uzyskamy dostęp z poziomu pakietu po jego imporcie. 

Przenosimy moduły do folderu pakietu
![[Pasted image 20230507051745.png]]
tak też będziemy musieli wymieniać pakeity po przecinku, zatem nie rozwiązuje to naszego problemu
Możemy jednak do pliku init pakietu dodać linijkę wykorzystującą predefiniowane pole 'all', to którego przypisujemy nazwy wszystkich interesujących nas modułów:
![[Pasted image 20230507051947.png]]

Dzięki temu gdy teraz wrócimy do naszego skryput, to możemy dokonać importu wrzystkich modułów, na które wskazuje zmienna all, w ten sposób:
![[Pasted image 20230507052057.png]]

W pliku _ _ init _ _ .py pakietu, możemy też doklarować całkiem zwyczajny kod, np jakieś dane czy fn
![[Pasted image 20230507052251.png]]


I jeśli teraz wrócimy do naszego skryptu, to możemy skorzystać z tego kodu poprzez zaimportowanie naszego pakietu
![[Pasted image 20230507052358.png]]

