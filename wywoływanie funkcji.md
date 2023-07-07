po zakończonym bloku kodu funkcji dwie linie puste

po prostu piszemy nazwę fn i nawiasy by ją wywołać. Co ważne, wykorzystanie pary nawiasów okrągłych jest istotne gdy chcemy aby fn została wywołana.

fn to obj typu function, możemy się odwołaś do niej jako do obj, bez jej wywoływania, nie wpisując na końcu nawiasów okrągłych. Dzięki temu można fn np przypisać do jakiejś zmiennej. Zmienna ta może też stać się uchwytem tej fn.
x = fn
x()
