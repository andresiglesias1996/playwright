# Pruebas Automatizadas con Playwright

## DescripciónEste proyecto utiliza 

[Playwright](https://playwright.dev/docs/intro) para realizar pruebas automatizadas Web.

## Tabla de Contenidos
- [Descripción](#descripción)
- [Prerequisitos](#prerequisitos)
- [Instalación](#instalación)
- [Configuración](#configuración)
- [Ejecución de Pruebas](#ejecución-de-pruebas)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Solución de Problemas](#solución-de-problemas)

## Prerequisitos
Antes de comenzar, asegúrate de tener instalado lo siguiente en tu sistema:
- [Node.js](https://nodejs.org/) (versión 14 o superior)
- [npm](https://www.npmjs.com/) o [Yarn](https://yarnpkg.com/)

## Instalación
Sigue estos pasos para configurar el proyecto en tu máquina local:
1. **Clona el Repositorio**
```bash   
git clone https://github.com/tu-usuario/tu-repositorio.git 
cd tu-repositorio 
```
2. **Instala las Dependencias**Utiliza npm para instalar las dependencias del proyecto.
```bash
    npm install
```
3. **Instala los Navegadores de Playwright**
Playwright requiere la descarga de navegadores específicos para ejecutar las pruebas. Ejecuta el siguiente comando:
```bash
npx playwright install
```
## ConfiguraciónConfigura las variables de entorno necesarias para ejecutar las pruebas correctamente.
1. **Crea un Archivo .env** 
En la raíz del proyecto, crea un archivo llamado .env y añade las variables:
```bash

```
2. **Instala dotenv (si aún no está instalado)**
```bash
npm install dotenv
```
## **Ejecución de Pruebas** 
Es la mejor experiencia para automatizar
```bash
npx playwright test
 --ui
 ```
1. **Ejecuta Todas las Pruebas**
```bash
npx playwright test
```
2. **Ejecuta una Prueba Específica**
```bash
npx playwright test tests/login.spec.js
```
3. **Ejecutar en Modo de Depuración**
Para depurar las pruebas y ver el navegador en acción:
```bash
npx playwright test --debug
```
3. **Generar Código con Codegenn**
Playwright incluye una herramienta para generar código automáticamente a partir de interacciones en el navegador. Usa el siguiente comando:
```bash
npx playwright codegen
```
Esto abrirá un navegador donde puedes realizar acciones manuales y generara el codigo correspondiente.

## **Test reports**
```bash
npx playwright show-report
```




## **Estructura del Proyecto**
La estructura recomendada para el proyecto es la siguiente:
/project-root
│
├── /tests
│   └── example.spec.ts
│
├── /utils
│   └── comandosPersonalizados.ts
│
├── playwright.config.ts
├── package.json
├── .env
└── README.md

/tests: Archivos de pruebas.
/utils: Utilidades y comandos personalizados.
playwright.config.ts: Configuración de Playwright.
.env: Variables de entorno.
README.md: Documentación.


## **Solución de Problemas**





