---
title: Manpage kso - KOOMPI OS
description: Manpage for the kso utility.
---

# Manpage `kso`

## NAME

```text
kso is an utility which allows you to perform maintenance tasks on your KOOMPI OS installation.
```

## SYNOPSIS

```text
kso [options] [command] [arguments]
```

## DESCRIPTION

```markdown
Usage: 
    kso [options] [command] [arguments]

Options:
    -h, --help            Show this help message and exit

Commands:
    config                  Configure VSO
    create-task             Create a new task
    delete-task             Delete a task
    developer-program       Join the developers program
    help                    Show this help message and exit
    list-tasks              List all tasks
    rotate-tasks            Rotate tasks
    trigger-update          Trigger a system update
    version                 Show version and exit`
```

## CONFIG

```markdown
Description: 
    Configure VSO

Usage:
    kso config [options] [command]

Options:
    --help/-h           show this message
    --assume-yes/-y     assume yes to all questions

Commands:
    show                show current configuration
    get <key>           get a configuration value
    set <key> <value>   set a configuration value

Examples:
    kso config get updates::schedule
    kso config set updates::schedule weekly
```

## CREATE TASK

```markdown
Description: 
    Create a new task

Usage:
    kso create-task [options] [arguments]

Options:
    --help/-h               show this message

Arguments:
    --name/-n               name of the task
    --description/-d        description of the task
    --need-confirm          ask for confirmation before executing the task
    --command/-c            command to execute
    --after-task            execute the task after another task
    --after-task-success    execute the task after another task if it was successful
    --after-task-failure    execute the task after another task if it failed
    --every/-e              execute the task every X (minutes, hours, days)
    --at/-a                 execute the task at a specific time (hh:mm)
    --on-boot               execute the task on boot
    --on-shutdown           execute the task on shutdown
    --on-login              execute the task on login
    --on-network            execute the task on network connection
    --on-disconnect         execute the task on network disconnection
    --on-battery            execute the task on battery
    --on-low-battery        execute the task on low battery (20%)
    --on-charge             execute the task on battery charging
    --on-full-battery       execute the task on full battery
    --on-condition-command  execute the task on condition command
    --on-process            execute the task when a process comes up

Examples:
    kso create-task -n "Battery fully charged" -d "notify at full charge" -c "notify-send 'Battery fully charged'" --on-full-battery
    kso create-task -n "Launch-terminal" -d "Launch terminal at Settings launch" -c "kgx" --on-process gnome-control-center
```

## DELETE TASK

```markdown
Description: 
    Delete a task

Usage:
    kso delete-task [task] [options]

Options:
    --help/-h       show this message

Examples:
    kso delete-task my-task
    kso delete-task "my task"
```

## DEVELOPER PROGRAM

```markdown
Description: 
    Join the developers program

Usage:
    kso developer-program [options]

Options:
    --help/-h       show this message

Examples:
    kso developer-program
```

## LIST TASKS

```markdown
Description: 
    List all tasks

Usage:
    kso list-tasks [options]

Options:
    --help/-h       show this message

Examples:
    kso list-tasks
```

## ROTATE TASKS

```markdown
Description: 
    Rotate tasks

Usage:
    kso rotate-tasks [options]

Options:
    --help/-h       show this message

Examples:
    kso rotate-tasks
```

## TRIGGER UPDATE

```markdown
Description: 
    Trigger a system update

Usage:
    kso trigger-update [options]

Options:
    --help/-h       show this message
    --now           trigger a system update immediately

Examples:
    kso trigger-update --now
```

## SEE ALSO

- [`pix`](/docs/pix)
- [`abroot`](/docs/kso)

## AUTHOR

```text
Contributors of KOOMPI OS
```

## REPORTING BUGS

Report bugs to the [issue tracker](https://github.com/koompi-os/vanilla-system-operator/issues).
