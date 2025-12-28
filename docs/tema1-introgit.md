# Tema 1: Introducción a Git y el Control de Versiones

## 1. ¿Qué es el Control de Versiones?
Imagina que estás escribiendo un trabajo y guardas archivos como `trabajo_v1.doc`, `trabajo_final.doc`, `trabajo_final_final.doc`. Esto es ineficiente y peligroso.

**Git** es un sistema de control de versiones que registra cada cambio realizado en un proyecto. Permite:
* **Viajar en el tiempo:** Puedes volver a cualquier versión anterior de tus apuntes o código.
* **Ramificar (Branching):** Puedes probar ideas nuevas sin romper el trabajo principal.
* **Colaborar:** Varias personas pueden trabajar en el mismo archivo sin pisarse el trabajo.

## 2. El Flujo de Trabajo Profesional
En la industria tecnológica, no simplemente "guardamos" archivos. Seguimos un ciclo lógico que garantiza la integridad de la información:

```mermaid
graph LR
    A[Modificar Archivo] --> B[Stage: Preparar cambio]
    B --> C[Commit: Registrar en la historia]
    C --> D[Push: Subir a la nube / GitHub]
