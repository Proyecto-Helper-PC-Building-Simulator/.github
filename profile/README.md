# PC Building Simulator (Proyecto) - Documentación

> [!IMPORTANT]
>
> Este proyecto no trata sobre el videojuego del mismo nombre, si no en una aplicación que ayude a los jugadores a gestionar sus partidas.

## Introducción

Este proyecto consiste en un sistema de gestión de tareas del videojuego PC Building Simulator.

Consta de:

- Una **base de datos** con los datos de los componentes de ordenador.
- Una **API** desarrollada con SpringBoot JPA para gestionar las operaciones
- Una **aplicación móvil** desarrollada con Flutter para que los usuarios interactúen con el sistema.

## Arquitectura general

![Diagrama de despliegue](https://www.plantuml.com/plantuml/png/RP112eD034NtSuhWtZkek6cX8BWiNGnEQWFJYMHIDwMdyWXUh5gAj3BPXFpyzmCfebhHnzqRZrS5PH3gRmgE13ib3iO4TWXPYpAIOu5bg6p4jTTMEMRmDB3K-K-zc5UAB9l3vcy7eT13nQnmRCeVegOuS2IbaU4qJoFv3Ie7JvtjQ9x2T_NXTiSXpnFvUsMrfHCB36xvoHi0)

<details>

<summary>Ver código (PlantUML)</summary>

```plantuml
left to right direction

node "Servidor de Base de Datos" {
    [Base de Datos]
}

node "Servidor de API" {
    [Spring Boot JPA]
}

node "Dispositivo Móvil" {
    [Aplicación Móvil]
}

[Base de Datos] -- [Spring Boot JPA]
[Spring Boot JPA] -- [Aplicación Móvil]
```

</details>

> [!NOTE]
>
> Si se fuese a poner en desarrollo se usarían 2 servidores. Al ser un proyecto personal tan solo es una representación.

## Base de datos

[Para ver más información haz clic aquí](https://github.com/Proyecto-Helper-PC-Building-Simulator/database)

## API

[Para ver más información haz clic aquí](https://github.com/Proyecto-Helper-PC-Building-Simulator/api)

## Aplicación móvil

[Para ver más información haz clic aquí](https://github.com/Proyecto-Helper-PC-Building-Simulator/app_flutter)
