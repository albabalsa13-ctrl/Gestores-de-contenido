## ¿Qué es un SSG y cómo funciona?

Un generador de sitios estáticos (SSG) es una herramienta que compila código y contenido en local o en un servidor de integración para generar una web compuesta únicamente por archivos planos (HTML, CSS y JavaScript) listos para servir. Utiliza como punto de partida archivos de texto ligero (habitualmente Markdown o MDX con metadatos en YAML/TOML) y los procesa a través de plantillas y motores de compilación (build pipeline), generando todo el HTML final antes de que cualquier usuario visite la página. Gracias a esto, el servidor no necesita ejecutar consultas a bases de datos ni interpretar código en tiempo real, lo que ofrece máxima velocidad de carga, alta seguridad y costes mínimos de alojamiento, a cambio de requerir recompilaciones completas ante cada cambio y exigir conocimientos técnicos de consola y Git.  
![Imagen](SSG.jpg)

## Ventajas SSG frente al HTML
Usar un SSG hace que no tengas que escribir HTML desde cero para cada página, tiene plantillas y componentes reutilizables, por lo que la creación de webs es mas automática y optimizada. Agiliza mucho la carga de trabajo.

## Comparación de generadores estáticos

| Aspecto que investigar | Jekyll | Hugo | Astro |
| --- | --- | --- | --- |
| **Tecnología o lenguaje principal** | Ruby | Go | JavaScript / TypeScript |
| **Formato utilizado para el contenido** | Markdown (.md) con metadatos en YAML. | Markdown (.md) con metadatos en TOML, YAML o JSON. | Markdown (.md), MDX (.mdx), HTML o componentes propios. |
| **Necesidad de instalación** | Requiere el entorno Ruby y su gestor de gemas (Bundler). | Solo requiere descargar un binario ejecutable único. | Requiere entorno Node.js y gestor de paquetes (npm, pnpm o yarn). |
| **Funcionamiento básico** | Lee archivos y plantillas Liquid para compilar el HTML. | Motor Go ultrarrápido que procesa y vuelca el sitio en milisegundos. | Usa "Islas de Arquitectura": envía HTML puro y solo hidrata componentes interactivos. |
| **Usos habituales** | Blogs personales y páginas de proyectos en GitHub Pages. | Sitios grandes, portales de documentación y blogs con miles de páginas. | Portafolios, landing pages y webs modernas con React, Vue o Svelte. |
| **Ventajas** | Integración nativa con GitHub Pages y sintaxis simple. | Velocidad de compilación casi instantánea y sin dependencias externas. | Carga cero JavaScript por defecto y permite mezclar múltiples frameworks. |
| **Inconvenientes** | Compilación lenta en proyectos grandes y dependencias pesadas de Ruby. | Curva de aprendizaje empinada para dominar las plantillas de Go. | Mayor complejidad técnica inicial al depender del ecosistema npm. |
| **Posibilidad de publicarlo en GitHub Pages** | Sí, de forma nativa con solo hacer `push`. | Sí, mediante un flujo automatizado de CI/CD (GitHub Actions). | Sí, configurando un flujo de trabajo con GitHub Actions. |

---
👉 [Ver vídeo explicativo sobre SSG](https://www.youtube.com/watch?v=osWfEtbP_sk)  
👉 [Ir a la investigación sobre CMS](cms.md)
