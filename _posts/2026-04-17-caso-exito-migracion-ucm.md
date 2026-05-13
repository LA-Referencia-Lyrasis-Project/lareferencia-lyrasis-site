---
layout: post
title: "Caso de Éxito de Migración DSpace (2026) – Universidad Católica del Maule, Chile"
subtitle: "Cómo la UCM unificó dos repositorios y migró exitosamente a DSpace 8.1"
date: 2026-04-17
categories: [casos-de-exito]
---

Como parte del Pilar III (Comunidad y Capacitación) del proyecto conjunto entre LA Referencia y Lyrasis, hemos iniciado una serie de entrevistas destinadas a documentar y compartir las experiencias de instituciones que han liderado la transición hacia versiones modernas de DSpace (7.x, 8.x y 9.x) en nuestra región.

El objetivo central de esta iniciativa es transformar los desafíos técnicos y las decisiones estratégicas de cada institución en un recurso de aprendizaje colectivo que permita reducir la brecha tecnológica mediante el intercambio de lecciones aprendidas.

En esta entrega, destacamos la experiencia de la **Universidad Católica del Maule (Chile)**, quienes han completado con éxito un proceso de unificación y actualización tecnológica hacia DSpace 8.1, fortaleciendo así la visibilidad de su producción científica institucional.

## I. Información General y Responsables

Para comenzar con el caso de éxito, la Universidad Católica del Maule (Chile) nos comparte los detalles de quiénes estuvieron al frente de este proceso. El liderazgo técnico y la ejecución de la migración estuvieron a cargo de **Javier Caro Aguilera** (jcaro@ucm.cl) y **Fabián Arellano Calderón** (farellanoc@ucm.cl). El repositorio institucional en producción ya se encuentra disponible para consulta pública en: [repositorioinstitucional.ucm.cl](https://repositorioinstitucional.ucm.cl)

## II. Perfil Tecnológico de la Migración

Uno de los aspectos más interesantes de este caso es el salto tecnológico realizado. Al consultarles sobre las versiones de partida y de destino, el equipo nos explicó:

> «Se unificaron dos repositorios en sus versiones 5.6 de DSpace y 7.1 de DSpace Cris a la versión 8.1 de DSpace».

Respecto a la arquitectura de despliegue seleccionada para soportar esta nueva infraestructura, señalaron el uso de una:

> «Instalación manual, con servidor virtualizado QEMU Virtual CPU versión 2.5+ 4 CPU(s), 12GB RAM, 100GB SSD, Ubuntu 24.04.2 LTS».

Un punto fundamental para el proyecto es saber si los recursos generados son de utilidad. Al preguntarles si utilizaron la documentación oficial traducida por el proyecto (en una escala del 1 al 5), la respuesta fue contundente:

> «Escala 5: la documentación sirvió de guía durante todo el proceso de instalación y migración».

## III. Desafíos y Soluciones

La gestión de los datos suele ser el mayor reto. Al pedirles que describieran sus procesos de limpieza de metadatos o base de datos, detallaron su estrategia de «instalación limpia»:

> «Nuestra migración, constó en realizar la instalación limpia de la versión 8.1 de DSpace y cosechar los metadatos de ambos repositorios con el fin de unificar ambos (DSpace 5.6 y DSpace Cris 7.1) en la última versión instalada. Luego se llevó a cabo una limpieza de metadatos de la cosecha en Dspace 8.1».

Sobre la Interfaz de Usuario (UI) y la complejidad del paso de JSPUI/XMLUI al nuevo frontend en Angular, así como el nivel de personalización, comentaron:

> «La personalización de las diferentes plantillas fue el proceso más complejo, debido a que fue una experiencia nueva para nosotros, teniendo que identificar la ubicación de las diferentes plantillas a editar. La personalización fue completamente en Dspace 8.1, no hubo migración de las versiones anteriores y se realizaron cambios orientados a dar identidad al sitio, utilizando el formato institucional. Los cambios afectaron la personalización de los colores, la plantilla de inicio, la plantilla del ítem y colecciones».

En cuanto a la visualización de estadísticas en la nueva versión, el equipo aclaró la situación actual de sus reportes:

> «Al ser una instalación limpia lamentablemente las estadísticas se pierden, pero mantenemos los reportes correspondientes de los repositorios anteriores y la evidencia correspondiente».

## IV. Interacción con el Proyecto

La colaboración con la comunidad es un pilar estratégico. Al preguntarles sobre el soporte técnico y si abrieron tickets o participaron en los ciclos de intervención de LA Referencia-Lyrasis, destacaron:

> «Sí, se abrió ticket y también se participó en los ciclos de intervención, además compartimos con la comunidad de Discord. Nos pareció una grata experiencia poder contar con ayuda de un soporte especializado, como también el haber participado en el ciclo cerrado donde compartimos nuestra experiencia con diferentes universidades de la región».

Sobre la capacitación y su asistencia a las Open Hours, mencionaron:

> «Se participó como oyente en la mayoría de las Open Hours dedicadas a la migración de Dspace y también contando nuestra experiencia en la Sexta Open Hour».

## V. Lecciones Aprendidas y Próximos Pasos

Finalmente, pedimos un consejo para otras instituciones que estén por iniciar su migración, a lo que respondieron:

> «Antes de iniciar el cambio tome en cuenta la posibilidad de migrar a la versión más actualizada y estable disponible, además ver si hará la migración traspasando la base de datos o utilizará cosecha, observando los pros y los contras. Además, creemos super importante y útil contar con una versión de pruebas, antes de pasar algún cambio a producción».

Mirando hacia el futuro, sus próximos pasos incluyen funcionalidades avanzadas:

> «Nuestro próximo paso será actualizar a la versión 9 más estable con el fin de incorporar mejoras sustantivas en seguridad y experiencia de usuario, alineándonos al desarrollo de la versión, además planeamos robustecer los metadatos existentes, lo cual nos ayudará a incrementar el valor estratégico y comunicacional de la información científica».
