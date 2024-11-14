
# Summary

- lista de comandos consejos, y sugerencias para administrar y manipular WSL (Windows sub-System for Linux)

# General objectives

- Aprender a utilizar WSL de forma profesional.

# Specific objectives

- Instalar, configurar, modificar WSL.

- Aprender a utilizar Visual Studio Code en el WSL.

- Aprender a usar Linux desde la terminal.


# WSL Commands Guide

Este documento proporciona una guía rápida de comandos para manejar el Subsistema de Windows para Linux (WSL).

---

## Índice

- [Instalación de WSL](#instalación-de-wsl)
- [Gestión de Distribuciones Linux](#gestión-de-distribuciones-linux)
- [Referencias](#referencias)

---

## Instalación de WSL

Aquí encontrarás los comandos principales para instalar y actualizar WSL en Windows.

```bash
wsl --version           # Ver la versión de WSL instalada
wsl --update            # Actualizar WSL a la última versión
wsl --install           # Instalar WSL y la distribución predeterminada
wsl --status            # Ver el estado actual de WSL
wsl --help              # Mostrar la ayuda de WSL
wsl --unregister <DistributionName>  # Desinstalar una distribución específica


Gestión de Distribuciones Linux
Comandos para listar, instalar, configurar y administrar distribuciones en WSL.

Listado y Configuración de Distribuciones

wsl --list --online             # Listar distribuciones disponibles para instalar
wsl --list --verbose            # Listar distribuciones instaladas con detalles

wsl --install <NameDistro>      # Instalar una distribución específica
wsl --set-default <Distribution Name>  # Establecer una distribución como predeterminada

Configuración Adicional

wsl --inbox                     # Ejecutar WSL desde la bandeja de entrada (opción avanzada)
wsl --no-distribution           # Ejecutar WSL sin distribución (opción avanzada)

Control de Sesión y Usuario

wsl --shutdown                      # Apagar todas las instancias de WSL
wsl --terminate <Distribution Name> # Terminar una instancia específica de distribución
wsl --user <Username>               # Establecer un usuario predeterminado
<DistributionName> config --default-user <Username>  # Configurar el usuario predeterminado para una distribución específica

Otros Comandos Útiles

wsl ~                           # Iniciar sesión en el directorio home
exit                            # Salir de la sesión de WSL


Referencias
Para más información sobre los comandos de WSL, consulta la documentación oficial:

Comandos básicos de WSL (en español)
Configuración del entorno de WSL (en inglés)


Este archivo `README.md` está organizado para facilitar el acceso a los diferentes comandos y opciones que ofrece WSL, incluyendo secciones de instalación, gestión de distribuciones y referencias.

#Bibliography
