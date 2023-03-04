---
theme: default
background: https://images.unsplash.com/photo-1608433223113-bb8d2ee51eb3?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1935&q=80
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
fonts:
  # for code blocks, inline code, etc.
  mono: 'Fira Code'
drawings:
  persist: false
# page transition
transition: fade
# use UnoCSS
css: unocss
layout: cover
title: Inicio
---

<h1 class="font-mono font-bold">Recomendaciones para <br/> el desarrollo <br/> en Javascript.</h1>

---
layout: cover
class: 'font-mono'
title: Node
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Entorno local</span>
</div>

<div class="logo">
  <img src="/logos/LogosNodejsIcon.svg"/>
</div>

<div class="stars-downloads">
  <div >
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>75 Billones de descargas mensuales</span>
  </div>
</div>

- 🖥️ **NODE** - El entorno en el que se ejecuta javascript <br> tanto en el cliente como en el server (V8 de Chrome)

<small class="relative block -top-2 text-gray-400 text-xs ml-6">DENO y BUN son alternativas a NODE. Están aún en beta y no es la elección predilecta para usar en producción.</small>

- 📦 **NPM** - "Node Package Manager" es el ecosistema predeterminado de Node para agregar de librerias de código abierto. Lo compro Github. (Microsoft <img src="/logos/LogosMicrosoft.svg" class="inline-block w-4 h-4 relative -top-0.5">) <br> Lee las dependencias en el package.json (como el requirements.txt de python). 

<small class="relative block -top-2 text-gray-400 text-xs ml-6">Existen también YARN y PNPM. Lo importante es no mezclar y utilizar uno solo por proyecto.</small>

- ✨ **NVM** - "Node Version Manager" para manejar e <br> intercambiar versiones de node localmente.

- 🕹️ <small text-green-400><b>NPX</b> - Para ejecutar paquetes de node sin package.json ni carpeta node_modules.</small>

---
class: 'font-mono pt-24'
layout: center
title: Vite
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vite</span>
</div>

<div class="logo">
  <img src="/logos/LogosVitejs.svg"/>
</div>

<h3 mb-2> &#x2022; Herramienta para la compilación de proyectos JS/TS</h3>
<h3 mb-2> &#x2022; Mejora sustancial tanto para Dev como en Prod</h3>

<img src="/vite.png"/>

<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>3.500.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>53.4k</span>
  </div>
</div>


---
class: font-mono pt-16
title: Vite - Soporte
layout: cover
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span text-gray-100>Vite</span>
    <img src="/logos/chevron.svg"/>
  <span>Soporte</span>
</div>

<div class="logo">
  <img src="/logos/LogosVitejs.svg"/>
</div>

<img src="/vite-ecosystem.jpg" class="max-w-6xl w-full mt-2"/>

<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>3.500.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>53.4k</span>
  </div>
</div>




<!-- 

- Surgio gracias a los ES Modules que ahora soportan el navegadores.

- code-splitting and CSS handling

- crawl, process and concatenate


 -->


---
class: font-mono pt-24
title: Library Tier List
layout: cover
---


<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Librerias por niveles</span>
</div>

<div class="logo flex items-center">
  <p text-xs>State of Javascript 2022</p>
  <img src="/logos/LogosStateOfJavascript2022.jpg" ml-1/>
</div>

<img  src="/tier-list-all.jpg"/>


<style>
.slidev-page  {
  background: #272324;
}
</style>

---
class: font-mono pt-24
title: Library Tier List - Frontend
layout: cover
---


<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Librerias por niveles</span>
    <img src="/logos/chevron.svg"/>
  <span>Front-end Frameworks</span>
</div>

<div class="logo flex items-center">
  <p text-xs>State of Javascript 2022</p>
  <img src="/logos/LogosStateOfJavascript2022.jpg" ml-1/>
</div>

<img  src="/tier-list-frontend.jpg"/>


<style>
.slidev-page  {
  background: #272324;
}
</style>


---
class: font-mono pt-24
title: Library Tier List - Rendering
layout: cover
---


