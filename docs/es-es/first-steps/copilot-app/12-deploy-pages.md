---
title: "Lección 12 - Publica el sitio con GitHub Pages"
description: "Usa la aplicación GitHub Copilot para configurar un flujo de trabajo de Pages, revisar su solicitud de incorporación de cambios y comprobar que Space Quiz está disponible."
authors:
  - jamesmontemagno
lastUpdated: 2026-10-12
---

Publica Space Quiz con GitHub Pages para que todo el mundo pueda probarlo. Copilot puede preparar el flujo de trabajo y guiarte durante la implementación, pero tú debes revisar los cambios y confirmar que el sitio está disponible.

En esta lección vas a:

- pedir a Copilot que configure una implementación en GitHub Pages.
- revisar el flujo de trabajo y la solicitud de incorporación de cambios antes de fusionarla.
- seguir la implementación y comprobar el sitio publicado.

## Escenario

Space Quiz ya está en un repositorio de GitHub, pero todavía hace falta una forma sencilla de probarlo. Publicar el sitio de un solo archivo con GitHub Pages lo pone a disposición en una URL pública sin añadir un servidor ni dependencias de ejecución.

## Pide a Copilot que publique el sitio

En la sesión de la aplicación Copilot para `space-quiz`, envía este prompt:

```plaintext
Habilita GitHub Pages para este repositorio. Crea un flujo de trabajo de GitHub Actions que compile el sitio web si es necesario y lo publique en GitHub Pages. Añade un README que describa la aplicación y cómo ejecutarla localmente, si aún no existe. Crea una solicitud de incorporación de cambios con estos cambios y fusiónala cuando se superen las comprobaciones obligatorias. Supervisa la implementación hasta que finalice correctamente y, después, indica la URL final del sitio publicado. Si no tienes permiso para habilitar Pages o fusionar la solicitud, dime exactamente qué debo aprobar o hacer; no informes de que se ha completado hasta que el sitio esté disponible.
```

![Diagrama de tres etapas: una solicitud de incorporación de cambios de space-quiz fusionada; una ejecución correcta de GitHub Actions para implementar el sitio, con los pasos Build website, Upload artifact y Deploy to Pages; y Space Quiz publicado en yourname.github.io/space-quiz/.](../../../_images/first-steps-app-pages-deploy.svg)

> [!WARNING]
> Este prompt pide al agente que cree y fusione una solicitud de incorporación de cambios y que cambie la configuración de Pages del repositorio. Revisa la diferencia, los permisos de implementación y cualquier solicitud de aprobación de GitHub antes de continuar.

## Revisa el flujo de trabajo y comprueba la implementación

1. Confirma que el README solo se añade si el repositorio aún no tiene uno.
2. Revisa los cambios de la solicitud de incorporación de cambios, incluidos los pasos de compilación e implementación del flujo de trabajo.
3. Fusiónala solo cuando se superen las comprobaciones obligatorias.
4. Sigue la ejecución de implementación de GitHub Actions hasta que finalice correctamente.
5. Abre la URL indicada y confirma que se carga Space Quiz.

Si el agente no puede habilitar Pages o fusionar la solicitud de incorporación de cambios, sigue las instrucciones concretas que te proporcione. No des la tarea por terminada hasta que la implementación finalice correctamente y se cargue el sitio.

## Resumen y siguientes pasos

Space Quiz ya está disponible como sitio público y has comprobado la implementación en lugar de confiar solo en el informe del agente. Continúa con la [lección 13: Repaso y próximos pasos][next-lesson].

[next-lesson]: ../13-review/
