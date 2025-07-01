# Datensammlungen

## Liste & Tupel

In Python gibt es verschiedene Möglichkeiten, **mehrere Werte in einer einzigen Variablen zu speichern**. Zwei der wichtigsten Datensammlungen sind:

* `list` (Liste): veränderbar
* `tuple` (Tupel): unveränderlich

***

### <mark style="color:blue;">1. Liste –</mark> <mark style="color:blue;"></mark><mark style="color:blue;">`list`</mark>

Eine **Liste** ist eine geordnete Sammlung von Werten, die veränderbar ist. Man erkennt sie an den **eckigen Klammern** `[]`.

```python
früchte = ["Apfel", "Banane", "Kirsche"]
```

Eigenschaften:

* Elemente sind **geordnet**
* **veränderbar** (man kann Werte hinzufügen, löschen, ändern)
* Kann verschiedene Datentypen enthalten



Beispiel:

```python
pythonKopierenBearbeitenfrüchte.append("Orange")  # Fügt Orange hinzu
früchte[0] = "Birne"       # Ändert Apfel zu Birne
```







### <mark style="color:blue;">2. Tupel –</mark> <mark style="color:blue;"></mark><mark style="color:blue;">`tuple`</mark>

Ein **Tupel** ist ähnlich wie eine Liste, aber **unveränderlich**. Es wird mit **runden Klammern** `()` geschrieben.

```python
pythonKopierenBearbeitenfarben = ("rot", "grün", "blau")
```

Eigenschaften:

* Elemente sind **geordnet**
* **nicht veränderbar** (man kann keine Werte ändern oder hinzufügen)
* Nützlich für feste Daten, die sich nicht ändern sollen



Beispiel – nicht erlaubt:

```python
pythonKopierenBearbeitenfarben[0] = "gelb"  # ❌ Fehler! Tupel kann nicht verändert werden
```



### <mark style="color:blue;">Unterschiede zwischen Liste und Tupel</mark>

| Eigenschaft   | Liste (`list`)         | Tupel (`tuple`)         |
| ------------- | ---------------------- | ----------------------- |
| Klammern      | `[]`                   | `()`                    |
| Veränderbar   | ✅ Ja                   | ❌ Nein                  |
| Einsatzgebiet | Wenn Werte sich ändern | Wenn Werte fest bleiben |