<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Librerias por niveles</span>
    <img src="/logos/chevron.svg"/>
  <span>Rendering Frameworks</span>
</div>

<div class="logo flex items-center">
  <p text-xs>State of Javascript 2022</p>
  <img src="/logos/LogosStateOfJavascript2022.jpg" ml-1/>
</div>

<img  src="/tier-list-rendering.jpg"/>


<style>
.slidev-page  {
  background: #272324;
}
</style>


---
class: font-mono pt-24
title: Library Tier List - Testing
layout: cover
---


<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Librerias por niveles</span>
    <img src="/logos/chevron.svg"/>
  <span>Testing</span>
</div>

<div class="logo flex items-center">
  <p text-xs>State of Javascript 2022</p>
  <img src="/logos/LogosStateOfJavascript2022.jpg" ml-1/>
</div>

<img  src="/tier-list-testing.jpg"/>


<style>
.slidev-page  {
  background: #272324;
}
</style>

---
class: font-mono pt-24
title: Library Tier List - Build
layout: cover
---


<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Librerias por niveles</span>
    <img src="/logos/chevron.svg"/>
  <span>Build Tools</span>
</div>

<div class="logo flex items-center">
  <p text-xs>State of Javascript 2022</p>
  <img src="/logos/LogosStateOfJavascript2022.jpg" ml-1/>
</div>

<img  src="/tier-list-build.jpg"/>


<style>
.slidev-page  {
  background: #272324;
}
</style>


---
class: font-mono pt-24
title: Library Tier List - Monorepos
layout: cover
---


<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Librerias por niveles</span>
    <img src="/logos/chevron.svg"/>
  <span>Monorepos</span>
</div>

<div class="logo flex items-center">
  <p text-xs>State of Javascript 2022</p>
  <img src="/logos/LogosStateOfJavascript2022.jpg" ml-1/>
</div>

<img  src="/tier-list-monorepos.jpg"/>


<style>
.slidev-page  {
  background: #272324;
}
</style>



---
class: font-mono pt-24
title: Frameworks
layout: cover
---


<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Frameworks</span>
</div>

<div class="logo flex items-center">
  <p text-xs>State of Javascript 2022</p>
  <img src="/logos/LogosStateOfJavascript2022.jpg" ml-1/>
</div>

<img  src="/retencion-frameworks.jpg"/>


<style>
.slidev-page  {
  background: #272324;
}
</style>


<!--

Esto tenerlo en el contexto de que cada vez mas gente usa js.

Y la mayoria por el Hype o la novedad eligio React.

-->

---
class: font-mono pt-24
title: Frameworks
layout: cover
---


<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Frameworks</span>
</div>

<div class="logo flex items-center">
  <p text-xs>State of Javascript 2022</p>
  <img src="/logos/LogosStateOfJavascript2022.jpg" ml-1/>
</div>

<img  src="/retencion-vue.jpg"/>


<style>
.slidev-page  {
  background: #272324;
}
</style>


---
class: font-mono pt-24
title: Frameworks
layout: cover
---


<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Frameworks</span>
</div>

<div class="logo flex items-center">
  <p text-xs>State of Javascript 2022</p>
  <img src="/logos/LogosStateOfJavascript2022.jpg" ml-1/>
</div>

<img  src="/usage-frameworks.jpg"/>


<style>
.slidev-page  {
  background: #272324;
}
</style>


---
class: 'font-mono pt-20'
title: Learn Vue
layout: center
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
</div>



<img src="/logos/LogosVue.svg" class="w-full h-32" />
<img src="/Vue-intro.png" class="w-full" />




---
class: 'font-mono pt-20'
title: Learn Vue
layout: center
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>LearnVue</span>
</div>

<div class="logo">
  <img src="/logos/LogosLearnVue.jpg"/>
</div>

### LearnVue es gran canal de youtube para aprender Vue.

<img src="/learnvue.jpg" class="-mx-2"/>


