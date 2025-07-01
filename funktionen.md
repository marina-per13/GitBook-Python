# Funktionen

## Funktionen in Python

Funktionen sind ein zentraler Bestandteil von Python. Sie helfen dabei, **Code wiederverwendbar**, **übersichtlich** und **strukturiert** zu schreiben.

Mit einer Funktion kann man eine bestimmte Aufgabe **einmal definieren** und dann **mehrfach verwenden**.

***

### <mark style="color:blue;">Was ist eine Funktion?</mark>

Eine Funktion ist ein benannter Codeblock, der **ausgeführt wird**, wenn er **aufgerufen** wird.

```python
def begrüße():
    print("Hallo und willkommen!")
```



Hier wird die Funktion `begrüße` definiert. Sie führt einfach einen `print`-Befehl aus.

Aufrufen der Funktion:

```python
pythonKopierenBearbeitenbegrüße()
```



### <mark style="color:blue;">Funktionen mit Parametern</mark>

Funktionen können **Parameter** enthalten. Ein Parameter ist eine **Variable**, die beim Funktionsaufruf **einen Wert bekommt**.

```python
pythonKopierenBearbeitendef begrüße(name):
    print("Hallo, " + name + "!")
```

Verwendung:

```python
pythonKopierenBearbeitenbegrüße("Anna")
begrüße("Tom")
```

→ Der Parameter `name` bekommt den Wert `"Anna"` bzw. `"Tom"` beim Aufruf.

Man kann auch mehrere Parameter verwenden:

```python
pythonKopierenBearbeitendef addiere(a, b):
    print(a + b)
```

```python
pythonKopierenBearbeitenaddiere(3, 5)  # Ausgabe: 8
```

***

### <mark style="color:blue;">Rückgabewerte mit</mark> <mark style="color:blue;"></mark><mark style="color:blue;">`return`</mark>

Manchmal möchte man, dass eine Funktion einen Wert **zurückgibt**, den man weiterverwenden kann. Dafür nutzt man das Schlüsselwort `return`.

```python
pythonKopierenBearbeitendef addiere(a, b):
    return a + b
```

Verwendung:

```python
pythonKopierenBearbeitenergebnis = addiere(10, 7)
print(ergebnis)  # Ausgabe: 17
```

💡 Der Unterschied zu `print`:

* `print` zeigt etwas auf dem Bildschirm an
* `return` gibt den Wert zurück, mit dem man weiterrechnen oder arbeiten kann

***

### <mark style="color:blue;">Zusammenfassung</mark>

| Begriff   | Bedeutung                                                          |
| --------- | ------------------------------------------------------------------ |
| Funktion  | Ein benannter Block von Code                                       |
| Parameter | Platzhalter für Werte, die an die Funktion übergeben werden        |
| `return`  | Gibt einen Wert aus der Funktion zurück                            |
| Aufruf    | Der Moment, in dem die Funktion ausgeführt wird (`funktionname()`) |

### <mark style="color:blue;">Beispiel: Eine Funktion mit allem kombiniert</mark>

```python
pythonKopierenBearbeitendef begrüsse_person(name, alter):
    return "Hallo " + name + ", du bist " + str(alter) + " Jahre alt."
```

```python
pythonKopierenBearbeitentext = begrüsse_person("Maya", 22)
print(text)
# Ausgabe: Hallo Maya, du bist 22 Jahre alt.
```

