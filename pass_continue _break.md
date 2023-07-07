instrukcje te mają sens tylko wtedy gdy zagnieżdzone są w blokach kodu innych instrukcji
pass - element zastępczy instrukcji, wykorzystywany gdy składnia języka wymaga jakiegoś bloku kodu, ale nie mamy nic istotnego do wyrażenia. Instrukcja pass jest tym samym dla instrukcji czym typ None dla obiektów - po prostu sposobem na wyrażenie, dosłownie niczego

for i in range(10):
	pass

continue - powoduje pominięcie reszty godu w zagnieżdzonym bloku i powrót do nagłówka pętli

for liczba in range(5):
	if liczba==2:
		continue
	print(liczba)


break (tak jak poprzednie tylko w pętlach) - natychmiastowe przerwanie pętli i zignorowanie pozostałych jej działań do wykonania. Następnie skupia się na pierwszej linii kodu, występującego po przerwanej pętli
W przypadku tej instr. blok kodu else po pętli nie wykona się

#break  
  
znaki = []  
print('zliczator znakow')  
while True:  
    dane_wejsciowe = input("Dane wejsciowe: ")  
    if dane_wejsciowe == "red pill":  
        break  
    else:  
        znaki+=list(dane_wejsciowe)  
  
print("Wystapienia: ",end=' ')  
for element in sorted(set(znaki)):  
    print(element,'=',znaki.count(element),end=' | ')