---
class: font-mono pt-16
title: Vue3
layout: cover
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span text-gray-100>Vue</span>
    <img src="/logos/chevron.svg"/>
  <span>Composition API</span>
</div>

<div class="logo">
  <img src="/logos/LogosVue.svg"/>
</div>

<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>4.000.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>35.7k</span>
  </div>
</div>

Dos estilos diferentes para generar componentes. Ambos obtienen el mismo resultado. Solo que con _Options API_ quedan templates largos y con la lógica dividida en más partes.



<a text-xs text-green-400 href="https://vuejs.org/guide/extras/composition-api-faq.html#what-is-composition-api">https://vuejs.org/guide/extras/composition-api-faq.html#what-is-composition-api</a>

<div class="grid grid-cols-2 w-full gap-9 mt-0">

<div>

<div class="flex justify-start items-center">
  <svg mr-3 xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24"><path fill="#fcbd12" d="M1 21L12 2l11 19H1Zm11-3q.425 0 .713-.288T13 17q0-.425-.288-.713T12 16q-.425 0-.713.288T11 17q0 .425.288.713T12 18Zm-1-3h2v-5h-2v5Z"/></svg>
  <p>Options API</p>
</div>

```vue {0|all|1-9|11-14|all}
<script>
export default {
  data() {
    return {
      message: 'Hello World!'
    }
  }
}
</script>

<template>
  <h1>{{ message }}</h1>
</template>
```
</div>

<div>

<div class="flex justify-start items-center">
  <svg mr-3 xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24"><path fill="#43b883" d="m10.6 16.2 7.05-7.05-1.4-1.4-5.65 5.65-2.85-2.85-1.4 1.4 4.25 4.25ZM5 21q-.825 0-1.413-.588T3 19V5q0-.825.588-1.413T5 3h14q.825 0 1.413.588T21 5v14q0 .825-.588 1.413T19 21H5Z"/></svg>
  <p>Composition API</p>
</div>

```vue {0|all|1-4|6-8|all}
<script setup>
import { ref } from 'vue'
const message = ref('Hello World!')
</script>

<template>
  <h1>{{ message }}</h1>
</template>
```

</div>

</div>

<!--
Si se quiere se pueden usar <br> ambos en un mismo template.



-->

---
title: Typescript
class: font-mono pt-0
layout: cover
---



<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Typescript</span>
</div>

<div class="logo">
  <img src="/logos/LogosTypescriptIcon.svg"/>
</div>

<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>38.000.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>89k</span>
  </div>
</div>

## Extraído de la documentación de Vue.

&#x2022;  Ayuda a detectar muchos errores comunes a través del <br>
análisis estático en el tiempo de compilación.

&#x2022; Esto reduce la posibilidad de errores de tiempo de <br>
ejecución en la producción.

&#x2022; Permite refactorizar con mayor confianza el código en <br>
aplicaciones a gran escala.

&#x2022; Mejora la experiencia de desarrollador a través de la <br>
completación automática basada en el tipo en IDE's.

---
class: 'font-mono pt-24'
layout: cover
title: VueUse
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>VueUse</span>
</div>

<div class="logo">
  <img src="/logos/LogosVueuse.svg"/>
</div>

<h3 mb-2>Colección de utilidades y componentes para extender Vue.</h3>

<img class="w-[750px] mr-auto" src="/vue-use.png"/>

<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>547.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>14.1k</span>
  </div>
</div>




---
class: 'font-mono pt-24'
layout: cover
title: VueUse
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>VueUse</span>
</div>

<div class="logo">
  <img src="/logos/LogosVueuse.svg"/>
</div>

<img  src="/vue-use-components.png"/>

<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>547.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>14.1k</span>
  </div>
</div>




---
class: 'font-mono pt-24'
title: Archivos de Configuración
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Archivos de Configuración</span>
</div>

<div class="logo">
  <img src="/logos/LogosVueConfig.svg"/>
</div>


### Archivos .config sirven para asistir al programador. 

