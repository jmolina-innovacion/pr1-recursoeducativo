---
layout: default
title: Tema 1 - Introducción a Git
---
# Tema 1: Introducción a Git y el Control de Versiones

## 1. ¿Qué es el Control de Versiones?
Imagina que estás escribiendo un trabajo y guardas archivos como `trabajo_v1.doc`, `trabajo_final.doc`, `trabajo_final_borrador.doc`. Esto es ineficiente y peligroso.

**Git** es un sistema de control de versiones distribuido que registra cada cambio realizado en un proyecto. Permite:
* **Viajar en el tiempo:** Volver a cualquier versión anterior.
* **Ramificar (Branching):** Probar ideas nuevas sin romper el trabajo principal.
* **Colaborar:** Trabajar en equipo sin conflictos.

## 2. Instalación y Configuración
Antes de empezar, necesitas instalar Git y decirle quién eres.

### Configuración de Identidad
Es crucial configurar tu nombre y correo, ya que aparecerán en cada commit que hagas.
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```

## 3. Operaciones Básicas
Comandos esenciales para empezar y trabajar:

1. **`git init`**: Inicializa un repositorio nuevo en la carpeta actual.
2. **`git clone <url>`**: Descarga un proyecto y todo su historial de versiones.
3. **`git add <archivo>`**: Pasa cambios al área de preparación (staging).
4. **`git commit -m "mensaje"`**: Guarda los cambios preparados en el historial.
5. **`git status`**: Muestra el estado de los archivos (modificados, preparados, etc.).

## 4. Operaciones Avanzadas

### Ramas y Fusiones
* **`git branch <nombre>`**: Crea una nueva rama.
* **`git checkout <nombre>`** (o `git switch`): Cambia de rama.
* **`git merge <rama>`**: Fusiona los cambios de una rama en la actual.

### Deshacer Cambios
* **`git revert <commit-id>`**: Crea un *nuevo* commit que deshace los cambios de uno anterior (seguro para historial público).
* **`git reset`**: Mueve el puntero a un estado anterior (peligroso en repos compartidos).

### Tags (Etiquetas)
Se usan para marcar puntos específicos en la historia como importantes (v1.0, v2.0).
```bash
git tag -a v1.0 -m "Versión 1.0 lista"
```

## 5. Historia y Trazabilidad
El historial no solo guarda código, cuenta una historia.
* **`git log`**: Muestra el historial de commits.
* **`git log --oneline --graph`**: Muestra el historial simplificado y gráfico.

## 6. Seguridad en Repositorios
Proteger tu código es vital.

### Autenticación SSH
En lugar de contraseñas, usa llaves SSH para conectar con GitHub/GitLab de forma segura.
1. Generar par de claves: `ssh-keygen -t ed25519 -C "tu@email.com"`
2. Añadir clave pública a GitHub (Settings > SSH Keys).

### Buenas Prácticas
* **.gitignore**: Nunca subas contraseñas, claves API, o carpetas de dependencias (`node_modules`, `venv`). Crea siempre un archivo `.gitignore`.
* **Control de Accesos**: En repositorios de organización, asigna roles (Read, Write, Admin) según necesidad.
* **Firmado de Commits**: Usa GPG para firmar criptográficamente tus commits y verificar tu identidad.
