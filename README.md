# Sortowanie uczniów

## Opis projektu

Program został napisany w języku **C++**.

Jego zadaniem jest:

1. Wczytanie danych uczniów z pliku tekstowego.
2. Zapisanie danych do tablicy rekordów.
3. Posortowanie uczniów rosnąco według nazwiska.
4. Zapisanie posortowanych danych do pliku wynikowego.

Program obsługuje maksymalnie **30 uczniów**.

## Struktura rekordu

Każda osoba jest przechowywana w rekordzie:

```cpp
struct Person
{
    string firstName;
    string lastName;
    int number;
};
```

Rekord zawiera:

* `firstName` – imię ucznia,
* `lastName` – nazwisko ucznia,
* `number` – numer ucznia.

## Plik wejściowy

Program pobiera dane z pliku:

```text
Nowy Dokument tekstowy.txt
```

Każdy uczeń znajduje się w osobnej linii.

Format danych:

```text
imię nazwisko numer
```

Przykład:

```text
Jan Kowalski 1
Anna Nowak 2
Piotr Wiśniewski 3
Katarzyna Wójcik 4
Tomasz Kamiński 5
```

## Plik wynikowy

Po posortowaniu dane są zapisywane do:

```text
wynik.txt
```

Każda osoba również znajduje się w osobnej linii.

## Funkcje programu

### `readPeople()`

Odpowiada za wczytanie danych z pliku do tablicy rekordów.

### `sortPeople()`

Sortuje uczniów rosnąco według nazwiska.

### `savePeople()`

Zapisuje posortowane dane do pliku wynikowego.

### `convertPolishLetters()`

Pomaga w prawidłowym porównywaniu nazwisk zawierających polskie znaki.

## Wykorzystane elementy C++

W projekcie wykorzystano:

* `struct`,
* tablicę rekordów,
* funkcje,
* `ifstream`,
* `ofstream`,
* `std::sort`,
* wyrażenie lambda,
* pętlę `for`,
* instrukcję `switch`,
* programowanie zstępujące.

## Uruchomienie

Program można uruchomić w środowisku obsługującym język C++, np. Visual Studio lub Code::Blocks.

Po uruchomieniu program:

```text
1. Wczytuje dane.
2. Sortuje nazwiska.
3. Zapisuje wynik.
```

Po poprawnym wykonaniu programu pojawi się komunikat:

```text
Dane zostaly posortowane i zapisane.
```

## Autor

Projekt wykonany na potrzeby zadania z programowania w języku C++.