- **Eslint** - Para encontrar y arreglar problemas en el código.
  - _tipo de javascript permitido (ES2021, ES2015)_
  - _estandarizar tipo de comillas a usar (comilla simple)_

- **Prettier** - Un formateador de codigo opinionado para mantener un estilo de codigo.
  - _ancho de lineas_
  - _un atributo por linea_
  
- **jsconfig/tsconfig**
  - Intellisense para los IDE con LSP (Language Server Protocol).
  - Permite configurar paths para importar componentes dentro del proyecto.



---
class: 'font-mono pt-24'
title: Vitest
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Vitest</span>
</div>

<div class="logo">
  <img src="/logos/LogosVitest.svg"/>
</div>


<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>1.369.562</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>8.3k</span>
  </div>
</div>

## Vitest

- El nuevo estandar (a pesar del nombre no requiere Vite pero si corre en NODE).

- Gracias al Hot Module Replacemente de Vite se puede testear componentes en tiempo real.

<img src="/vitest.gif"/>



---
class: 'font-mono pt-20'
title: Seguridad
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Seguridad</span>
</div>

<div class="logo">
  <img src="/logos/CarbonSecurity.svg"/>
</div>

 La regla general es que si permite que se ejecute contenido no “sanitizado” proporcionado por el usuario, podría exponerse a ataques.

<a class="text-green-500 mb-8 mt-2 text-xs" href="https://vuejs.org/guide/best-practices/security.html#best-practices">https://vuejs.org/guide/best-practices/security.html#best-practices</a>

- **HTML/JS/CSS** - injection

- **CSP** -  Content-Security Policy

- **noreferrer noopener** - indica al navegador que navegue sin otorgar acceso al nuevo contexto de navegación al no establecer la propiedad Window.opener en la ventana abierta (return 'null').

```vue {all|1-2|4-8}
 <!-- Eslint por ejemplo tira warning en esto -->
<a href="http://vuejs.com" target="_blank">link externo</a>

<!-- Correcto para ESLINT -->
<a href="http://vuejs.com" target="_blank" rel=”noreferrer noopener”>
  link 
</a>
```








---
class: 'font-mono pt-24'
laypot: center
title: Tailwind
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span> Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>TailwindCSS</span>
</div>

<div class="logo">
  <img src="/logos/LogosTailwindcssIcon.svg"/>
</div>


<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>5.490.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>65.6k</span>
  </div>
</div>

## TailwindCSS. Utilidades de CSS. 



<div class="mt-6">

- A diferencia de Bootstrap no trae componentes o interactividad de Javascript. 
- Ideal para Single File Components (SFC).
- Resetea todos los estilos. Un &lsaquo;h1&rsaquo; se ve igual que un &lsaquo;a&rsaquo; o un &lsaquo;p&rsaquo;. Esto permite intercambiar las class lo que acelera los ajustes visuales y la semántica.
- Elimina automaticamen el CSS que no se utiliza. Optimizacion al palo.
- Tailwind CSS IntelliSense para el IDE.
  
</div>


---
class: 'font-mono pt-24'
laypot: center
title: Tailwind
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span> Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>TailwindCSS</span>
</div>

<div class="logo">
  <img src="/logos/LogosTailwindcssIcon.svg"/>
</div>


<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>5.490.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>65.6k</span>
  </div>
</div>

## Utilidades de CSS. 

<div class="grid grid-cols-2 gap-6 mt-6">

<div>

- Cada estilo en CSS tiene una su clase en Tailwind.
- Hace más sencillo editar estilos a los desarrolladores.
- El estilo está en el componente. Editar estilos sin miedo a romper en otros sitios.
- Tambien se pueden establecer class que las agrupen.


</div>

<div class="pt-1">

<img rounded-lg bg-white p-3 shadow-lg src="/tailwind-css.png" />

</div>
</div>


---
class: 'font-mono pt-24'
title: Tailwind Demo
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>TailwindCSS</span>
</div>

<div class="logo">
  <img src="/logos/LogosTailwindcssIcon.svg"/>
</div>


