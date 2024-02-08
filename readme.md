**Autorzy:**

Marcin Królikowski, nr albumu 294262\
Patryk Piotrowski, nr albumu 315564

# Spis treści {#spis-treści .TOC-Heading}

[**1.** **Wprowadzenie** [3](#_Toc136015890)](#_Toc136015890)

[**2.** **Zakres prac** [3](#_Toc136015891)](#_Toc136015891)

[**3.** **Założenia projektowe** [4](#_Toc136015892)](#_Toc136015892)

[**4.** **Harmonogram prac i podział ról**
[4](#_Toc136015893)](#_Toc136015893)

[**5.** **Podstawy teoretyczne i zastosowane rozwiązania**
[5](#_Toc136015894)](#_Toc136015894)

[**7.** **Podsumowanie zastosowanego rozwiązania**
[12](#_Toc136015895)](#_Toc136015895)

[**8.** **Źródła** [13](#_Toc136015896)](#_Toc136015896)

1.  []{#_Toc136015890 .anchor}**Wprowadzenie**

Przedmiotem projektu jest gra 3D typu Tower Defense na komputery z
systemem Windows. Jest to popularny gatunek gier, w którym zadaniem
gracza jest obrona swojej bazy przed atakami przeciwnika, za pomocą
umiejętnego rozstawiania wież strzelających do napastników. Swoją
popularność ten gatunek gier zawdzięcza prostej mechanice, ale
jednocześnie wymaganej od gracza umiejętności planowania i strategii.

Istnieje wiele gier typu Tower Defense na różnych platformach.
Najpopularniejsze z nich to: *Kindgdom Rush*, *Bloons Tower Defense*,
czy *Plants vs. Zombies*.

Na rynku dostępnych jest wiele silników gier, pozwalających na
realizację projektu. Do najpopularniejszych należą:

a.  Unreal Engine -- często używany do tworzenia gier AAA, oferujący
    zaawansowane narzędzia graficzne i edytory, pozwalające na tworzenie
    w pełni funkcjonalnych gier 3D. Silnik obsługuje język programowania
    C++, co pozwala na optymalizację wydajności gry, szczególnie przy
    dużych projektach. Unreal Engine oferuje wiele gotowych modułów i
    dodatków, które ułatwiają pracę.

b.  Godot Engine -- to open-source'owy silnik gier, oferujący prosty i
    intuicyjny interfejs. Silnik obsługuje języki programowania takie
    jak, C++ i C#, co daje dużą elastyczność w wyborze zastosowanej
    technologii. Posiada wiele wbudowanych narzędzi i modułów
    ułatwiających prace.

c.  Unity -- popularny silnik gier posiadający prosty i intuicyjny
    interfejs. Obsługuje język programowania C#. Podobnie jak pozostałe
    silniki, posiada wiele wbudowanych narzędzi i modułów ułatwiających
    projektowanie. Na uwagę zasługuje duże wsparcie społeczności i
    liczne materiały edukacyjne, co czyni go popularnym wyborem wśród
    początkujących. Unity wspiera wieloplatformowość i pozwala w łatwy
    sposób przenosić gry na inne platformy.

```{=html}
<!-- -->
```
2.  []{#_Toc136015891 .anchor}**Zakres prac**

Założeniem projektu jest wykonanie następujących prac:

-   zaprojektowanie systemu siatki, na którym będzie znajdować się świat
    gry,

-   implementacja logiki gry i mechaniki strzelania,

-   implementację przeciwników i ich pojawiania się falowo,

-   stworzenie systemu ekonomii gry, pozwalający na zakup nowych wież,

-   zaprojektowanie poziomów, elementów scenografii, efektów
    dźwiękowych,

-   implementacja interfejsu użytkownika

> Z uwagi na ograniczenia wynikające z dwuosobowego zespołu, w zakres
> prac nie wchodzi stworzenie modeli 3D tekstur, obiektów i efektów
> dźwiękowych. Zostaną użyte darmowe modele udostępnione przez
> społeczność.

3.  []{#_Toc136015892 .anchor}**Założenia projektowe**

Do realizacji zadania został wykorzystany silnik gier Unity, z uwagi na
jego popularność, bogatą dokumentację, duże wsparcie społeczności i
przede wszystkim dużą ilość dostępnych materiałów do nauki.

Założono, że projektowana gra ma spełniać warunki:

-   grafika 3D,

-   świat gry zostanie umieszczony na siatce,

-   siatka posiadać będzie punkt początkowy, w którym będą pojawiać się
    przeciwnicy, oraz punkt docelowy (bazę), którą próbują zaatakować,

-   zadaniem gracza jest obrona celu ,

-   przeciwnicy gracza chcą zniszczyć cel broniony przez gracza,
    pojawiają się falami,

-   przeciwnicy mają poruszać się po wyznaczonych ścieżkach,

-   gracz ma mieć możliwość stawiania budynków obronnych chroniących
    bazę przez przeciwnikami,

-   wprowadzenie opóźnienia budowania wież, ograniczonych zasobów, aby
    urozmaicić rozgrywkę,

-   kreskówkowa grafika bez dużej ilości detali (low-poly) i bez
    wysokich wymagań sprzętowych.

> **Odczucia gracza:**
>
> Gra ma wymagać od gracza strategicznego myślenia i opracowania
> specjalnej taktyki pozwalającej na wygraną (obronę bazy), poprzez
> umiejętne stawianie budynków obronnych, przy wykorzystaniu
> ograniczonych zasobów (złota).

**Tematyka:**

Gra osadzona będzie w czasach średniowiecznych z elementami fantastyki,
gdzie grupa rabusiów przybyła do naszego królestwa, aby zrabować złoto
zgromadzone w zamku.

**Dane techniczne:**

Platforma: Windows 64-bit

Rozdzielczość: 1920x1080 16:9

Sterowanie: Mysz

4.  []{#_Toc136015893 .anchor}**Harmonogram prac i podział ról**

> Projekt wykonywany jest w dwuosobowym zespole. Podział prac podczas

  ---------------------------------------------------------------------------
  **Lp**   **Pozycja**                                   **Odpowiedzialny**
  -------- --------------------------------------------- --------------------
  1        Określenie wymagań i założeń projektu         MKR, PPI

  2        Dyskusja o sposobie realizacji projektu       MKR, PPI

  3        System kontroli wersji                        PPI

  4        Projekt siatki                                MKR

  5        Import modeli i tekstur                       PPI

  6        Implementacja obsługi myszy                   MKR

  7        Dodanie przeciwników                          MKR

  8        Znajdowanie ścieżki (pathfinding)             MKR

  9        System ekonomii                               PPI

  10       Punkty życia przeciwników                     PPI

  11       Refaktoryzacja, poprawa błędów                PPI

  12       Zaprojektowanie poziomu, balans gry           MKR

  13       Opóźnienie budowania                          MKR

  14       Licznik czasu i przejście do kolejnego        MKR
           poziomu                                       

  16       Efekty wizualne i post processing             PPI

  17       Efekty dźwiękowe                              MKR

  18       Licznik czasu i przejście do kolejnego        MKR
           poziomu                                       

  19       Testy i naprawa błędów                        MKR, PPI

  20       Kompilacja                                    MKR

  21       Przygotowanie raportu                         MKR

  22       Przygotowanie prezentacji                     PPI
  ---------------------------------------------------------------------------

5.  []{#_Toc136015894 .anchor}**Podstawy teoretyczne i zastosowane
    rozwiązania**

**Kontrola wersji i synchronizacja**

> Podstawowym narzędziem wykorzystanym do stworzenia projektu była
> platforma GitHub do kontroli wersji. GitHub umożliwił skuteczną
> współpracę zespołu i zarządzanie kodem projektu. Pozwolił również na
> bezproblemowy powrót do poprzedniej, stabilnej wersji gry po
> napotkaniu błędów, spowodowanych wprowadzeniem nowych rozwiązań.
>
> ![Obraz zawierający tekst, zrzut ekranu, oprogramowanie,
> Oprogramowanie multimedialne Opis wygenerowany
> automatycznie](.//media/image1.png){width="6.3in"
> height="2.6555555555555554in"}
>
> *Rysunek 1. Klient GitHub Desktop użyty do kontroli wersji*
>
> **Modele 3D i dźwięk**
>
> Do wykonania projektu skorzystano z darmowych obiektów 3D
> udostępnionych przez społeczność w Unity Asset Store
> (assetstore.unity.com) oraz plików dźwiękowych z biblioteki freesound
> (freesound.org). Unity Asset Store zintegrowany jest z edytorem Unity
> i pozwala na bezpośredni import zakupionych modeli do projektu.
> Wszystkie źródła zostały umieszczone w ostatnim rozdziale.
>
> ![Obraz zawierający tekst, zrzut ekranu, oprogramowanie,
> Oprogramowanie multimedialne Opis wygenerowany
> automatycznie](.//media/image2.png){width="6.3in"
> height="3.408333333333333in"}
>
> *Rysunek 2. Unity Asset Store*
>
> **Programowanie w Unity**
>
> Do stworzenia gry wykorzystano silnik Unity, który dostarczył
> potrzebne narzędzia do implementacji logiki gry. Mechanika gry i
> zachowanie wszystkich obiektów bazuje na stworzonych na potrzeby
> projektu skryptach napisanych w C#. Dzięki umieszczonym w skryptach
> polom *serializefield* osługiwanymi przez Unity możliwe było wygodne
> konfigurowanie parametrów zachowania obiektów i mechaniki gry z
> poziomu edytora Unity.
>
> ![](.//media/image3.png){width="6.285416666666666in"
> height="3.672222222222222in"}
>
> *Rysunek 3. Prefabrykat przeciwnika i powiązane z nim skrypty wraz z
> udostępnionymi do edycji polami serializedfield*
>
> **Optymalizacja i testowanie**
>
> Istotnym aspektem projektu było zapewnienie płynnej rozgrywki,
> niezależnie od sprzętu, na którym zostanie uruchomiona gra. Aby
> spełnić ten warunek, wykorzystano tekstury i modele o niskim poziomie
> szczegółowości i detalach, w stylu „kreskówkowym". Po stronie kodu,
> głównym wyzwaniem optymalizacyjnym było stworzenie fali przeciwników
> bez nadmiernego obciążenia zasobów sprzętowych. W tym celu
> wykorzystaliśmy technikę poolingu obiektów (ang. object pooling),
> która polega na stworzeniu puli obiektów, które są tworzone podczas
> uruchamiania gry i w zależności od osiągnięć gracza włączane lub
> wyłączane. W trakcie testów aplikacji metoda ta była znacząco
> wydajniejsza niż tworzenie i niszczenie obiektu każdego przeciwnika
> pojawiającego się na mapie.
>
> ![](.//media/image4.png){width="6.285416666666666in"
> height="2.928472222222222in"}
>
> *Rysunek 4. Pula przeciwników na poziomie 1. Aktywnych jest 3
> przeciwników z 5 obiektowej puli.*

6.  **Prezentacja i opis otrzymanych wyników**

**System siatki**

Podstawowym elementem gry jest system siatki, składający się z kafelków.
Każdy kafelek posiada unikalną współrzędną w świecie gry. Współrzędne
wykorzystywane są w innych elementach gry: do stawiania budowli oraz
odnajdywania ścieżki przez przeciwników.

![Obraz zawierający zrzut ekranu, kwadrat, piksel Opis wygenerowany
automatycznie](.//media/image5.png){width="3.363183508311461in"
height="3.1310345581802275in"}

Rysunek 5. System siatki z zaznaczonymi współrzędnymi

**Gameplay**

Gra składa się z 3 poziomów, warunkiem wygranej każdego poziomu jest
zachowanie dodatniej ilości złota (wartość Gold) przez wyznaczony czas
(remaining time). Gra kończy się przegraną gdy nastąpi wyzerowanie
zgromadzonego złota gracza przez przeciwników. W przypadku wygranej gra
przechodzi do kolejnego poziomu, w przypadku przegranej poziom
rozpoczyna się od nowa.

Gracz może budować budynki obronne (wieże) jedynie na niezajętych przez
inne obiekty kafelkach mapy przez kliknięcie lewym przyciskiem myszy na
wolnym kafelku. Każdy kafelek ma unikalną współrzędną (x,y). Na jednym
kafelku może znajdować się tylko jedna wieża.

Kafelki zajęte przez obiekty otoczenia (ścieżka, scenografia, baza
gracza i przeciwnika) są wyłączone z możliwości budowania na nich wież
(mają wyłączony parametr isPlaceable).

![](.//media/image6.jpeg){width="6.29375in"
height="3.561111111111111in"}

*Rysunek 6. Zaznaczony obszar mapy gry z oznaczonymi zajętymi miejscami
niedostępnymi do budowy wieży.*

**Interfejs użytkownika**

Interfejs zawiera informacje o ilości zgromadzonego złota oraz o czasie
pozostałym do końca poziomu.

![](.//media/image7.jpeg){width="6.29375in"
height="3.561111111111111in"}

Rysunek 7. Interfejs użytkownika

**System ekonomii**

Gracz na początku każdego poziomu otrzymuje początkową wartość złota
(Gold). Stan konta gracza może ulec zmianie poprzez:

-   budowa wieży odejmuje z konta gracza 75 sztuk złota,

-   wyeliminowanie przeciwnika dodaje do konta gracza 25 sztuk złota,

-   dotarcie przeciwnika do bazy gracza odejmuje z konta gracza 25 sztuk
    złota.

Minimalny stan konta gracza to 0 sztuk złota. Wieża nie może zostać
wybudowana, jeżeli gracz nie ma wystarczającej ilości złota.

**Wieże i przeciwnicy**

Przeciwnicy pojawiają się w punkcie startowym i poruszają wyznaczoną
ścieżką. Każdy przeciwnik posiada punkty życia (maxHitPoints), które
wyznaczają liczbę trafień wieży potrzebną do jego wyeliminowania z mapy
gry oraz porusza się z określoną prędkością (speed). Przeciwnicy
pojawiający się na mapie wraz z upływem czasu mają więcej punktów życia
(maxHitPoints + difficultyRamp).

![](.//media/image8.png){width="4.386111111111111in"
height="1.2979166666666666in"}

*Rysunek 8. Baza gracza (niebieski) i punkt startowy przeciwników
(czerwony).*

Wieże mają ograniczony zasięg ataku (range). Jedno trafienie wieży
odejmuje jeden punkt życia przeciwnika. Jeżeli w zasięgu wieży jest
kilka celów, to wieża atakuje cel najbliższy sobie. Od momentu
postawienia wieży przez gracza na wolnym kafelku, do jej gotowości do
ataku trwa budowanie wieży. Czas ten jest określony przez zmienną
buildDelay.

![](.//media/image9.png){width="5.061111111111111in"
height="1.7458333333333333in"}

*Rysunek 9. Wieża w trakcie budowy (po lewej) i zbudowana wieża gotowa
do ataku (po prawej).*

![](.//media/image10.jpeg){width="6.289583333333334in"
height="3.2194444444444446in"}

*Rysunek 10. Wieża i jej zasięg. W zasięgu wieży znajduje się dwóch
przeciwników, wieża atakuje cel bliższy sobie.*

**Post processing**

Aby ulepszyć efekty wizualne i jakość grafiki, a tym samym poprawić
odczucia gracza zastosowano post-processing. Jest to technika obejmująca
szereg różnych efektów, takich jak filtry kolorów, rozmycie, efekty
świetlne. Poniżej przedstawiono porównanie poziomu z włączonym i
wyłączonym post-processingiem.

![Obraz zawierający zabawka Opis wygenerowany
automatycznie](.//media/image11.png){width="6.3in"
height="3.2423611111111112in"}

*Rysunek 11. Poziom z post-processingiem*

![Obraz zawierający zabawka, Minecraft Opis wygenerowany
automatycznie](.//media/image12.png){width="6.3in"
height="3.2604166666666665in"}

*Rysunek 12. Poziom bez post-processingu*

**Kompilacja gry i sposób uruchomienia**

Gra została skompilowana na komputery PC z systemem Windows 64-bit. W
celu uruchomienia gry, należy pobrać katalog Build i uruchomić plik
wykonywalny unity-game-project.exe. Plik jest dostępny w repozytorium na
platformie GitHub:

<https://github.com/piotrowskipatryk/unity-game-project/tree/main/Build>

Aby zakończyć działanie programu, należy skorzystać ze skrótu
klawiszowego Alt + F4.

7.  []{#_Toc136015895 .anchor}**Podsumowanie zastosowanego rozwiązania**

W ramach projektu udało stworzyć się funkcjonalną grę 3D typu tower
defense i zaimplementować charakterystyczne dla tego gatunku mechaniki i
rozwiązania. Projekt był również okazją do przejścia procesu wytwarzania
oprogramowania, od sprecyzowania początkowych założeń, przez wybór
odpowiednich narzędzi, produkcję oprogramowania i skonfrontowanie
otrzymanych wyników z początkowymi założeniami.

Gra posiada pewne uproszczenia, które w kolejnej wersji można będzie
rozwinąć, np. dodanie menu gry, kolejnych poziomów, nowych modeli
przeciwników i rodzajów budowli, elementów scenografii lub możliwości
ulepszania wież. W trakcie prac wykorzystano darmowe zasoby modeli
udostępnione przez społeczność, jednak w przyszłości można wykorzystać
również własne modele przygotowane w np. w Blender. Przygotowane w
ramach projektu rozwiązania, mogą posłużyć za bazę do rozbudowy gry,
użyte mechaniki są dobrze skalowalne. Rozwijając projekt dalej, można
będzie za pomocą funkcji wbudowanych w silnik Unity wykonać port na
urządzenia mobilne.

8.  []{#_Toc136015896 .anchor}**Źródła**

**audio:**

a)  https://freesound.org/people/sonically_sound/sounds/624644

b)  https://freesound.org/people/TheoJT/sounds/511311

c)  https://freesound.org/people/LittleRobotSoundFactory/sounds/270309

**modele przeciwników i scenografii:**

a)  *Forest - Low Poly Toon Battle Arena / Tower Defense Pack*
    <https://assetstore.unity.com/packages/3d/environments/forest-low-poly-toon-battle-arena-tower-defense-pack-100080>

b)  *Goblin & Cannon*
    <https://assetstore.unity.com/packages/3d/environments/fantasy/goblin-cannon-145437>

c)  *Meshtint Free Tile Map Mega Toon Series*
    <https://assetstore.unity.com/packages/3d/environments/meshtint-free-tile-map-mega-toon-series-153619>

d)  *Meshtint Free Boximon Cyclopes Mega Toon Series*
    <https://assetstore.unity.com/packages/3d/characters/meshtint-free-boximon-cyclopes-mega-toon-series-154436>

e)  *Meshtint Free Turret Tower Mega Toon Series*
    <https://assetstore.unity.com/packages/3d/environments/fantasy/meshtint-free-turret-tower-mega-toon-series-155310>
