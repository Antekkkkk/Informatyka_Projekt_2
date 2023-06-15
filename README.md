# Informatyka_Projekt_2
W ramach projejktu numer 2 na przedmiocie Informatyka geodezyjna stworzona została wtyczka do programu qgis w języku Python.

Wtyczkę należy wkleić do folderu plugins. Przykładowa ścieżka:
C:\Users\antek\AppData\Roaming\QGIS\QGIS3\profiles\default\python\plugins

Działanie wtyczki zaprezentujęna podstawie pliku stworzonego w Autocad, zawierającego kilka punktów. 

Po wrzuceniu pliku dxf do qgisa należy dodaćstrybuty geometrii, tak jak na zdjęciu

![image](https://github.com/Antekkkkk/Informatyka_Projekt_2/assets/129069654/4ed23271-7da1-4083-86bf-c0a2d149d2ec)

A następnie uzupełnić okienko warstwą z plikami i układem. Ważne jest by zaznaczyć ukłąd projektu. 

![image](https://github.com/Antekkkkk/Informatyka_Projekt_2/assets/129069654/eb0c6414-a126-46c9-9020-39b3703af92e)


Uwaga! Żeby program działał poprawnie, kolumny tabeli atrybutów powinny być nazwane w odpowiedni sposób - nazwy w kolumnie 'EntityHanle',
a współrzędne X,Y,Z kolejno 'xcoord', 'ycoord' i 'zcoord'.

![image](https://github.com/Antekkkkk/Informatyka_Projekt_2/assets/129069654/fe9fc1d4-2099-4958-bd02-0876ffa0fa48)

Na tak przygotowanych plikach można użyć wtyczki. Zaznaczamy wybrane punkty i odpalamy wtyczkę. Jeśli chcemy policzyć przewyższenie, trzeba zaznaczyćdokładnie 2 punkty. Żeby policzyć pole, należy wybrać 3 punkty lub więcej. Jednostki i przyciski podpisane są bezpośrednio w okienku wtyczki. Żeby wyczyścić zawartość wtyczki należy kliknąć reload plugin.

Ważne! W okienku wybierz warstwę należy wybrać warstwę z dodaną geometrią, inaczej liczenie przewyższeń może nie zadziałać. 

Wygląd wtyczki i przykładowy wynik:

![image](https://github.com/Antekkkkk/Informatyka_Projekt_2/assets/129069654/86d54083-f08e-41d5-9278-38d200e265e6)

Znane błędy:
 - Wtyczka nie działa gdy nazwy kolumn mająinne nazwy, co może się stać gdy punkty sąeksportowane w innym formacie niż dxf. 
 - przy bardzo dużej ilości punktów kod na pole potrafi dawać dziwne wyniki

