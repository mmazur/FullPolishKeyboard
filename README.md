FullPolishKeyboard
==================

Full Polish Keyboard Layout for Android

(It's a Polish keyboard layout, no point in the docs being in English.)

To jest mapa klawiatury dla ludzi z *fizyczną* klawiaturą podłączoną do androidowego urządzenia.


Pobieranie
----------

Będzie, póki co trzeba sobie samemu zbudować.


Budowanie
---------

Najpierw trzeba ściągnąć sdk i wrzucić sobie 'sdk/tools' w $PATH, po czym:

    cd FullPolishKeyboard
    android update project -t android-19 -p .
    mkdir src
    ant debug
  
Wynikowy plik będzie w 'bin'.


Instalacja
----------
  
Plik 'full_polish_keyboard-debug.apk' trzeba wrzucić na urządzenie, odpalić, zainstalować (musi być zaznaczone na urządzeniu 'Ustawienia | Zabezpieczenia | Nieznane źródła'), po czym w ustawieniach wybrać klawiaturę fizyczną 'Polish (Programmers+) - Full Polish Keyboard'. Powinno działać.

