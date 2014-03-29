Full Polish Keyboard Layout for Android
=======================================

(It's a Polish keyboard layout, no point in the docs being in English.)

To jest mapa klawiatury dla ludzi z fizyczną klawiaturą podłączoną do androidowego urządzenia (np. z androidowym laptopem/netbookiem).



Instalacja
----------

Zbudowaną paczkę można pobrać z http://ep09.pld-linux.org/~mmazur/fpk/fpk.apk

Alternatywny opis instalacji wraz z obrazkami jest tu:
http://jogger.pl/redirect/mmazur/2014/03/29/pelna-polska-fizyczna-klawiatura-do-androida/

  
Plik fpk.apk trzeba wrzucić na urządzenie, odpalić, zainstalować (musi być zaznaczone na urządzeniu «Ustawienia | Zabezpieczenia | Nieznane źródła»), po czym w ustawieniach wybrać klawiaturę fizyczną «Polski (programisty) - Full Polish Keyboard». Powinno działać.

Posiadacze urządzeń w których obok prawego klawisza Alt znajduje się klawisz Menu (trzy małe kwadraty jeden nad drugim), mogą wybrać wersję «Polski (programisty), bez klawisza Menu», która jest identyczna do powyższej z tą różnicą, że klawisz Menu działa tak samo jak prawy Alt, więc jeśli podczas szybkiego pisania się spudłuje kciukiem i trafi w Menu zamiast Alt, efekt będzie taki, jak gdyby się wcale nie spudłowało.

**Uwaga:** autor przetestował przemapowanie klawisza Menu na swoim Lenovo A10. Jeśli ktoś chciałby zgłosić, że działa mu to (bądź nie) na jakimś innym sprzęcie, to proszę o maila na mmazur@kernel.pl.



Budowanie
---------

Najpierw trzeba ściągnąć sdk i wrzucić sobie *sdk/tools* w $PATH, po czym:

    cd FullPolishKeyboard
    android update project -t android-19 -p .
    mkdir src
    ant debug
  
Wynikowy plik to *bin/full_polish_keyboard-debug.apk*.



