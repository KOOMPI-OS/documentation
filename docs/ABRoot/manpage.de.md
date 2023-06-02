---
Titel: Manpage ABRoot - KOOMPI OS
Beschreibung: Manpage für das ABRoot-Programm.
---

# Manpage `abroot`

## NAME

```text
ABRoot ist ein Programm, das komplette Unveränderlichkeit und Atomarität bietet, indem es Transaktionen zwischen 2 Root-Partitionen (A⟺B) ausführt. Es ermöglicht auch sofortige Transaktionen mithilfe einer interaktiven Shell.
```

## ÜBERSICHT

```text
abroot [Optionen] [Befehl]
```

## BESCHREIBUNG

```markdown
Verwendung:
    abroot [Optionen] [Befehl]

Optionen:
    --help/-h           Diese Hilfe ausgeben
    --verbose/-v        Ausführlichere Informationen ausgeben
    --version/-V        Version anzeigen

Befehle:
    _update-boot        Boot-Partition aktualisieren (nur für fortgeschrittene Nutzer)
    get                 Gibt den derzeitigen oder zukünftigen Zustand der Root-Partition aus
    shell               Interaktive Shell in der zukünftigen Root-Partition öffnen und beim nächsten Neustart die Root-Partition wechseln
    exec                Befehl in einer interaktiven Shell in der zukünftigen Root-Partition ausführen und beim nächsten Neustart die Root-Partition wechseln
```

## EXEC

```markdown
Befehl in einer interaktiven Shell in der zukünftigen Root-Partition ausführen und beim nächsten Neustart die Root-Partition wechseln.

Verwendung:
    exec [Befehl]

Optionen:
    --help/-h           Diese Hilfe ausgeben
    --assume-yes/-y     Ohne manuelle Bestätigung fortfahren

Beispiele:
    abroot exec ls -l /
    abroot exec apt install git 
```

```text
Tipp: Sie können mehrere Befehle mit "" einklammern und als einzelnen String eingeben.
```

### GET

```markdown
Gibt den derzeitigen oder zukünftigen Zustand der Root-Partition aus (A oder B).

Verwendung:
    get [Stadium]

Optionen:
    --help/-h       Diese Hilfe ausgeben

Stadien:
    present         Den derzeitigen Stand ausgeben
    future          Den zukünftigen Stand ausgeben

Beispiele:
    abroot get present
    abroot get future
```

## SHELL

```markdown
Interaktive Shell in der zukünftigen Root-Partition öffnen und beim nächsten Neustart die Root-Partition wechseln.

Verwendung:
    shell

Optionen:
    --help/-h           Diese Hilfe ausgeben
    --assume-yes/-y     Ohne manuelle Bestätigung fortfahren

Beispiele:
    abroot shell
```

## UPDATE BOOT

```markdown
Boot-Partition zu Wartungszwecken aktualisieren (nur für fortgeschrittene Nutzer).

Verwendung:
    _update-boot

Optionen:
    --help/-h           Diese Hilfe ausgeben
    --assume-yes/-y     Ohne manuelle Bestätigung fortfahren
```

## SIEHE AUCH

- [`pix`](/docs/pix)
- [`kso`](/docs/kso)

## AUTHOR

```text
Mitwirkende von KOOMPI OS
```

## FEHLER MELDEN

Fehler bitte beim [Bugtracker](https://github.com/koompi-os/ABRoot/issues) melden.
