---
layout: post
title: "Formularios en DSpace Angular: Configuración, curaduría y mejores prácticas para la visibilidad global"
subtitle: "Calidad de metadatos desde el origen: Optimizando los procesos de depósito en DSpace Angular"
date: 2026-10-01 10:00:00 -0600
categories: [capacitacion, soporte]
tags: [dspace, dspace-angular, formularios, metadatos, oai-pmh, curaduria, open-hours, la-referencia, lyrasis]
author: "Arturo Garduño Magaña"
---

El pasado **30 de septiembre**, el proyecto colaborativo **LA Referencia – Lyrasis** llevó a cabo su sesión mensual de Open Hour dedicada al diseño, administración y mejores prácticas en los formularios de envío (*submission*) y edición en las versiones modernas de DSpace (Angular 7.x, 8.x, 9.x y la próxima versión 10.x).

La sesión contó con la participación de **Luciana Mara Silva** (Lead de Documentación) y **Jesiel Viana** (Lead de Desarrollo), quienes abordaron el tema combinando la visión estratégica de curaduría de contenidos con la configuración técnica a nivel de servidor y las innovaciones funcionales que llegan con las nuevas versiones del software.

## Temas Clave Abordados en la Sesión

A lo largo del encuentro se analizaron los puntos críticos para asegurar la calidad de la información y la autonomía técnica en la gestión de repositorios:

### 1. Visibilidad global e interoperabilidad regional
Se destacó que la estandarización de metadatos en los formularios de depósito no es un mero requisito administrativo, sino el motor fundamental que alimenta correctamente el protocolo **OAI-PMH**. Una captura consistente y normalizada desde el origen garantiza una indexación eficiente y maximiza la presencia e impacto de la producción científica en motores de búsqueda, cosechadores globales como **Google Scholar** y las redes nacionales de agregación.

### 2. Estrategias de curaduría: Adiós a los formularios genéricos
Uno de los puntos centrales del encuentro fue la recomendación de abandonar el esquema de un único formulario genérico para toda la institución. Diseñar formularios específicos por tipología documental (tesis de grado/TCC, disertaciones, artículos de revistas, capítulos o libros electrónicos) reduce drásticamente las omisiones por parte de los autores y optimiza los flujos de trabajo de los equipos bibliotecarios al disminuir la carga de curaduría posterior.

### 3. Arquitectura e implementación técnica
En la sección técnica se examinó a profundidad el funcionamiento y la interacción entre los dos archivos XML fundamentales del backend de DSpace:
- `submission-forms.xml`: Define los campos, etiquetas de interfaz, vocabularios controlados, validaciones y atributos obligatorios u opcionales.
- `item-submission.xml`: Estructura los pasos lógicos del flujo de depósito y asocia los formularios correspondientes con sus colecciones específicas.

### 4. Novedades en DSpace 10: Gestión desde la interfaz gráfica (UI)
Se presentaron los avances que incorporará DSpace 10, destacando la capacidad de vincular y gestionar formularios directamente con las colecciones desde la interfaz gráfica de administración. Esta evolución representa un salto significativo en la autonomía de los gestores de repositorios, reduciendo la dependencia de intervenciones directas en la consola o la edición manual de archivos en el servidor.

### 5. Recursos de integración y soporte para la comunidad
Se compartieron recursos orientados a integraciones especializadas, como el esquema y repositorio de metadatos de la **CAPES** para articular repositorios con la plataforma Sucupira en Brasil, y se recordó la disponibilidad de los canales de asistencia técnica gratuita que el proyecto LA Referencia – Lyrasis brinda a toda la región.

## Grabaciones y Materiales Disponibles

Ponemos a disposición de la comunidad las grabaciones bilingües y las diapositivas oficiales de la presentación:

- 🎥 **Grabación en Español (Interpretación):** [Ver en YouTube](https://youtu.be/7ZbMGVDdVA0)
- 🎥 **Gravação em Português (Original):** [Assistir no YouTube](https://youtu.be/IOpTPpXrCjE)
- 📑 **Diapositivas de la sesión:** [Descargar en el Repositorio del Proyecto](https://dspace-prd.lareferencia.info/handle/123456789/275)

## Soporte y Comunidad Técnica

Si tu institución requiere orientación para reestructurar sus formularios de depósito, resolver inconsistencias de interoperabilidad o planificar la migración hacia DSpace 8 o 9, recuerda que puedes apoyarte en nuestros canales abiertos:

- 🛠️ **Sitio de Soporte Técnico:** [Portal de Soporte DSpace LA Referencia](https://soporte-dspace.lareferencia.info/es/home) (atención y seguimiento estandarizado mediante GitHub Issues con SLA de respuesta).
- 💬 **Servidor de Discord:** Únete a la conversación en nuestro [servidor de Discord](https://discord.com/invite/GQzvHREzNy) para interactuar con colegas, resolver consultas técnicas cotidianas y enterarte de los próximos eventos y cursos.
- 🌐 **Portal del Proyecto:** Explora recursos, documentación viva y novedades en el [Portal DSpace LA Referencia](https://dspace.lareferencia.info/).

**Autor:** Arturo Garduño Magaña  
**Coordinador del Proyecto LA Referencia – Lyrasis**
