funkcja może przyjmować dane,ale nie musi. Fn może przetwarzać dane, ale nie musi. Fn może też   zwracać dane, ale nie musi.

def(definiuję)  fn()(funkcję o nazwie 'funkcja',która...):  
    ...wykonuje inst i wyrażenia tutaj opisane

definiujemy funkcje o określonej nazwie, która definiuje zagnieżdzone instrukcje w jej bloku kodu

fn w py nie istnieje, dopóki interpreter nie dojdzie w kodzie do słowa 'def', dzieje się tak dlatego, że 'def' jest instr wykonywalną, co pozwala zdefiniować kilka wariantów tej samej funkcji w drabince instrukcji warunkowych if, elif, else. I skorzystać akurat z tego wariantu, który zostanie wykonany po spełnieniu danego ifa

x =10  
y = 9  
if x > y:  
    def function():  
        print("x jest większe od y")  
else:  
    def function():  
        print("x jest mniejsze od y")  
  
function()

kiedy interpreter py dotrze do fn 'def' i ją wykona to w rezultacie zostaje utworzony nowy obiekt reprezentujacy fn, do którego zostaje przypisana nazwa fn, która nie różni się od nazwy najzwyklejszej zmiennej. Możemy bowiem przechowywać nazwy fn np. w listach i korzystać z nich tak jak ze zwykłych zmiennych

konwencja nazewnictwa funkcji:
wyłącznie małe litery, 
gdy więcej wyrazów, oddzielamy podkreślnikami

dodatkowo pomiędzy nagłówkiem fn, a poprzedzającym go kodem, powinny być dwie puste linie