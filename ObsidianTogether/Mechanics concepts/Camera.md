

Gra ma dwie fazy:
1. Eksploracja
2. Combat

Jak już pokazywałam tobie wcześniej, w moim prototypie są dwie kamery

Pierwsza - renderuje POV gracza i ogólnie arene gdzie miałby być boss gdzie tło jest transparent
Druga - renderuje cały skybox pod widokiem kamery i POV gracza

Jest tutaj problem ponieważ to w aktualnej chwili nie pozwala za bardzo na możliwość eksploracji interaktywnej, jako że gracz porusza się po arenie a nie w tamtym skyboxie.

Rozwiązanie:

EKSPLORACJA
W momencie w którym gracz jest w fazie eksploracji jego inputy w arenie są lockowane a jego kamera przechodzi z trybu FPP na TPP. Widać wtedy model/sprite gracza. Wcześniejsza kamera którą ci pokazywałam że poruszała się po pathie teraz przyjmuje inputy i gracz porusza się kamerą w tym environmencie skyboxowym aż nie znajdzie momentu gdzie ma rozpocząć się combat phase

COMBAT
Gdy gracz w trakcie eksploracji znajdzie trigger który wywołuje walkę z bossem, np odpowiednią lokacje, traci kontrolę nad kamerą w skyboxie, perspektywa wraca z TPP na FPP i odzyskuje kontrole nad poruszaniem się w arenie


