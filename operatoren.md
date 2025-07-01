#  Operatoren in Python

Beim Programmieren mit Python braucht man **Operatoren**, um Werte zu vergleichen, Rechenoperationen durchzuführen oder Bedingungen zu verknüpfen. In diesem Kapitel geht es um die **logischen Operatoren** – ein zentrales Thema, wenn du mit Bedingungen (`if`, `while`, `and`, `or`, `not`) arbeitest.

---

##  Was sind logische Operatoren?

**Logische Operatoren** werden verwendet, um **Wahrheitswerte (True/False)** miteinander zu verknüpfen. Das Ergebnis ist immer entweder `True` oder `False`.

Python kennt drei logische Operatoren:

| Operator | Bedeutung          | Beschreibung                                  |
|----------|--------------------|-----------------------------------------------|
| `and`    | Und                | Nur `True`, wenn **beide** Bedingungen wahr sind |
| `or`     | Oder               | `True`, wenn **mindestens eine** Bedingung wahr ist |
| `not`    | Nicht              | Kehrt den Wahrheitswert um (`not True` → `False`) |

---

## Beispiele

### `and` – Beide Bedingungen müssen zutreffen

```python
x = 5
print(x > 3 and x < 10)  # True, weil beides stimmt
print(x > 3 and x > 10)  # False, weil x nicht > 10 ist
````
## Arithmetische Operatoren

| Operator | Beschreibung            | Beispiel           | Ergebnis |
|----------|-------------------------|--------------------|----------|
| `+`      | Addition                 | `3 + 2`            | `5`      |
| `-`      | Subtraktion              | `5 - 3`            | `2`      |
| `*`      | Multiplikation           | `4 * 2`            | `8`      |
| `/`      | Division (Kommazahl)     | `10 / 4`           | `2.5`    |
| `//`     | Ganzzahlige Division     | `10 // 4`          | `2`      |
| `%`      | Modulo (Rest)            | `10 % 4`           | `2`      |
| `**`     | Potenzierung             | `2 ** 3`           | `8`      |

**Hinweis:** Die Division `/` liefert immer ein **float** (Kommazahl), auch wenn das Ergebnis eine ganze Zahl ist.

---

## Vergleichsoperatoren

Diese Operatoren geben `True` oder `False` zurück – also einen **Wahrheitswert**.

| Operator | Beschreibung             | Beispiel         | Ergebnis |
|----------|--------------------------|------------------|----------|
| `==`     | Gleich                   | `5 == 5`         | `True`   |
| `!=`     | Ungleich                 | `5 != 3`         | `True`   |
| `<`      | Kleiner als              | `3 < 4`          | `True`   |
| `<=`     | Kleiner oder gleich      | `3 <= 3`         | `True`   |
| `>`      | Größer als               | `5 > 2`          | `True`   |
| `>=`     | Größer oder gleich       | `4 >= 4`         | `True`   |

---
## or – Eine Bedingung reicht aus
````
x = 5
print(x > 3 or x > 10)   # True, weil x > 3
print(x < 3 or x > 10)   # False, weil beides falsch ist
````

## not – Umkehr des Wahrheitswertes
````
x = 5
print(not x > 3)         # False, weil x > 3 → True → wird umgekehrt
````

## Praktisches Beispiel
````
benutzername = "alina"
passwort = "geheim123"

if benutzername == "alina" and passwort == "geheim123":
    print("Zugriff erlaubt")
else:
    print("Zugriff verweigert")
