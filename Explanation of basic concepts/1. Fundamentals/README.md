## 1. Matrices & Linear Algebra Fundamentals

### About

In mathematics, a matrix is a __rectangular array of numbers, symbols, or expressions, arranged in rows and columns__. A matrix could be reduced as a submatrix of a matrix by deleting any collection of rows and/or columns.

![matrix-image](https://upload.wikimedia.org/wikipedia/commons/b/bb/Matrix.svg)

## 2. Hash Functions, Binary Tree, O(n)

__Computational Complexity O(n)__ refers to the amount of resources, typically time or memory, that an algorithm requires to complete as a function of the size of its input. It is commonly expressed using Big O notation, which provides an upper bound on the algorithm's growth rate as input size increases, allowing us to evaluate its efficiency.

- O(1) – Stała złożoność, np. dostęp do elementu tablicy po indeksie.
- O(n) – Liniowa złożoność, np. jednokrotne przejście przez tablicę.
- O(n2) – Kwadratowa złożoność, np. dwie zagnieżdżone pętle for.
- O(logn) – Logarytmiczna złożoność, np. algorytmy dzielące przestrzeń wyszukiwania na pół (binary search).
- O(nlogn) – Liniowo-logarytmiczna złożoność, np. efektywne algorytmy sortujące jak merge sort.

## 3. Relational Algebra, DB Basics

Relational Algebra i DB Basics to podstawowe pojęcia związane z bazami danych, które pomagają w organizowaniu, manipulowaniu i zarządzaniu danymi w systemach zarządzania bazami danych (DBMS). Oto krótkie wyjaśnienie tych terminów:

__Relational Algebra__ (Algebra Relacyjna)
Algebra relacyjna to zbiór operacji, które są używane do przetwarzania i manipulowania danymi w relacyjnych bazach danych. Jest to formalny język zapytań, który stanowi podstawę dla bardziej zaawansowanych systemów zapytań, takich jak SQL. W algebrze relacyjnej operacje są wykonywane na relacjach (tabelach), które składają się z wierszy (krotek) i kolumn (atrybutów). Operacje algebry relacyjnej zwracają nowe relacje jako wynik.

Niektóre podstawowe operacje w algebrze relacyjnej to:

 - Selekcja (Selection): Wybieranie wierszy z tabeli, które spełniają określony warunek (np. σ).
 - Projekcja (Projection): Wybieranie tylko niektórych kolumn z tabeli (np. π).
 - Słączenie (Join): Łączenie dwóch tabel na podstawie wspólnego atrybutu (np. ⨝).
 - Unia (Union): Łączenie danych z dwóch tabel, eliminując duplikaty (np. ∪).
 - Różnica (Difference): Zwracanie różnicy między dwiema tabelami (np. -).
 - Iloczyn kartezjański (Cartesian Product): Łączenie wszystkich możliwych par wierszy z dwóch tabel (np. ×).
Przykład: Załóżmy, że mamy dwie tabele – Pracownicy i Działy. Możemy użyć operacji z algebry relacyjnej, aby połączyć je na podstawie wspólnego atrybutu, np. ID Działu, co daje nam jedną tabelę z pełnymi informacjami.

__DB Basics__ (Podstawy baz danych)
Podstawy baz danych (DB Basics) obejmują fundamentalne pojęcia i zasady, które pozwalają zrozumieć, jak działają bazy danych i jak są one używane do przechowywania, organizowania i przetwarzania danych. Kluczowe pojęcia to:
 - Tabela: Podstawowa jednostka przechowywania danych w relacyjnej bazie danych, składająca się z wierszy i kolumn.
 - Wiersz (Tuple): Pojedynczy rekord w tabeli. Wiersze zawierają konkretne dane.
 - Kolumna (Attribute): Kategoria danych w tabeli, np. "Imię", "Nazwisko", "Data urodzenia".
 - Klucz główny (Primary Key): Unikalny identyfikator dla każdego wiersza w tabeli, np. "ID pracownika".
 - Klucz obcy (Foreign Key): Atrybut w jednej tabeli, który wskazuje na klucz główny w innej tabeli, służy do tworzenia powiązań między tabelami.
 - Relacja: Struktura tabeli w bazie danych, która wiąże ze sobą różne dane.

SQL (Structured Query Language): Język zapytań używany do zarządzania bazami danych. SQL jest używany do definiowania, manipulowania i pobierania danych z baz danych.
Kluczowe operacje w bazach danych:
 - Dodawanie danych (INSERT): Wstawianie nowych wierszy do tabeli.
 - Usuwanie danych (DELETE): Usuwanie wierszy z tabeli.
 - Aktualizowanie danych (UPDATE): Zmiana wartości w tabeli.
 - Wybieranie danych (SELECT): Pobieranie danych z tabeli.
Bazy danych mogą być używane w różnych typach aplikacji, od prostych aplikacji webowych po duże systemy zarządzania informacjami w organizacjach. W zależności od zastosowania bazy danych mogą być zarządzane za pomocą różnych systemów, np. MySQL, PostgreSQL, Oracle, SQL Server.

## 4. Inner, Outer, Cross, Theta Join

__Inner Join__ zwraca tylko te wiersze, które mają dopasowanie w obu tabelach. Oznacza to, że tylko wiersze, które spełniają warunek łączenia (np. na podstawie wspólnego klucza), będą pojawiały się w wynikowej tabeli.

__Outer Join__ zwraca wszystkie wiersze z jednej tabeli oraz dopasowane wiersze z drugiej tabeli. Jeśli w drugiej tabeli nie ma dopasowania, wiersze z pierwszej tabeli pojawią się w wynikach, ale z wartościami NULL w kolumnach drugiej tabeli.
 - Left Outer Join (LEFT JOIN): Zwraca wszystkie wiersze z lewej tabeli i dopasowane wiersze z prawej tabeli. Jeśli nie ma dopasowania w prawej tabeli, pojawią się wartości NULL.
 - Right Outer Join (RIGHT JOIN): Zwraca wszystkie wiersze z prawej tabeli i dopasowane wiersze z lewej tabeli. Jeśli nie ma dopasowania w lewej tabeli, pojawią się wartości NULL.
 - Full Outer Join (FULL JOIN): Zwraca wszystkie wiersze z obu tabel, w tym te, które nie mają dopasowania. W przypadku braku dopasowania w jednej z tabel, w kolumnach tej tabeli pojawią się wartości NULL.

__Cross Join__ (znane także jako iloczyn kartezjański) zwraca wszystkie możliwe pary wierszy z dwóch tabel. Jest to operacja, która łączy każdy wiersz z jednej tabeli z każdym wierszem z drugiej tabeli, tworząc wynik, który zawiera wszystkie możliwe kombinacje.

__Theta Join__ to ogólny typ łączenia, w którym warunek łączenia jest określony za pomocą dowolnego operatora porównania, np. =, >, <, <=, >=, <>. Jest to bardziej ogólny przypadek joinów, który pozwala na zastosowanie bardziej złożonych warunków niż tylko równość.

## 5. CAP Theorem

Twierdzenie CAP mówi, że w systemach rozproszonych można zagwarantować maksymalnie dwa z trzech:

 - C (Consistency) – spójność danych,
 - A (Availability) – dostępność systemu,
 - P (Partition Tolerance) – tolerancja na podział sieci.
Nie da się osiągnąć wszystkich trzech jednocześnie.

## 6. Tabular Data

Tabular data (dane tabelaryczne) to dane, które są zorganizowane w formie tabeli, składającej się z wierszy i kolumn. Tego typu dane są powszechnie używane w bazach danych, arkuszach kalkulacyjnych (np. Excel), plikach CSV, a także w analizach danych i uczeniu maszynowym. Struktura tabeli pozwala na łatwe przechowywanie, organizowanie, analizowanie oraz manipulowanie danymi.

Kluczowe cechy danych tabelarycznych:
 - Wiersze (Rows): Każdy wiersz w tabeli reprezentuje pojedynczy rekord (np. dane dotyczące jednego klienta, zamówienia, pracownika itp.).
 - Kolumny (Columns): Kolumny reprezentują różne atrybuty lub cechy danych. Na przykład w tabeli dotyczącej pracowników kolumny mogą zawierać takie atrybuty jak ID, Imię, Nazwisko, Wiek, Dział, itp.
 - Komórki (Cells): Każda komórka w tabeli zawiera wartość, która jest wynikiem przecięcia wiersza i kolumny. Na przykład komórka może zawierać imię pracownika, jego wiek, datę zamówienia itp.

Zastosowania danych tabelarycznych:
 - Bazy danych: Relacyjne bazy danych przechowują dane tabelaryczne w tabelach. Tabele te są połączone ze sobą za pomocą kluczy, co pozwala na złożone zapytania i analizy.
 - Analiza danych: Dane tabelaryczne są popularne w analizie danych, szczególnie w narzędziach takich jak Python (pandas), R, Excel, czy SQL.
 - Uczenie maszynowe: W uczeniu maszynowym dane tabelaryczne są jedną z najczęściej stosowanych form danych wejściowych, szczególnie w zadaniach klasyfikacji, regresji i analizy danych.

Zalety danych tabelarycznych:
 - Strukturalność: Dzięki uporządkowanej strukturze (wiersze i kolumny) dane są łatwe do zrozumienia i przetwarzania.
 - Prostota: Tabele są łatwe w edycji, przechowywaniu i udostępnianiu.
 - Integracja: Tabele mogą być łatwo eksportowane i importowane do różnych narzędzi i systemów (np. CSV, Excel, bazy danych SQL).

## 7. Entropy

W kontekście analizy danych entropia (często nazywana entropią informacji) jest miarą niepewności, niejednoznaczności lub "chaosu" w zbiorze danych. Mówiąc prościej, entropia mierzy, jak bardzo rozproszone są dane w zbiorze — im wyższa entropia, tym mniej przewidywalne i bardziej zróżnicowane są dane. Jest to pojęcie szeroko stosowane w różnych technikach analizy danych, w tym w uczeniu maszynowym, drzewach decyzyjnych, algorytmach klasyfikacyjnych i kompresji danych.

__Entropia w kontekście analizy danych__
W analizie danych entropia jest wykorzystywana do mierzenia niepewności, jaką niosą dane w odniesieniu do ich klasyfikacji, segmentacji lub grupowania. Jeśli mamy zbiór danych, który jest w dużej mierze jednorodny (np. w większości przypadków ten sam typ danych, np. "tak" lub "nie"), entropia będzie niska. Natomiast w zbiorze, który zawiera różnorodne dane (np. wiele różnych klas lub wyników), entropia będzie wysoka.

__Entropia w kontekście drzew decyzyjnych__
Jednym z najczęstszych zastosowań entropii w analizie danych jest jej wykorzystanie w drzewach decyzyjnych (np. w algorytmie ID3, C4.5, CART). W tym przypadku entropia służy do wyboru najlepszego atrybutu, który najlepiej dzieli dane na mniejsze grupy, zmniejszając niepewność (lub entropię) w każdej z tych grup.

Wysoka entropia oznacza, że dane są bardzo zróżnicowane i nie można ich łatwo podzielić na jednorodne grupy.
Niska entropia oznacza, że dane są jednorodne i łatwo je podzielić.
Algorytm ID3, na przykład, stara się minimalizować entropię (redukcję niepewności) podczas tworzenia drzewa decyzyjnego. Działa to w sposób następujący:

Oblicza entropię całego zbioru danych, na przykład pod względem klas (np. "tak" lub "nie").
Następnie analizuje różne atrybuty (np. wiek, płeć, dochód) i sprawdza, jak podział na te atrybuty wpływa na zmniejszenie entropii w wyniku podziału danych.
Atrybut, który najbardziej zmniejsza entropię (czyli najlepiej "segreguje" dane), zostaje wybrany jako węzeł w drzewie decyzyjnym.

__Zastosowania entropii w analizie danych__:
 - Drzewa decyzyjne: Jak wspomniano, entropia jest wykorzystywana do podziału danych w algorytmach drzewa decyzyjnego (np. ID3, C4.5).
 - Klastry: W algorytmach grupujących, takich jak k-means, entropia może być używana do oceny, jak dobrze dane są podzielone na grupy.
 - Wybór cech: Entropia może być wykorzystywana do oceny znaczenia poszczególnych cech w zbiorze danych, pomagając w wyborze najistotniejszych cech do analizy.


## 8. Data Frames & Series

 - Data Frame – dwuwymiarowa struktura danych (podobna do tabeli), np. w Pandas (Python).
 - Series – jednowymiarowa struktura (kolumna tabeli).

## 9. Sharding

Sharding to technika używana w bazach danych i systemach rozproszonych, polegająca na podzieleniu danych na mniejsze, łatwiejsze do zarządzania części, zwane "shardami". Każdy shard to fragment danych, który może być przechowywany na osobnym serwerze lub w odrębnym węźle w systemie rozproszonym. Celem shardingu jest zwiększenie wydajności, skalowalności oraz dostępności systemu.

W praktyce, sharding pozwala rozdzielić obciążenie między wiele serwerów, co ułatwia obsługę dużych zbiorów danych i umożliwia równoczesne przetwarzanie wielu zapytań w różnych miejscach. Shardowanie jest powszechnie wykorzystywane w bazach danych NoSQL, takich jak MongoDB, oraz w niektórych tradycyjnych bazach danych SQL.

Główne korzyści z sharding:
 - Skalowalność: Dzięki podzieleniu danych na mniejsze fragmenty, system może rosnąć, dodając kolejne serwery lub węzły.
 - Wydajność: Równoległe przetwarzanie zapytań na różnych shardach zwiększa szybkość operacji.
 - Dostępność: W przypadku awarii jednego z shardów, dane mogą być nadal dostępne na innych węzłach.

Wyzwania związane z shardingiem to m.in. utrzymanie integralności danych między shardami, złożoność zapytań, które mogą wymagać dostępu do wielu shardów jednocześnie, oraz zarządzanie równomiernym rozkładem danych między shardami.

## 10. OLAP

Technologia baz danych umożliwiająca analizę wielowymiarowych zbiorów danych w celu generowania raportów i analiz biznesowych.

## 11. Multidimensional Data Model

Modelowanie danych w postaci wymiarów i miar – wykorzystywane w hurtowniach danych i systemach OLAP.

## 12. ETL

Proces pobierania, przekształcania i ładowania danych do systemów analitycznych lub hurtowni danych.

## 13. Reporting Vs BI Vs Analytics

 - Reporting – Generowanie statycznych raportów na podstawie danych.
 - BI (Business Intelligence) – Interaktywna analiza danych do wspomagania decyzji biznesowych.
 - Analytics – Zaawansowana analiza predykcyjna i eksploracyjna danych (np. ML).

## 14. JSON & XML

 - JSON – Lekki format wymiany danych, czytelny dla ludzi i łatwy do przetwarzania przez maszyny (używany np. w API).
 - XML – Strukturalny format wymiany danych, często wykorzystywany w starszych systemach

## 15. NoSQL

Rodzina baz danych nie-relacyjnych, zaprojektowanych do obsługi dużych zbiorów danych i wysokiej wydajności (np. MongoDB, Cassandra, Redis).

## 16. Regex

Wzorce służące do wyszukiwania i manipulacji tekstu (np. znajdowanie e-maili, numerów telefonów w tekście).

## 17. Vendor Landscape

Analiza dostawców technologii lub produktów w danej branży, np. analiza firm dostarczających rozwiązania chmurowe (AWS, Azure, GCP).

## 18. Env Setup

Proces konfiguracji środowiska pracy, np. instalacja Python, Jupyter Notebook, VS Code, Docker, bazy danych itp.
