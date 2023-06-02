---
Título: Documentación de KOOMPI OS
Descripción: Descubra cómo utilizar KOOMPI OS y todas sus herramientas y ajustes.
---

# KOOMPI OS

*Pruebe la experiencia de GNOME Vanilla en Ubuntu con algunos condimentos.*

**Está página es la documentación oficial para los componentes de KOOMPI OS en su edición en Español.**\
Lea el [**Manual**](https://handbook.koompios.org) para aprender guías y tutoriales escritos por la comunidad.

## PREGUNTAS FRECUENTES

Respuestas a las preguntas más frecuentes (aunque el proyecto es muy joven).
- **¿Por qué una nueva distribución?**\
  KOOMPI OS surgió de la necesidad de una distribución de Linux basada en Ubuntu que 
  proporcionara GNOME vanilla sin ningún cambio en la experiencia 
  de usuario. Más tarde, su alcance se amplió para experimentar con algunas herramientas y 
  tecnologías, como ABRoot y pix (el 
  subsistema basado en Distrobox).
  
- **¿Utiliza OSTree?**\
  No. KOOMPI OS consigue la inmutabilidad a través de [`ABRoot`](https://github.com/koompi-os/ABRoot)[anteriormente lo conseguíamos gracias a la utilidad `almost`]. El uso de OSTree se considerará en el futuro.
  
  Escribimos esta utilidad para la inmutabilidad bajo demanda basada en el 
  atributo de inmutabilidad de los archivos. Este enfoque funciona en cualquier partición 
  del sistema de archivos/esquema de particiones.
  
  Actualmente hemos introducido otra nueva utilidad para conseguir la inmutabilidad bajo demanda
  llamada [`ABRoot`](https://github.com/koompi-os/ABRoot) reemplazando a `almost` para proveer una completa inmutabilidad y atomicidad, al realizar las transacciones entre 2 particiones raíz (A⟺B). También se consiguen las transacciones bajo demanda gracias al shell transaccional.
  
- **Lanzamiento contínuo**\
  No. KOOMPI OS es un lanzamiento puntual y sigue el ciclo de lanzamiento de Ubuntu.

## Documentación

- **[Instalación](https://handbook.koompios.org/2022/11/05/installation.html)**\
Instrucciones para la instalación del sistema mediante [Vanilla Installer](https://github.com/koompi-os/vanilla-installer).

- **[Configuración Inicial](https://handbook.koompios.org/2022/11/18/first-setup.html)**\
Con la utilidad de [Configuración Inicial](https://github.com/koompi-os/first-setup) que proporciona KOOMPI OS, usted podrá ajustar su sistema a sus necesidades.

- **[Administrador de paquetes (`pix`)](/docs/pix)**\
pix es un administrador de paquetes que permite instalar y gestionar paquetes en un
contenedor gestionado, sin afectar al sistema anfitrión. `pix` puede instalar paquetes de los repositorios oficiales de Ubuntu, pero no solo eso, tambien de Arch User Repository (AUR) y de los repositorios DNF de Fedora dentro de un contenedor. Está muy bien integrado con el sistema anfitrión. Para los paquetes con interfaz gráfica (GUI), un acceso directo se creará automáticamente y se agragará al menú de aplicaciones de GNOME.

- **[Operador del Sistema de Vanilla (`KSO por sus siglas en inglés`)](/docs/kso)**\
El [Operador del Sistema de Vanilla](/docs/kso) es una utilidad de KOOMPI OS que le permite realizar tareas de mantenimiento como actualizar el software, programar tareas, etc.

- **[Panel de Control de Vanilla](https://github.com/koompi-os/vanilla-control-center)**\
Es una utilidad que le permite configurar las [actualizaciones](https://handbook.koompios.org/2022/12/10/updates.html) e instalar [controladores adicionales](https://handbook.koompios.org/2022/12/10/install-additional-drivers.html) en su sistema.

- **[Inmutabilidad (`almost`)](/docs/almost)**\
~~[Almost](https://github.com/koompi-os/almost) es una utilidad para la inmutabilidad bajo demanda basada
en el atributo de inmutabilidad de los archivos.~~ (Almost fue reemplazado por `ABRoot`).
