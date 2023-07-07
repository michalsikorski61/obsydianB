pętla for to doskonały itelator - czyli kontrukcja do przechodzenia przez kolejne elementy itelowarnej kolekcji

for(dla) elementu in(w) obj_iterrowalnym:
	wykonaj zawarte tutaj instrukcje (w bloku)
else (w przeciwnym razie):
	wykonaj zawarte tutaj instrukcje
gdy pętla zakończy swoje działaniee

wyraz = "sdfsfs"
for lit in wyraz:
	print(lit,end=". ")

suma=0  
for liczba in range(1,25):  
    print(suma,end=" | ")  
    suma +=liczba  
else:  
    print(f"suma: {suma}")