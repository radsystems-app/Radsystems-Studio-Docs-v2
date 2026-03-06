---
title: Requerimientos del Sistema
description: RadSystems Studio consume muy pocos recursos del sistema.
published: true
date: 2023-09-17T23:49:03.186Z
tags: sistema, recursos
editor: markdown
dateCreated: 2023-09-17T20:55:24.964Z
---

# Requisitos del Sistema
RadSystems ofrece varias opciones para elegir tu stack de desarrollo. Sin embargo, es importante tener en cuenta que algunas herramientas y aplicaciones de terceros necesarias para configurar tu entorno de desarrollo local no están incluidas en la Configuración de Instalación de la Aplicación RadSystems Studio. Dependiendo del conjunto de desarrollo que elijas, se recomienda instalar las siguientes herramientas de desarrollo, frameworks y aplicaciones por separado.

## Requisitos del Sistema de la Computadora
- SO Compatible: Windows 7, Windows 8, Windows 10, Windows 11
- Mínimo de 4 GB de RAM (se recomiendan 8 GB o más)
- Procesador de cuatro núcleos o superior para un rendimiento óptimo
- Pantalla de alta resolución (Full HD o superior)
- Conexión a Internet activa para la gestión de paquetes y actualizaciones

**Nota:**

- Hasta ahora, RadSystems Studio es compatible exclusivamente con el Sistema Operativo (SO) de Windows, específicamente las versiones Windows x86/x64 (7, 8, 10, 11).
- Si estás trabajando con un sistema operativo diferente, la solución implica configurar una Máquina Virtual (VM) utilizando herramientas de virtualización como Wine, VirtualBox, VMWare, etc., e instalar el SO de Windows compatible dentro de esa VM. Esto te permite instalar RadSystems Studio con éxito dentro del entorno de la Máquina Virtual.

## Stack de Desarrollo
## DevelopmentStackTabs{.tabset}
### Frameworks de Backend
**1. PHP Laravel 10 (PHP 8.xx)**

- XAMPP
- PHP 8.xx
- MySQL u otra base de datos compatible de tu elección

**2. Python Flask (Python 3.8)**

- Python 3.8
- Pip (Instalador de Paquetes de Python)
- MySQL o SQLite u otra base de datos compatible de tu elección

**3. Node ExpressJS (NodeJS <= 16)**

- Node.js (v16 o inferior)
- npm (Administrador de Paquetes de Node)
- Cualquier base de datos de tu elección

**4. ASP .Net Core**

- .NET Core SDK
- MySQL o SQL Server u otra base de datos compatible de tu elección

### Frameworks de Frontend

**1. Framework Quasar**

- Node.js (se recomienda v14+)
- npm (Administrador de Paquetes de Node)
- Quasar CLI
- Cualquier base de datos compatible de tu elección

**2. PrimeVue**

- Node.js (se recomienda v14+)
- npm (Administrador de Paquetes de Node)
- Vue.js CLI
- Cualquier base de datos compatible de tu elección

**3. PrimeReact**

- Node.js (se recomienda v14+)
- npm (Administrador de Paquetes de Node)
- Vue.js CLI
- Cualquier base de datos compatible de tu elección

## Herramientas de Desarrollo

RadSystems Studio ofrece una plataforma completa para construir aplicaciones web, móviles y de escritorio dinámicas utilizando tecnología de bases de datos. Sin embargo, tener ciertas herramientas instaladas en tu máquina de desarrollo puede mejorar significativamente tu experiencia durante las fases de prueba, depuración y generación de ideas del desarrollo de la aplicación. Al aprovechar estas herramientas junto con RadSystems Studio, obtienes acceso a capacidades avanzadas que agilizan tu flujo de trabajo y permiten una creación más eficiente de soluciones de software innovadoras.

1. **Visual Studio Code** o cualquier otro editor de código similar.
2. **Android Studio:** Un entorno de desarrollo integrado (IDE) diseñado para el desarrollo de aplicaciones Android. Simplifica el proceso de creación, prueba y depuración de aplicaciones 
3. **Software Cliente de Gestión de Bases de Datos:** Software como phpMyAdmin u otra aplicación de escritorio de Windows que proporciona una forma de crear, gestionar y manipular bases de datos en LocalHost. Estas herramientas facilitan la administración y manipulación eficientes de la base de datos, lo cual es fundamental para muchos proyectos de desarrollo de aplicaciones.