<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>5.490.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>65.6k</span>
  </div>
</div>

## Utilidades de CSS en uso

<video autoplay loop muted playsinline class="mt-3" ><source src="/tailwind.mp4" type="video/mp4"></video>





---
class: 'font-mono pt-20'
title: HeadlessUI
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>HeadlessUI</span>
</div>

<div class="logo">
  <img src="/logos/LogosHeadlessuiIcon.svg"/>
</div>


<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM. (1.000.000 son de React)" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>1.290.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>19.3k</span>
  </div>
</div>

Componentes completamente accesibles, sin estilos, diseñados para integrarse con Tailwind CSS. **Para Vue y React**.

<img src="/headlessui.png" />






---
class: 'font-mono pt-20'
title: Componentes UI
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Componentes UI</span>
</div>

Agregan los componentes de Bootstrap que no tiene Tailwind.

PrimeVue y NaiveUI permiten importar solo el componente que se necesite.

Vuetify es muy bueno para iniciar rapidamente un proyecto pero resulta complejo adaptarlo a un diseño
porque hay que pisar todos los estilos o aprender a configurando.

<small class="text-green-400 relative -top-4">(recién esta lanzando su version para Vue3).</small>

<img src="/componentesui.png" class="relative -top-4"/>



---
class: 'font-mono pt-24'
title: Librerias UI
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Librerias UI</span>
</div>

<img src="/libreriasui.png" />


---
class: 'font-mono pt-6'
title: Librerias UI
layout: center
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Librerias UI</span>
</div>

<img src="/diagrama-css.png" class="w-160" />








---
class: 'font-mono pt-24 text-center'
title: Tanstack Table
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>DataTable</span>
</div>


<div class="logo">
  <img src="/logos/LogosTanstack.png"/>
</div>


<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>385.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>20.8k</span>
  </div>
</div>


## TanStack Table 🤩

Potencie sus tablas desde cero para TS/JS, React, Vue, Solid y Svelte
mientras se conserva el 100% de control sobre el HTML y CSS.


<img src="/tanstack.png" />




---
class: 'font-mono pt-24 text-center'
title: Tanstack Table
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>DataTable</span>
</div>


<div class="logo">
  <img src="/logos/LogosTanstack.png"/>
</div>


<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>385.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>20.8k</span>
  </div>
</div>


## TanStack Table 🤩

<img src="/tanstack-features.png" />






---
class: 'font-mono pt-24'
title: Graficos
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Gráficos</span>
</div>


<div class="logo">
  <img src="/logos/chartjs.svg"/>
</div>


<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>1.692.338</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>60k</span>
  </div>
</div>


## Para hacer gráficos.

Actualmente lo usamos para webs en wordpress. Cuenta con <a href="https://github.com/chartjs/awesome">su propio ecosistema de plugins</a> para extender y con una libreria especifica para Vue (vue-charts).

<div class="max-w-6xl flex justify-center items-center mx-auto bg-white p-2 rounded shadow-lg h-80">
  <BarChart/>
</div>



---
class: 'font-mono pt-20'
title: Validar Forms
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Validar Formularios</span>
</div>




## Validación de formularios

Hay dos escuelas de pensamiento en lo que respecta a la validación de formularios, el enfoque declarativo (vee-validate) y el imperativo (vuelidate). Eso significa que no existe una solución definitiva que se adapte a todos. Depende en gran medida de su aplicación.

<img src="/vuevalidate-vs-veevalidate.png"  />


<a class="text-xs text-green-400 fixed top-8 right-16" href="https://www.reddit.com/r/vuejs/comments/emcsoa/veevalidate_vs_vuelidate/">veevalidate_vs_vuelidate</a>






---
class: 'font-mono pt-20'
title: VeeValidate vs Vuelidate
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>VeeValidate vs Vuelidate</span>
</div>

<div class="grid grid-cols-2">

<div class="text-center">

<img src="/logos/LogosVeevalidate.png" class="w-32 mx-auto"/>

## VeeValidate

valida Inputs



