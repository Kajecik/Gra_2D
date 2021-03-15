# Gra_2D

# Kod
Gra zostałą napisana w jeżyku python z zaimportowanymi bibliotekami tkinter i random.

## Klasa Snake()
Określa ciało Snake. Pierwsza pętla uzupełnia współrzędne każdej części ciała Snake, Druga zamalowuje je kwadratami na planszy.

## Klasa Food()
Określa ciało 'jabłka'. Zawiera koordynaty, a za pomocą canvas pojawia się na planszy

## Funkcja next_turn()
Za pomocą pierwszej instrukcji warunkowej i klasy canvas zmieniam położenie kwadratów. Za pomocą drugiej instrukcji warunkowej sprawdzam czy Snake 'trafił' na jabłko.
Za pomocą trzeciej instrukcji warunkowej sprawdzam czy w tym czasie wystąpiła jakaś kolizja w grze, jeśli tak wzywam funkcję za to odpowiedzialną która kończy grę, jeśli nie - gra toczy się dalej

## Funkcja change_direction()
Funkcja odpowiedzialna za przechwytywanie zmiany kierunku poruszania się Snake.

## Funkcja check_collisions()
Sprawdza czy w trakcie gry wystąpi jakaś kolizja. Pierwsza instrukcja warunkowa sprawdza czy nie nastąpiło zderzenie ze ścianą okna. Druga - czy Snake nie 'naszedł' na siebie.

## Funkcja game_over()
Usuwa wszystko i wyświetla napis "Koniec gry"

## Pozostała część programu
W dalszej części kodu tworzę okienko, za pomocą window.bind przechwytuje dane wejsciowe z klawiatury (zmianę kierunku trasy Snake). Tworzę obiekty klasy Snake i Food.
Na końcu wywołuję funkcję next_turn() która do momentu kolizji będzie wywoływała sama siebie w nieskończoność.
