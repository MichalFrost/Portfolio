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

__Relational Algebra__ – Matematyczny formalizm do manipulacji danymi w relacyjnych bazach danych (SQL opiera się na jej zasadach).
__DB Basics__ – Podstawy baz danych, w tym tabele, klucze, indeksy, normalizacja i zapytania SQL.

## 4. Inner, Outer, Cross, Theta Join

 - Inner Join – Zwraca tylko pasujące rekordy między dwiema tabelami.
 - Outer Join – Może być LEFT, RIGHT, FULL – zwraca pasujące rekordy oraz te, które nie mają odpowiednika.
 - Cross Join – Tworzy iloczyn kartezjański dwóch tabel (łączy każdy wiersz pierwszej tabeli z każdym wierszem drugiej).
 - Theta Join – Warunkowe łączenie tabel na podstawie dowolnego warunku (niekoniecznie klucza).

## 5. CAP Theorem

Twierdzenie CAP mówi, że w systemach rozproszonych można zagwarantować maksymalnie dwa z trzech:

 - C (Consistency) – spójność danych,
 - A (Availability) – dostępność systemu,
 - P (Partition Tolerance) – tolerancja na podział sieci.
Nie da się osiągnąć wszystkich trzech jednocześnie.

## 6. Tabular Data

Dane tabelaryczne – zorganizowane w wiersze i kolumny (np. pliki CSV, SQL, arkusze kalkulacyjne).

## 7. Entropy

W teorii informacji – miara niepewności w zbiorze danych (np. w drzewach decyzyjnych).
W statystyce – określa niejednorodność danych w podziale klasyfikacyjnym.

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
