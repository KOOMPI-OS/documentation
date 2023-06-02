---
Título: Manual pix - KOOMPI OS
Descripción: Manual para pix.
---

# Manual `pix`

## NOMBRE

```text
`pix` es el administrador de paquetes de KOOMPI OS que es fácil de usar para instalar paquetes de múltiples fuentes dentro de contenedores sin la necesidad de alterar el sistema de archivos raíz.
```

## SINOPSIS

```text
pix [opciones] [comando] [argumentos]
```

## DESCRIPCIÓN

```markdown
pix is a wrapper around multiple package managers to install packages and run commands inside a managed container.
pix es un envoltorio alrededor de múltiples administradores de paquetes para realizar la instalación de paquetes y ejecutar comandos dentro de un contenedor.

Uso:
    pix [opciones] [comando] [argumentos]

Opciones:
    -h, --help      Muestra este mensaje
    -v, --version   Muestra la versión
    --aur           Instala paquetes desde el repositorio AUR
    --dnf           Instala paquetes desde los repositorios de Fedora Linux

Commands:
    autoremove      Elimina todos los paquetes no utilizados
    clean           Limpia la caché de pix
    enter           Entra al shell del contenedor
    export          Exporta/Recrea el acceso directo de un programa del contenedor
    help            Muestra este mensaje
    init            Inicializa un contenedor
    install         Instala paquetes dentro del contenedor
    list            Lista todos los paquetes instalados
    log             Muestra los registros
    purge           Purga los paquetes del contenedor
    run             Ejecuta un comando dentro del contenedor
    remove          Elimina paquetes del contenedor
    search          Buscar paquetes
    show            Muestra los detalles de un paquete
    unexport        Elimina el acceso directo de un programa
    update          Actualiza los repositorios de paquetes disponibles
    upgrade         Actualiza todo el sistema instalando/actualizado los paquetes disponibles
```

## AUTOREMOVE (autoremover)

```markdown
Descripción: 
    Elimina todos los paquetes no utilizados.
Uso:
    pix autoremove [opciones]

Opciones:
    -h, --help            Muestra este mensaje

Uso:
    pix autoremove
```

## CLEAN (limpiar)

```markdown
Descrición: 
    Limpia la caché de pix.

Uso:
    pix clean [opciones]

Opciones:
    -h, --help            Muestra este mensaje

Ejemplo:
    pix clean
```

## ENTER (entrar)

```markdown
Descripción: 
    Entra al shell del contenedor.

Uso:
    pix enter [opciones]

Opciones:
    -h, --help            Muestra este mensaje
```

## EXPORT (exportar)

```markdown
Descripción: 
    Exporta/Recrea el acceso directo de un programa del contenedor.

Uso:
    pix export <programa> [opciones]

Opciones:
    -h, --help            Muestra este mensaje

Ejemplo:
    pix export htop
```

## INIT (inicializar)

```markdown
Descripción: 
    Inicializa un contenedor.

Uso:
    pix init [opciones]

Opciones:
    -h, --help            Muestra este mensaje
```

## INSTALL (instalar)

```markdown
Descripción: 
    Instala paquetes dentro del contenedor.

Uso:
    pix install [opciones] <paquetes>

Opciones:
    -h, --help            Muestra este mensaje
    -y, --assume-yes      Proceder sin confirmación manual.
    -f, --fix-broken      Reparar dependencias rotas antes de instalar.
    --no-export           No exportar acceso directo después de instalar.
    --sideload [ruta]     Instalar un paquete desde un archivo local.

Ejemplos:
    pix install htop git
    pix install --sideload /path/to/file.deb
```

## LIST (listar)

```markdown
Descripción: 
    Lista todos los paquetes instalados.

Uso:
    pix list [opciones]

Opciones:
    -h, --help            Muestra este mensaje
```

## LOG (registro/bitácora)

```markdown
Descripción: 
    Muestra los registros.

Uso:
    pix log [opciones]

Opciones:
    -h, --help            Muestra este mensaje
```

## PURGE (purgar)

```markdown
Descripción: 
    Purga los paquetes del contenedor.

Uso:
    pix purge <paquetes> [opciones]

Opciones:
    -h, --help            Show this help message and exit

Ejemplos:
    pix purge htop
```

## RUN (correr/ejecutar)

```markdown
Descripción: 
    Ejecuta un comando dentro del contenedor.

Uso:
    pix run <programa> [opciones]

Opciones:
    -h, --help            Muestra este mensaje

Ejemplo:
    pix run htop
```

## REMOVE (remover)

```markdown
Descripción:
    Elimina paquetes del contenedor.

Uso:
    pix remove <paquetes> [opciones]

Opciones:
    -h, --help            Muestra este mensaje

Ejemplo:
    pix remove htop
```

## SEARCH (buscar)

```markdown
Descripción: 
    Buscar paquetes.

Uso
    pix search <paquetes> [opciones]

Opciones:
    -h, --help            Muestra este mensaje

Ejemplo:
    pix search htop
```

## SHOW (mostrar)

```markdown
Descripción: 
    Muestra los detalles de un paquete.

Uso:
    pix show <paquete> [opciones]

Opciones:
    -h, --help            Muestra este mensaje

Ejemplo:
    pix show htop
```

## UNEXPORT (des-exportar)

```markdown
Descripción:
    Elimina el acceso directo de un programa.

Uso:
    pix unexport <programa> [opciones]

Opciones:
    -h, --help            Muestra este mensaje

Ejemplo:
    pix unexport htop
```

## UPDATE (actualizar)

```markdown
Descripción: 
    Actualiza los repositorios de paquetes disponibles.

Uso:
    pix update [opciones]

Opciones:
    -h, --help            Muestra este mensaje

Ejemplo:
    pix update
```

## UPGRADE (mejorar)

```markdown
Descripción: 
    Actualiza todo el sistema instalando/actualizado los paquetes disponibles.

Uso:
    pix upgrade [opciones]

Opciones:
    -h, --help            Muestra este mensaje

Ejemplo:
    pix upgrade
```

## VERSION

```markdown
Descripción:
    Muestra la versión.

Uso:
    pix --version
    pix -v
```

## VEA TAMBIÉN

- [`abroot`](/docs/ABRoot)
- [`kso`](/docs/kso)

## AUTOR

```text
@JMarcosHP
```

## REPORTE DE ERRORES

Reportar los errores al [rastreador de problemas](https://github.com/koompi-os/ABRoot/issues).
