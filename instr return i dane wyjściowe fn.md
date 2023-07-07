by funkcja coś zwracała, tak by można było to coś przetwarzać w dalszej części programu należy użyć instrukcji return, której użycie wygląda następująco
![[Pasted image 20230503195042.png]]
Po wywołaniu tak napisanej fn, wynik nie zostanie wyświetlony na standardowe wyjście, ponieważ instrukcja return zwraca adres obiektu, a nie przekazuje go do strumienia. Dlatego możemy przypisać do zwracanego obj nową zmienną. 

W tym momencie instr return zwraca obj reprezentowany przez referencję o nazwie wynik, możemy natomiast zwracać sam wynik zrealizowanego wyrażenia w postaci potęgowania
![[Pasted image 20230503195550.png]]
w tej sytuacji return zwróci wynik wyrazenia napisanego po instrukcji, czyli obiekt reprezentujący wynik tego potęgowania, a raczej adres do tego obiektu

Instr też kończy działanie fn, nie tylko zwraca jej wynik.
za pomocąreturn możemy też zwracać kilka obj

![[Pasted image 20230503195943.png]]