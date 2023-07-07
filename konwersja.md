Zmienną i jej typ możemy zmieniać dynamicznie. Znaczy to główie dla nas tyle, że za wykonując przypisania, wczytania i inne operacje na zmiennych, możemy mniej lub bardziej świadomie zmieniać typ zmiennych.
licz = 3
print(licz, type(licz))
licz = licz / 2
print(licz, type(licz))

Zmienna raz może być liczbą, raz sterem
bylaLiczba = 7.5
print(bylaLiczba, type(bylaLiczba))
bylaLiczba = input("Podaj cokolwiek ")
print(bylaLiczba, type(bylaLiczba))

str (lub cokolwiek) na int 
int("3") - funkcja, która zamienia łańcuch na liczbę całkowitą,
którą on reprezentuje,


str (lub cokolwiek) na float
float(cokolwiek) - funkcja, która zamienia łańcuch na liczbę
zmiennoprzecinkową, którą on reprezentuje


a = "3,14" 
a = float(a) - błąd bo przecinek, a nie kropka
a = "30.3" 
a = int(a) - błąd, nie przekonwertujemy na int, tekstu z floatem, musimy najpierw na float