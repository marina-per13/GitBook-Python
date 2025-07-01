---
icon: gamepad-modern
coverY: 0
---

# Abschlussprojekt

## Zufallsspiel mit Zahlen

***

### Schritt 1: Module importieren

Wir brauchen das Modul `random` für Zufallszahlen und `time`, um Pausen einzubauen.

<details> <summary>Code anzeigen</summary>
python
Kopieren
Bearbeiten
import random
import time
</details> ````
Schritt 2: Spielbegrüßung und Regeln anzeigen
Begrüße den Spieler und erkläre kurz die Spielregeln.

bash
Kopieren
Bearbeiten
<details>
  <summary>Code anzeigen</summary>

```python
print("Willkommen zum Zufallsspiel!")
print("Du hast 5 Versuche, eine Zahl zwischen 1 und 10 zu erraten.")
print("Für jeden richtigen Tipp bekommst du einen Punkt.")
print("Viel Erfolg!")
time.sleep(2)  # Kurze Pause von 2 Sekunden
```

</details>
Schritt 3: Punkte und Versuche initialisieren
Setze die Punkte und maximale Versuche auf 0 bzw. 5.

javascript
Kopieren
Bearbeiten
<details>
  <summary>Code anzeigen</summary>

```python
punkte = 0
max_versuche = 5
```

</details>
Schritt 4: Schleife für Versuche starten
Erstelle eine Schleife, die für jeden Versuch einmal durchläuft.

css
Kopieren
Bearbeiten
<details>
  <summary>Code anzeigen</summary>

```python
for versuch in range(1, max_versuche + 1):
    print(f"\nVersuch {versuch} von {max_versuche}")
```

</details>
Schritt 5: Zufallszahl erzeugen
Erzeuge für jeden Versuch eine neue Zufallszahl zwischen 1 und 10.

javascript
Kopieren
Bearbeiten
<details>
  <summary>Code anzeigen</summary>

```python
    zahl = random.randint(1, 10)
```

</details>
Schritt 6: Spieler nach Eingabe fragen und prüfen
Fordere den Spieler auf, eine Zahl einzugeben. Prüfe, ob die Eingabe gültig ist (Zahl zwischen 1 und 10).

css
Kopieren
Bearbeiten
<details>
  <summary>Code anzeigen</summary>

```python
    while True:
        try:
            tipp = int(input("Rate eine Zahl zwischen 1 und 10: "))
            if 1 <= tipp <= 10:
                break
            else:
                print("Bitte gib eine Zahl zwischen 1 und 10 ein.")
        except ValueError:
            print("Das war keine gültige Zahl. Versuch es nochmal.")
```

</details>
Schritt 7: Tipp mit Zufallszahl vergleichen
Wenn der Tipp richtig ist, Punkte erhöhen und Erfolg melden.

bash
Kopieren
Bearbeiten
<details>
  <summary>Code anzeigen</summary>

```python
    if tipp == zahl:
        print("Richtig! Du bekommst einen Punkt.")
        punkte += 1
    else:
        print(f"Falsch! Die richtige Zahl war {zahl}.")
```

</details>
Schritt 8: Kurze Pause einbauen
Damit das Spiel nicht zu schnell ist, füge eine kurze Pause von 1 Sekunde ein.

css
Kopieren
Bearbeiten
<details>
  <summary>Code anzeigen</summary>

```python
    time.sleep(1)
```

</details>
Schritt 9: Punkte nach jedem Versuch anzeigen
Zeige nach jedem Versuch den aktuellen Punktestand.

css
Kopieren
Bearbeiten
<details>
  <summary>Code anzeigen</summary>

```python
    print(f"Deine Punkte: {punkte}")
```

</details>
Schritt 10: Spiel beenden und Gesamtergebnis ausgeben
Nach der Schleife gebe das Endergebnis aus und verabschiede den Spieler.

bash
Kopieren
Bearbeiten
<details>
  <summary>Code anzeigen</summary>

```python
print("\nSpiel beendet!")
print(f"Du hast {punkte} von {max_versuche} Punkten erreicht. Gut gemacht!")
```

</details>
Komplett-Code (mit allen 10 Schritten)
swift
Kopieren
Bearbeiten
<details>
  <summary>Kompletten Code anzeigen</summary>

```python
import random
import time

print("Willkommen zum Zufallsspiel!")
print("Du hast 5 Versuche, eine Zahl zwischen 1 und 10 zu erraten.")
print("Für jeden richtigen Tipp bekommst du einen Punkt.")
print("Viel Erfolg!")

time.sleep(2)

punkte = 0
max_versuche = 5

for versuch in range(1, max_versuche + 1):
    print(f"\nVersuch {versuch} von {max_versuche}")
    zahl = random.randint(1, 10)

    while True:
        try:
            tipp = int(input("Rate eine Zahl zwischen 1 und 10: "))
            if 1 <= tipp <= 10:
                break
            else:
                print("Bitte gib eine Zahl zwischen 1 und 10 ein.")
        except ValueError:
            print("Das war keine gültige Zahl. Versuch es nochmal.")

    if tipp == zahl:
        print("Richtig! Du bekommst einen Punkt.")
        punkte += 1
    else:
        print(f"Falsch! Die richtige Zahl war {zahl}.")

    time.sleep(1)
    print(f"Deine Punkte: {punkte}")

print("\nSpiel beendet!")
print(f"Du hast {punkte} von {max_versuche} Punkten erreicht. Gut gemacht!")
```

</details>