<div class="flex justify-center items-center space-x-3">

<div data-text="Descargas semanales en NPM" class="tooltip flex items-center">
<img src="/logos/MaterialSymbolsDownloadRounded.svg" class="h-6 w-6 mr-2"/>
<span text-gray-100>426.000</span>
</div>
<div data-text="Github Stars" class="tooltip flex items-center">
<img src="/logos/MaterialSymbolsStar.svg" class="h-6 w-6 mr-2"/>
<span text-gray-100>9k</span>
</div>

</div>

<img src="/vee-validate-features.jpg" class="mt-12" />

</div>

<div class="text-center">

<img src="/logos/LogosVuevalidate.png"  class="w-32 mx-auto"/>

## Vuelidate

valida valores

<div class="flex justify-center items-center space-x-3">

  <div data-text="Descargas semanales en NPM" class="tooltip flex items-center">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg" class="h-6 w-6 mr-2"/>
    <span text-gray-100>297.000</span>
  </div>
  <div data-text="Github Stars" class="tooltip flex items-center">
    <img src="/logos/MaterialSymbolsStar.svg" class="h-6 w-6 mr-2"/>
    <span text-gray-100>6.6k</span>
  </div>

</div>

<div>

</div>


</div>


</div>


---
class: 'font-mono pt-12'
layout: center
title: WYSIWYG
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Editores de texto enriquecido.</span>
</div>

<img src="/wys.png" class="w-[80%] mx-auto" />

<br>

<p text-center> Quill requiere mas desarrollo para obtener lo mismo que CKEditor.</p>
<p text-center> Es la "mejor" alternativa para los desarrolladores a CKEditor.</p>



---
class: 'font-mono pt-24'
layout: cover
title: Unplugin Icons
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Unplugin Icons</span>
</div>

<div class="logo">
  <img src="/logos/Logounpluginicons-icones.svg"/>
</div>

## Libreria de libreria de iconos.


<div class="grid grid-cols-2 gap-6 mt-12">

<div>

- **Cualquier conjunto de íconos** <br> más de
100 conjuntos populares con más de
10,000 íconos, logotipos, emojis, etc.
Desarrollado por Iconify.

- **Estilizable** <br> cambie el tamaño, el
color o incluso agregue animaciones
usando estilos y clases.

</div>

<div class="pt-4">

```vue
<script setup>
  import IconAccessibility from '~icons/carbon/accessibility'
  import IconAccountBox from '~icons/mdi/account-box'
</script>

<template>
  <icon-accessibility/>
  <icon-account-box style="font-size: 2em; color: red"/>
</template>
```

</div>
</div>


<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>32.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>2.4k</span>
  </div>
</div>



---
title: fuse.js
class: 'font-mono pt-24'
layout: cover
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Fuse.js</span>
</div>


<div class="logo">
  <img src="/logos/LogosFusejs.png"/>
</div>


<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>2.712.073</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>15.5k</span>
  </div>
</div>


## Fuse.js

Fuzzy searching (approximate string matching) es la técnica para encontrar strings que son aproximadamente iguales a un patron. (en lugar de exactamente).

<Fuse/>


---
class: 'font-mono pt-24'
title: Nuxt
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Vue</span>
  <img src="/logos/chevron.svg"/>
  <span>Nuxt.js (metaframework)</span>
</div>


<div class="logo">
  <img src="/logos/LogosNuxtIcon.svg"/>
</div>


<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>500.858</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>4.4k</span>
  </div>
</div>

## Nuxt.js

<br>

- Es Vue de base pero orientado a renderizar en el servidor.
- Mejor SEO
- Extiende con todo un ecosistema.
- Mejora la carga inicial, ideal para sitios estaticos.
- Router viene incluido. En vue hay que instalar vue-router.
- Autoimports de componentes

<img src="/nuxt.png" class="mx-auto w-[500px] mt-12" />

<style>

li {
  @apply text-sm
}

.slidev-page  {
  background: #0c0c0c;
}

</style>


