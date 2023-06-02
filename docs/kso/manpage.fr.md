---
title: Manpage kso - KOOMPI OS
description: Manpage pour l'utilitaire vso.
---

# Manpage `kso`

## NOM

```text
kso est un utilitaire qui vous permet de réaliser des taches de maintenance sur votre installation KOOMPI OS.
```

## SYNOPSIS

```text
kso [options] [commande] [arguments]
```

## DESCRIPTION

```markdown
Utilisation: 
    kso [options] [commande] [arguments]

Options:
    -h, --help            Afficher ce message d'aide et quitter

Commandes:
    config                  Configurer VSO
    create-task             Créer une nouvelle tache
    delete-task             Supprimer une tache
    developer-program       Rejoindre le programme développeurs
    help                    Afficher ce message d'aide et quitter
    list-tasks              Lister toutes les taches
    rotate-tasks            Faire tourner les taches
    trigger-update          Actionner une mise à jour système
    version                 Afficher la version et quitter
```

## CONFIGURATION

```markdown
Description: 
    Configurer VSO

Utilisation:
    kso config [options] [commande]

Options:
    --help/-h           afficher ce message
    --assume-yes/-y     supposer oui à toutes les questions

Commandes:
    show                afficher la configuration actuelle
    get <key>           obtenir une valeur de configuration
    set <key> <value>   définir une valeur de configuration

Exemples:
    kso config get updates::schedule
    kso config set updates::schedule weekly
```

## CREER UNE TACHE

```markdown
Description: 
    Créer une nouvelle tache

Utilisation:
    kso create-task [options] [arguments]

Options:
    --help/-h               afficher ce message

Arguments:
    --name/-n               nom de la tache
    --description/-d        description de la tache
    --need-confirm          demander confirmation avant d'exécuter la tache
    --command/-c            commande pour exécuter
    --after-task            exécuter la tache après une autre tache
    --after-task-success    exécuter la tache après une autre tache si elle a réussi
    --after-task-failure    exécuter la tache après une autre tache si elle a échoué
    --every/-e              exécuter la tache toute les X (minutes, heures, jours)
    --at/-a                 exécuter la tache à un temps spécifique (hh:mm)
    --on-boot               exécuter la tache au démarrage
    --on-shutdown           exécuter la tache à l'arrêt
    --on-login              exécuter la tache à la connexion
    --on-network            exécuter la tache à la connexion réseau
    --on-disconnect         exécuter la tache à la déconnexion réseau
    --on-battery            exécuter la tache sur batterie
    --on-low-battery        exécuter la tache sur batterie faible (20%)
    --on-charge             exécuter la tache sur batterie en charge
    --on-full-battery       exécuter la tache sur batterie pleine
    --on-condition-command  exécuter la tache sur commande conditionnelle
    --on-process            exécuter la tache lorsqu'un processus apparait

Exemples:
    kso create-task -n "Batterie pleinement chargée" -d "notifier lors du chargement complet" -c "notify-send 'Batterie pleinement chargée'" --on-full-battery
    kso create-task -n "Lancer-terminal" -d "Lancer le terminal lors du lancement des Paramètres" -c "kgx" --on-process gnome-control-center
```

## SUPPRIMER UNE TACHE

```markdown
Description: 
    Supprimer une tache

Utilisation:
    kso delete-task [tache] [options]

Options:
    --help/-h       afficher ce message

Exemples:
    kso delete-task ma-tache
    kso delete-task "ma tache"
```

## PROGRAMME DEVELOPPEURS

```markdown
Description: 
    Rejoindre le programme développeurs

Utilisation:
    kso developer-program [options]

Options:
    --help/-h       afficher ce message

Exemples:
    kso developer-program
```

## LISTER LES TACHES

```markdown
Description: 
    Lister toutes les taches

Usage:
    kso list-tasks [options]

Options:
    --help/-h       afficher ce message

Examples:
    kso list-tasks
```

## FAIRE TOURNER LES TACHES

```markdown
Description: 
    Faire tourner les taches

Usage:
    kso rotate-tasks [options]

Options:
    --help/-h       afficher ce message

Examples:
    kso rotate-tasks
```

## ACTIONNER UNE MISE A JOUR

```markdown
Description: 
    Actionner une mise à jour système

Usage:
    kso trigger-update [options]

Options:
    --help/-h       afficher ce message
    --now           actionner une mise à jour système immédiatement

Examples:
    kso trigger-update --now
```

## CONSULTER EGALEMENT

- [`pix`](/docs/pix)
- [`abroot`](/docs/kso)

## AUTEUR

```text
Les contributeurs de KOOMPI OS, dont D-Maxwell (traducteur)
```

## SIGNALER DES BUGS

Signalez des bugs sur le [recenseur de problèmes](https://github.com/koompi-os/vanilla-system-operator/issues).
