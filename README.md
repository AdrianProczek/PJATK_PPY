Imię i nazwisko: Adrian Proczek
Nr studenta: s25179

Ten projekt to prosta implementacja klasycznej gry w węża za pomocą biblioteki graficznej turtle w Pythonie. W grze sterujemy wężem, który porusza się po ekranie, zjada jedzenie i rośnie w długość. Celem gry jest zdobywanie punktów poprzez zjadanie jedzenia, unikając zderzeń z ścianami lub własnym ciałem. Gra zapisuje również najwyższy osiągnięty wynik.

Moduły i Klasy:

main.py to główny skrypt uruchamiający grę.
Konfiguracja i Inicjalizacja:
    -Konfiguracja Ekranu: Inicjalizuje okno gry z czarnym tłem i tytułem.
    -Obiekty Gry: Tworzy obiekty dla węża, jedzenia i tablicy wyników.
    -Sterowanie: Ustawia sterowanie klawiaturą do poruszania węża.

Pętla Gry:
    -Wykonanie Pętli Gry: Ciągle aktualizuje ekran, porusza węża i sprawdza kolizje.
    -Detekcja Kolizji: Sprawdza, czy wąż zjadł jedzenie, uderzył w ścianę lub zderzył się sam ze sobą.

food.py definiuje klasę Food, która reprezentuje jedzenie, które zjada wąż.
Klasa Food:
    -Inicjalizacja: Tworzy małe zielone koło reprezentujące jedzenie.
    -refresh(): Przesuwa jedzenie na losową pozycję na ekranie.

snake.py definiuje klasę Snake, która reprezentuje węża w grze.
Klasa Snake:
    -Inicjalizacja: Tworzy węża z początkowym zestawem segmentów.
    -create_snake(): Ustawia początkowe segmenty węża.
    -add_segment(): Dodaje nowy segment do węża.
    -extend(): Wydłuża węża, dodając nowy segment na końcu.
    -move(): Porusza węża do przodu, aktualizując pozycję każdego segmentu.
    -Metody Kierunkowe (up, down, left, right): Zmieniają kierunek głowy węża.

scoreboard.py definiuje klasę Scoreboard, która obsługuje wyświetlanie wyniku i najwyższego wyniku.
Klasa Scoreboard:
    -Inicjalizacja: Ustawia tablicę wyników i odczytuje najwyższy wynik z pliku.
    -update_scoreboard(): Aktualizuje wyświetlany wynik i najwyższy wynik.
    -score_up(): Zwiększa wynik o jeden i aktualizuje wyświetlacz.
    -game_over(): Wyświetla komunikat "GAME OVER".
    -reset(): Resetuje bieżący wynik i aktualizuje najwyższy wynik, jeśli jest konieczne.

Użycie:
Aby uruchomić grę, wykonaj skrypt main.py. Użyj klawiszy strzałek do sterowania kierunkiem węża. Celem jest zjedzenie jedzenia, wydłużenie węża i osiągnięcie jak najwyższego wyniku.
