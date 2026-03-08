---
title: Markdown — przykładowy plik do nauki
---

Ten plik pokazuje **najważniejsze elementy Markdown** na praktycznych przykładach.

[Linia pozioma] (#linia_pozioma)

---

## 1. Nagłówki

# Nagłówek poziomu 1
## Nagłówek poziomu 2
### Nagłówek poziomu 3
#### Nagłówek poziomu 4
##### Nagłówek poziomu 5
###### Nagłówek poziomu 6

**Składnia:**

```md
# Nagłówek 1
## Nagłówek 2
### Nagłówek 3
```

---

## 2. Akapity i łamanie linii

To jest zwykły akapit tekstu. Markdown sam składa tekst w akapity.

To jest nowy akapit, bo między nimi jest pusta linia.

To jest linia zakończona dwoma spacjami na końcu.  
Dzięki temu tekst przeszedł do nowej linii.

**Składnia:**

```md
Pierwszy akapit.

Drugi akapit.

Pierwsza linia.  
Druga linia.
```

---

## 3. Wyróżnienia tekstu

To jest tekst *kursywą*.

To jest tekst **pogrubiony**.

To jest tekst ***pogrubiony i kursywą***.

To jest ~~tekst przekreślony~~.

Można też używać `kodu w linii`.

**Składnia:**

```md
*kursywa*
**pogrubienie**
***pogrubienie i kursywa***
~~przekreślenie~~
`kod w linii`
```

---

## 4. Listy

### Lista nienumerowana

- element 1
- element 2
  - podpunkt 2a
  - podpunkt 2b
- element 3

### Lista numerowana

1. pierwszy krok
2. drugi krok
3. trzeci krok

### Lista zadań

- [x] utworzyć plik `.md`
- [x] dodać nagłówki
- [ ] poćwiczyć samodzielnie

**Składnia:**

```md
- element
- element
  - podpunkt

1. pierwszy
2. drugi

- [x] zrobione
- [ ] do zrobienia
```

---

## 5. Cytaty

> To jest prosty cytat.
>
> Może mieć kilka akapitów.

> ### Cytat może też zawierać inne elementy
> - listę
> - **pogrubienie**
> - `kod`

**Składnia:**

```md
> To jest cytat.
>
> Drugi akapit cytatu.
```

---

## 6. Linki

Link do [GitHub](https://github.com).

Link z pełnym adresem: <https://www.markdownguide.org>

**Składnia:**

```md
[GitHub](https://github.com)
<https://www.markdownguide.org>
```

---

## 7. Obrazy

![Przykładowy obraz](https://via.placeholder.com/600x120?text=Przykladowy+obraz+Markdown)

**Składnia:**

```md
![Opis obrazu](https://adres.pl/obraz.png)
```

---

## 8. Kod

### Kod w linii

Użyj polecenia `git status`, aby sprawdzić stan repozytorium.

### Blok kodu bez podświetlania składni

```
To jest zwykły blok kodu.
Może mieć kilka linii.
```

### Blok kodu z podświetlaniem składni

```python
name = "Markdown"
for i in range(3):
    print(f"{i+1}. Uczę się {name}")
```

```bash
git add .
git commit -m "Dodano plik markdown"
git push
```

**Składnia:**

````md
```python
print("Hello")
```
````

---

## 9. Linia pozioma 
{: #linia_pozioma}
Poniżej jest linia pozioma:

---

**Składnia:**

```md
---
```

---

## 10. Tabele

| Kolumna 1 | Kolumna 2 | Kolumna 3 |
|-----------|-----------|-----------|
| A         | B         | C         |
| 1         | 2         | 3         |
| lewo      | środek    | prawo     |

Tabela z wyrównaniem:

| Nazwa      | Typ        | Status |
|:-----------|:----------:|-------:|
| README.md  | plik       | gotowe |
| docs/      | katalog    | w toku |
| index.html | plik       | brak   |

**Składnia:**

```md
| Nazwa | Typ | Status |
|:------|:---:|-------:|
| A     | B   | C      |
```

---

## 11. Bloki informacyjne jako zwykły trik tekstowy

> **Uwaga:** Markdown sam w sobie nie ma „kolorowych ramek” jak Word.
> Na GitHubie często używa się po prostu cytatów, emoji albo HTML.

> ✅ **Wskazówka:** Pisz krótko i czytelnie.

> ⚠️ **Ostrzeżenie:** Nie każda platforma obsługuje wszystkie rozszerzenia Markdown.

---

## 12. HTML w Markdown

Czasami można wstawić prosty HTML:

<p><b>Ten tekst jest pogrubiony przez HTML.</b></p>
<p style="color: gray;">Nie wszędzie style CSS będą działały.</p>

<details>
  <summary>Kliknij, aby rozwinąć</summary>

  To jest treść ukryta w znaczniku `details`.
</details>

**Składnia:**

```md
<details>
  <summary>Kliknij</summary>
  Ukryta treść.
</details>
```

---

## 13. Przypisy

Markdown w niektórych wersjach obsługuje przypisy.[^1]

[^1]: To jest przykładowy przypis.

**Składnia:**

```md
Tekst z przypisem.[^1]

[^1]: Treść przypisu.
```

---

## 14. Checklista najczęściej używanych rzeczy

Najczęściej w praktyce używa się tylko kilku elementów:

- nagłówków
- pogrubienia i kursywy
- list
- linków
- obrazów
- bloków kodu
- tabel

To już wystarcza do:

- README na GitHubie
- notatek
- dokumentacji projektu
- prostych instrukcji
- treści do GitHub Pages

---

## 15. Mini przykład gotowego dokumentu

# Mój projekt

Krótki opis projektu w 2–3 zdaniach.

## Funkcje

- szybkie działanie
- prosty interfejs
- eksport wyników

## Instalacja

```bash
git clone https://github.com/uzytkownik/projekt.git
cd projekt
python app.py
```

## Zrzut ekranu

![Zrzut ekranu](https://via.placeholder.com/700x200?text=Screenshot)

## Autor

Jan Kowalski

---

## 16. Dobre praktyki

1. Używaj krótkich nagłówków.
2. Nie przesadzaj z pogrubieniem.
3. Zostawiaj puste linie między sekcjami.
4. W kodzie zawsze dodawaj język po trzech backtickach, jeśli to możliwe.
5. Sprawdzaj, jak plik wygląda po wyrenderowaniu.

---

## 17. Ściąga składni

```md
# Nagłówek 1
## Nagłówek 2

**pogrubienie**
*kursywa*
~~przekreślenie~~
`kod`

- lista
1. lista numerowana
- [ ] zadanie
- [x] zadanie zrobione

[tekst linku](https://example.com)
![opis obrazu](obraz.png)

> cytat

```python
print("kod")
```

| kol1 | kol2 |
|------|------|
| A    | B    |
```

---

Powodzenia w nauce Markdown.
