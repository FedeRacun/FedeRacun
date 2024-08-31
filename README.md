# Frontend Developer 🖥️  
## [.JS | .TS] 📚

## Readme Demo

### ✨ Bienvenido al equipo!
Se que estas emocionado por poner manos a la obra pero antes de comenzar te pido que dediques el tiempo necesario para leer este documento, seguro te de una mejor comprensión del proyecto y te ahorre algun que otro problema a futuro. Sin nada mas que decir, comenzamos:


### 📦 Instalaciones necesarias

1. Verifica tener la ultima version de Node instalada, puedes descargarla desde el [sitio oficial](https://nodejs.org/en) o utilizar NVM haciendo `nvm use` en la raiz del proyecto. 

2. Utilizamos `pnpm`, es un gestor de paquetes de Node como npm o yarn pero mas rápido y ligero, puedes instalarlo haciendo `npm install -g pnpm` o [siguiendo estos pasos](https://pnpm.io/es/installation)

3. Una vez ya tengas pnpm ejecuta el comando `pnpm install` para instalar las dependencias

4. Listo! ya puedes iniciar el proyecto escribiendo `pnpm dev`


### 🔎 Datos relevantes
- El proyecto utiliza Tailwindcss pero **solo dentro los archivos SCSS**, nunca escribimos las clases de tailwind sobre los componentes de React

- Husky se encarga de indentar el codigo y buscar posibles errores o inconsistencias antes de cada commit, en caso de encontrar algo, **el commit se detendra** y deberas arreglarlo antes de volver a commitear

- Utilizamos `.gitkeep` para mantener las carpetas vacias y asi no perder la estructura del proyecto

- Las extensiones `Better Comments` y `Material Icon Theme` pueden brindarte una mejor experiencia de desarrollo en este proyecto


### ⚙️ Comandos utiles
- `pnpm format:write` | Revisa el proyecto y da formato a todo lo que no este alineado a las reglas de Prettier

- `pnpm update:project` | Actualiza todas las dependencias a la ultima version estable que este registrada, ten en cuenta que puede generar breaking change.

- `clean:install` | Realiza una instalacion limpia de todos los paquetes de Node, **solo funciona en linux**


### 📐 Entendiendo la arquitectura
La estructura de este proyecto esta inspirada gran parte en estos videos, si tienes curiosidad puedes verlos:

1. [Qué es Clean Architecture en Frontend?](https://www.youtube.com/watch?v=vRGVnqylO68&t=2417s&ab_channel=GentlemanProgramming)

2. [Cómo estructurar un proyecto en react? 1/2](https://youtu.be/5LqhlCd2_nE)

3. [Cómo estructurar un proyecto en react? 2/2](https://youtu.be/XEcZaKK38fg)

4. [Cómo funcionan las rutas?](https://youtu.be/UVsX7A2wfLo)

### ➡️ Workflow de GIT
Para que a simple vista sea facil identificar cada branch y cada pull request establecemos una convencion a respetar en los nombres de los branch <br>
La estructura es `[tipo]/[pantalla o componente]-[descripcion o detalle]` los tipos pueden ser:
   - feature:     Nueva característica para el usuario
   - fix:      Corrección de errores
   - docs:     Cambios en la documentación
   - style:    Cambios en el formato/código que no afectan la lógica
   - refactor: Refactorización del código
   - test:     Añadiendo o mejorando pruebas

Un ejemplo seria `feature/stepper-custom_progressBar`


### 📄 Documenta tus componentes
Aqui te brindo un template para que puedas documentar todo componente o cambio que sumes

```md
# Nombre del Componente
Descripción breve del componente y su propósito.


## Ejemplo de Uso

```jsx
import React from 'react';
import NombreDelComponente from 'nombre-del-componente';

const MiComponente = () => {
  return (
    <div>
      <NombreDelComponente prop1="valor1" prop2="valor2" />
    </div>
  );
};


## Propiedades (Props)

| Propiedad | Tipo     | Descripción                      |
| --------- | -------- | -------------------------------- |
| prop1     | tipo1    | Descripción de la primera prop.  |
| prop2     | tipo2    | Descripción de la segunda prop.  |

## Ejemplos Adicionales

Incluye aquí más ejemplos y casos de uso para ayudar a los usuarios a comprender mejor cómo utilizar el componente en diversas situaciones.

## Notas Importantes

- Ten en cuenta que...
- Este componente no es adecuado para...

```

### 🗺️ Componentes actuales
#### [Comp1](src/components/stepper/readme.md) | Es un componente 1
#### [Comp2](src/components/inputStep/readme.md) | Es un componente 2