---
class: 'font-mono pt-24'
title: Markdown
---

<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Markdown</span>
</div>


<div class="logo">
  <img src="/logos/LogosMarkdown.svg"/>
</div>

# Markdown

- Ideal para documentar.
- Lenguaje que usa Gitlab en comentarios y readme.md
- Usando YAML Frontmatter se pueden pasar parametros.


<div class="grid grid-cols-2 gap-6">

<div>

```md

---
title: Introduction
description: Learn how to use @nuxt/content.
---

```



</div>

<div>


```json
{
  body: Object
  excerpt: Object
  title: "Introduction"
  description: "Learn how to use @nuxt/content."
  dir: "/"
  extension: ".md"
  path: "/index"
  slug: "index"
  toc: Array
  createdAt: DateTime
  updatedAt: DateTime
}
```


</div>

</div>







---
title: Astro
class: font-mono pt-24
---



<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Astro</span>
</div>

<div class="logo top-3">
  <img src="/logos/LogosAstro.svg"/>
</div>

<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>69.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>27.8k</span>
  </div>
</div>

## Cero javascript por defecto en el frontend.

- Es un Multi-Page Application (MPA) que usa javascript como lenguaje de servidor y runtime.

- Viene con todo para crear un sitio. (component syntax, file-based routing, asset handling, build process, bundling, optimizations, data-fetching).

- Se puede extender usando componentes de React, Vue, Solid, Svelte.




---
title: Alpine
class: font-mono pt-24
---



<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Alpine.js</span>
</div>

<div class="logo ">
  <img src="/logos/LogosAlpinejsIcon.svg"/>
</div>

<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>135.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>23.2k</span>
  </div>
</div>

## Alternativa a Jquery

- Mucho de lo que Vue ofrece para agregar
comportamientos e interacciones a una web
con muy poco peso.

- Reemplaza jQuery para pequeños sitios

- Usar en el modo apto para CSP <a href="https://alpinejs.dev/advanced/csp">(Content-Security Policy)</a>

<div class="grid grid-cols-2 gap-6">

<div>

Alpine

```html
<script src="//unpkg.com/alpinejs" defer ></script>
 
<div x-data="{ open: false }">
    <button @click="open = true">Expand</button>
 
    <span x-show="open">
      Content...
    </span>
</div>
```

</div>


<div>

Vue

```vue
<button @click="isOpen = !isOpen">Expand</button>
<span v-show="isOpen">
  Content...
</span>

<script setup>
  import { ref } from 'vue'
  const isOpen = ref(true)
</script>
```

</div>

</div>


---
title: Alpine
class: font-mono pt-24
---



<div class="breadcrumb">
  <span text-gray-100> Javascript</span>
  <img src="/logos/chevron.svg"/>
  <span>Alpine.js</span>
</div>

<div class="logo ">
  <img src="/logos/LogosAlpinejsIcon.svg"/>
</div>

<div class="stars-downloads">
  <div data-text="Descargas semanales en NPM" class="tooltip">
    <img src="/logos/MaterialSymbolsDownloadRounded.svg"/>
    <span text-gray-100>135.000</span>
  </div>
  <div  data-text="Github Stars" class="tooltip">
    <img src="/logos/MaterialSymbolsStar.svg"/>
    <span text-gray-100>23.2k</span>
  </div>
</div>


## Alternativa a Jquery

- Usar en el modo apto para CSP <a href="https://alpinejs.dev/advanced/csp">(Content-Security Policy)</a>

<div class="grid grid-cols-1 gap-6">

<div>

```html
<!-- Mal -->
<div x-data="{ count: 1 }">
    <button @click="count++">Increment</button>
    <span x-text="count"></span>
</div>
```

</div>


<div>

```html
<!-- Bien -->
<div x-data="counter">
    <button @click="increment">Increment</button>
    <span x-text="count"></span>
</div>

<script>
  Alpine.data('counter', () => ({
      count: 1,
      increment() { this.count++ }
  }))
</script>
```

</div>

</div>
