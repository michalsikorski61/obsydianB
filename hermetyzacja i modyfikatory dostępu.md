hermetyzacja (enkapsulacja) - zapewnia kontrolę nad widocznością i dostępem do danych zdefiniowanych w klasach, z zewnątrz - czyli albo z poziomu obiektu klasy, albo z poziomu instancji tej klasy. Często bowiem jest tak, że instancje klas przechowują dane wrażliwe, do których luźny dostęp nie jest najlepszym pomysłem i powinien być zdecydowanie ograniczony. Enkapsulacja pozwala bowiem ograniczyć dostęp do danych obecnych w jednym obiekcie, z poziomu innego obiektu. Przy zachowaniu porządanego działania programu. 
W py implementujemy mechanizm hermetyzacji z wykorzystaniem modyfikatorów dostępu:
public - niewjawny i automatycznie wykorzystywany
protected - dostęp w klasie i klasach dziedziczących ( _ )
private - wyłącznie w klasie ( _ _ )

![[Pasted image 20230504110459.png]]

w powyższym kodzie atryb projekt jest chroniony, a wynagrodzenie jest prywatny

możemy uzyskać dostęp do prywatnych atr z wykorzystaniem publicznych metod lub specjalnego odwołania do prywatnego atry
![[Pasted image 20230504110734.png]]

![[Pasted image 20230504110814.png]]
dodając przed nazwą atryb z private nazwę jego klasy poprzedzoną pojedynczym podkreśleniem możemy niejako obejść ukrycie atryb i uzyskać do niego dostęp w ramach  wyjątkowych okoliczności. 

btw. zamiast super (jako inicjalizacji klasy dziedziczonej w dziedziczącej) można użyć nazwy klasy dziedziczonej np. Firma._ _ init_ _ (self)
![[Pasted image 20230504111945.png]]
zalety hermetyzacji
- zwiększamy bezp
- zapewniamy sobie możliwość ukrywania danych na różnych poziomach pracy z kodem
- upraszczamy proces tworzenia oprogramowania poprzez ograniczenie liczby interakcji pomiędzy obiektami i ich atrybutami
- zwiększamy poziom estetyki kodu poprzez przetwarzanie danych za pomocą instancji klas i ich metod
