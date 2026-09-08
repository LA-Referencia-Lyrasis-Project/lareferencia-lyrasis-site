---
layout: post
title: "Optimización, seguridad y rendimiento en DSpace: Estrategias frente al tráfico masivo de bots e IA"
subtitle: "Enfrentando los nuevos desafíos de infraestructura en repositorios institucionales"
date: 2026-08-14 10:00:00 -0600
categories: [infraestructura, seguridad]
tags: [dspace, rendimiento, seguridad, crawlers-ia, anubis-waf, angular-ssr, la-referencia, lyrasis, open-hours]
author: "Arturo Garduño Magaña"
---

En los últimos años, los repositorios institucionales han experimentado un incremento exponencial en consultas automatizadas originadas por herramientas de minería de datos, indexadores y rastreadores (*crawlers*) de inteligencia artificial. Esta actividad genera sobrecargas imprevistas que ponen en riesgo la estabilidad, disponibilidad y rendimiento de plataformas como DSpace.

Para analizar este escenario crítico y compartir soluciones prácticas basadas en experiencias reales, el proyecto **LA Referencia – Lyrasis** dedicó la sesión de la **Open Hour de Agosto 2026** al tema: *“Optimización, seguridad y buenas prácticas para la mejora de rendimiento en repositorios”*.

## Experiencias desde la práctica: Los ponentes

El encuentro reunió la perspectiva técnica de dos especialistas de amplia trayectoria en la región:

- **Agustín Alfieri** (Universidad Nacional de Rosario / LA Referencia): Especialista en administración de plataformas de ciencia abierta, gestión integral de DSpace, interoperabilidad mediante OAI-PMH e implementación de identificadores persistentes.
- **Gerardo Flores** (CIMMYT / LA Referencia): Especialista en entornos Linux, mantenimiento de repositorios de datos científicos, automatización de flujos e infraestructura sustentada en tecnologías de código abierto.

## Puntos clave y estrategias compartidas

A partir del análisis de incidentes de saturación y pruebas de estrés en servidores de producción, los ponentes desglosaron los principales retos de infraestructura y las líneas de acción recomendadas:

### 1. El impacto del tráfico agresivo en DSpace
Agustín Alfieri expuso el caso de la Universidad Nacional de Rosario (UNR), donde ráfagas masivas y concurrentes de peticiones automatizadas provocaron la saturación de memoria RAM al 100%, derivando en lentitud extrema e interrupciones del servicio. En instancias sobre DSpace 7.6.x, las ineficiencias en el renderizado del frontend desacoplado (Angular con Server-Side Rendering - SSR) agravaron la situación al procesar y reconstruir páginas completas en cada solicitud sin contar con una capa intermedia de caché optimizada para este perfil de tráfico.

### 2. Límites de las medidas paliativas
Los métodos tradicionales de contención demostraron claras restricciones estructurales:
- **Bloqueo manual de IPs:** Resultó ineficaz frente a redes dinámicas, residenciales y distribuidas globalmente.
- **Bloqueo geográfico estricto:** Aunque se evaluó como medida de emergencia preservando únicamente servicios como Handle y Google Scholar, restringe el acceso universal y contradice el principio de acceso abierto que fundamenta a los repositorios institucionales.
- **Escalamiento vertical de hardware:** Incrementar CPU y RAM de forma indefinida supone costos económicos insostenibles a mediano y largo plazo sin resolver el cuello de botella de fondo.

### 3. Soluciones estructurales y actualización de versiones
Se enfatizó la necesidad estratégica de migrar hacia versiones modernas de la plataforma (DSpace 8 y DSpace 9). Estas versiones integran optimizaciones sustanciales en el motor de renderizado de Angular SSR, mejoras en el pipeline de entrega de assets y esquemas de caché más eficientes diseñados para amortiguar impactos masivos sobre el backend y la base de datos.

### 4. Filtrado activo y WAF con Anubis
Gerardo Flores presentó en detalle la arquitectura e integración de **Anubis**, un cortafuegos para aplicaciones web (*Web Application Firewall* o WAF) de código abierto diseñado para identificar y mitigar tráfico abusivo. Mediante inspección de comportamiento, heurísticas avanzadas y desafíos automáticos basados en prueba de trabajo (*proof-of-work*), Anubis neutraliza bots no deseados en la capa perimetral antes de que sus peticiones consuman memoria y procesamiento en el servidor de aplicaciones de DSpace.

### 5. Enfoque de defensa integral
La sesión concluyó destacando que la resiliencia de un repositorio requiere un equilibrio coordinado:
- Mantener la plataforma actualizada hacia las ramas con soporte activo.
- Optimizar la configuración de Nginx, Node.js y Tomcat.
- Implementar mecanismos perimetrales de filtrado y validación de tráfico sin sacrificar la indexación legítima ni el acceso global.

## Grabación completa de la sesión

La sesión completa, con los análisis técnicos y la ronda de preguntas y respuestas, se encuentra disponible para consulta libre:

- 🎥 **Grabación en video:** [Ver sesión completa en YouTube](https://www.youtube.com/watch?v=DrrUjHySFxQ)

## Canales de consulta y acompañamiento técnico

El equipo del proyecto mantiene abiertos sus espacios de colaboración para asesorar a las instituciones de América Latina que enfrenten retos de saturación, rendimiento o migración:

- 🛠️ **Portal de Soporte Técnico:** Solicita asistencia técnica y diagnósticos en el [Portal de Soporte DSpace LA Referencia](https://soporte-dspace.lareferencia.info/es/home).
- 💬 **Comunidad en Discord:** Conéctate con colegas y el equipo del proyecto en nuestro [Servidor de Discord](https://discord.com/invite/GQzvHREzNy).
- 🌐 **Recursos y canales institucionales:** Consulta todas nuestras iniciativas en [Enlaces de LA Referencia](https://linktr.ee/LA_Referencia).

<br>

**Autor:** Arturo Garduño Magaña  
**Coordinador del Proyecto LA Referencia – Lyrasis**
