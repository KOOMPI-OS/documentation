---
Titel: Manpage pix - KOOMPI OS
Beschreibung: Manpage für das pix-Programm.
---

# Manpage `pix`

## NAME

```text
`pix` - Der nutzerfreundliche KOOMPI OS-Paketverwalter mit Unterstützung für die Installation von Paketen aus verschiedenen Quellen in Containern, um das Root-Dateisystem nicht zu verändern.
```

## ÜBERSICHT

```text
pix [Optionen] [Befehl] [Argumente]
```

## BESCHREIBUNG

```markdown
pix ist ein Wrapper um mehrere Paketvervaltungprogramme, der Installationen und andere Befehle in einem verwalteten Container durchführt.

Aufruf:
    pix [Optionen] [Befehl] [Argumente]

Optionen:
    -h, --help      Diese Hilfe ausgeben und beenden
    -v, --version   Versionsinformation anzeigen und beenden
    --aur           Pakete aus dem AUR installieren
    --dnf           Pakete aus dem Fedora-Repository installieren

Befehle:
    autoremove      Alle nicht genutzten Pakete entfernen
    clean           Cache des pix-Paketverwalters leeren
    enter           Container-Shell öffnen
    export          Menüeintrag eines Programms aus dem Container exportieren
    help            Diese Hilfe ausgeben und beenden
    init            Einen verwalteten Container initialisieren
    install         Paket innerhalb des Containers installieren
    list            Installierte Pakete auflisten
    log             Logdateien anzeigen
    purge           Pakete und Konfigurationsdateien vom Container entfernen
    run             Befehl innerhalb des Containers ausführen
    remove          Pakete vom Container entfernen
    search          Nach Paketen suchen
    show            Details über ein Paket anzeigen
    unexport        Menüeintrag eines Programms entfernen
    update          Liste der verfügbaren Pakete aktualisieren
    upgrade         Verfügbare Paketaktualisierungen anwenden
    version         Versionsinformation anzeigen und beenden
```

## AUTOREMOVE

```markdown
Beschreibung: 
    Alle nicht genutzten Pakete automatisch entfernen.

Aufruf:
    pix autoremove [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden

Beispiele:
    pix autoremove
```

## CLEAN

```markdown
Beschreibung: 
    Cache des pix-Paketverwalters leeren.

Aufruf:
    pix clean [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden

Beispiele:
    pix clean
```

## ENTER

```markdown
Beschreibung: 
    Die Shell des gegebenen Containers öffnen.

Aufruf:
    pix enter [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden
```

## EXPORT

```markdown
Beschreibung: 
    Den Menüeintrag eines Programms aus einem verwalteten Container exportieren/neuerstellen.

Aufruf:
    pix export <Programm> [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden

Beispiele:
    pix export htop
```

## INIT

```markdown
Beschreibung: 
    Einen verwalteten Container initialisieren.

Aufruf:
    pix init [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden
```

## INSTALL

```markdown
Beschreibung: 
    Pakete innerhalb eines verwalteten Containers installieren.

Aufruf:
    pix install [Optionen] <Pakete>

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden
    -y, --assume-yes      Ohne manuelle Bestätigung fortfahren
    -f, --fix-broken      Vor der Installation beschädigte Abhängigkeiten reparieren
    --no-export           Menüeintrag nach der Installation nicht exportieren
    --sideload [Pfad]     Paket von einer lokalen Datei installieren

Beispiele:
    pix install htop git
    pix install --sideload /Pfad/zur/Datei.deb
```

## LIST

```markdown
Beschreibung: 
    Installierte Pakete auflisten.

Aufruf:
    pix list [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden
```

## PURGE

```markdown
Beschreibung: 
    Pakete und Konfigurationsdateien in einem verwalteten Container entfernen.

Aufruf:
    pix purge <Pakete> [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden

Beispiele:
    pix purge htop
```

## REMOVE

```markdown
Beschreibung:
    Pakete in einem verwalteten Container entfernen.

Aufruf:
    pix remove <Pakete> [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden

Beispiele:
    pix remove htop
```

## RUN

```markdown
Beschreibung: 
    Programm in einem verwalteten Container ausführen.

Aufruf:
    pix run <Programm> [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden

Beispiele:
    pix run htop
```

## SEARCH

```markdown
Beschreibung: 
    In einem verwalteten Container nach Paketen suchen.

Aufruf:
    pix search <Pakete> [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden

Beispiele:
    pix search htop
```

## SHOW

```markdown
Beschreibung: 
    Details über ein Paket anzeigen.

Aufruf:
    pix show <package> [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden

Beispiele:
    pix show htop
```

## UNEXPORT

```markdown
Beschreibung:
    Menüeintrag eines Programms aus einem verwalteten Container entfernen.

Aufruf:
    pix unexport <Programm> [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden

Beispiele:
    pix unexport htop
```

## UPDATE

```markdown
Beschreibung: 
    Die Liste der verfügbaren Pakete aktualisieren.

Aufruf:
    pix update [Optionen]

Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden

Beispiele:
    pix update
```

## UPGRADE

```markdown
Beschreibung: 
    Verfügbare Paketaktualisierungen anwenden.

Aufruf:
    pix upgrade [Optionen]
  
Optionen:
    -h, --help            Diese Hilfe ausgeben und beenden

Beispiele:
    pix upgrade
```

## VERSION

```markdown
Beschreibung:
    Die pix-Version anzeigen.

Aufruf:
    pix --version
    pix -v
```

## SIEHE AUCH

- [`abroot`](/docs/ABRoot)
- [`kso`](/docs/kso)

## AUTHOR

```text
Mitwirkende von KOOMPI OS
```

## FEHLER MELDEN

Fehler bitte beim [Bugtracker](https://github.com/koompi-os/pix/issues) melden.
