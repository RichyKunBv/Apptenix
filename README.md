# 🐧 Apptenix - Gestor de Aplicaciones para Linux

[![Versión](https://img.shields.io/badge/Versión-1.1-blue.svg)](https://github.com/RichyKunBv/Apptenix)
[![Licencia](https://img.shields.io/badge/Licencia-Apache-green.svg)](https://github.com/RichyKunBv/Apptenix/blob/main/LICENSE)
[![Lenguaje](https://img.shields.io/badge/Lenguaje-Bash-lightgrey.svg)](https://github.com/RichyKunBv/Apptenix)

Un script de terminal para instalar, gestionar y desinstalar aplicaciones portátiles de Linux de forma sencilla, inteligente y sin pereza.

---

## 🤔 ¿Qué es esto?

Este proyecto nació de la pereza de tener que instalar manualmente aplicaciones que vienen en archivos comprimidos (`.zip`, `.tar.gz`, etc.). En lugar de mover carpetas, crear accesos directos y enlaces a mano, este script lo automatiza todo a través de un menú interactivo en la terminal.

Ha evolucionado a un gestor completo (**Apptenix**) que no solo instala, sino que también lleva un registro de tus aplicaciones, las desinstala limpiamente y se mantiene actualizado.

## ✨ Características Principales

* **INSTALADOR INTELIGENTE:**
    * 🧠 **Análisis de Dependencias:** Revisa el ejecutable y te avisa si te faltan librerías (`.so`) para que la aplicación funcione.
    * 🔎 **Detección Automática:** Detecta paquetes oficiales con archivos `.desktop` para autocompletar nombre, ejecutable e icono.
    * ⚠️ **Detector de Duplicados:** Te advierte si intentas instalar una aplicación que ya tienes registrada.
    * 📂 **Opciones de Instalación:** Instala localmente (`~/Applications`) o para todo el sistema (`/opt`).

* **GESTOR COMPLETO:**
    * ✅ **Instalación Guiada y Automática:** Te lleva paso a paso (o lo hace automáticamente) para instalar, crear accesos directos en el menú y comandos en la terminal.
    * ❌ **Desinstalación Segura:** Borra todos los archivos de una aplicación. ¡Incluso detecta si la app está en ejecución y te ofrece cerrarla!
    * 📋 **Listado de Apps:** Muestra un resumen de todas las aplicaciones que has instalado con la herramienta.

* **MÁXIMA COMPATIBILIDAD:**
    * 📦 **Soporte Amplio de Formatos:** Funciona con `.zip`, `.tar.gz`, `.tar.xz`, `.tar.bz2`, `.7z` y hasta con **binarios simples** sin comprimir.
    * 🔄 **Auto-Actualización:** Se mantiene al día con la última versión directamente desde GitHub.

---

## 🚀 Instalación y Uso

1.  **Descarga el script** con `wget` o `curl`:
    ```bash
    wget https://raw.githubusercontent.com/RichyKunBv/Apptenix/main/Apptenix.sh
    ```
2.  **Dale permisos de ejecución:**
    ```bash
    chmod +x Apptenix.sh
    ```
3.  **Ejecútalo:**
    ```bash
    ./Apptenix.sh
    ```
4.  **Usa el menú interactivo** para instalar, desinstalar, listar o actualizar tus aplicaciones.

---

## 🛠️ Dependencias

Para que todas las funciones operen correctamente, asegúrate de tener instalados los siguientes paquetes:
* `curl` o `wget` (para la auto-actualización)
* `unzip` (para archivos `.zip`)
* `tar` (para archivos `.tar.*`)
* `p7zip-full` (en Debian/Ubuntu) o `p7zip` (en Arch/Fedora) (para archivos `.7z`)
* `rsync` (opcional, para una copia más rápida)

---

## 📝 Estado del Proyecto

**Versión 1.1 - Estable.** Apptenix es un gestor de aplicaciones maduro y con funcionalidades completas.
