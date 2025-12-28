---
layout: default
title: Tema 2 - Documentación Técnica y Markdown
---
# Tema 2: Herramientas para la Generación de Documentación Técnica

La documentación es una parte fundamental del desarrollo de software. No solo explica cómo funciona el código, sino que garantiza su mantenibilidad y usabilidad por parte de otros (o de tu "yo" del futuro).

## 1. Markdown: El Estándar de Facto
Markdown es un lenguaje de marcado ligero que permite dar formato a textos planos de manera sencilla y legible. Es la herramienta principal en plataformas como GitHub, GitLab y StackOverflow.

### 1.1 Sintaxis Básica
* **Encabezados:** `# H1`, `## H2`, `### H3`
* **Énfasis:** `*cursiva*`, `**negrita**`, `***ambas***`
* **Listas:**
    * No ordenadas: `*` o `-`
    * Ordenadas: `1.`
* **Enlaces e Imágenes:**
    * Enlace: `[Texto](URL)`
    * Imagen: `![Texto Alternativo](URL)`
* **Código:**
    * En línea: \`código\`
    * Bloque: 
      \```python
      print("Hola Mundo")
      \```

### 1.2 Por qué usar Markdown
1. **Portabilidad:** Es texto plano, legible en cualquier editor.
2. **Versatilidad:** Se puede convertir a HTML, PDF, ePub, etc.
3. **Integración:** Nativamente soportado en repositorios de código para READMEs, wikis y issues.

## 2. Otras Herramientas de Documentación
Aunque Markdown es excelente para documentación general, existen herramientas más potentes para documentación técnica de APIs o proyectos complejos:

* **Sphinx:** Generador de documentación escrito en Python. Es el estándar para proyectos Python. Utiliza reStructuredText (reST) aunque soporta Markdown. Genera sitios web estáticos muy completos.
* **Doxygen:** Herramienta estándar para generar documentación a partir de código fuente anotado (C++, C, Java, Python, etc.). Extrae comentarios del código para crear manuales de referencia.

## 3. Plantillas para Documentación Profesional
El uso de plantillas estandariza la comunicación y asegura que no se olvide información crítica.

### Ejemplo de Estructura de un README PRO
```markdown
# Nombre del Proyecto

Descripción breve y atractiva.

## 🚀 Comenzando
Instrucciones para tener el proyecto corriendo en local.

### Prerrequisitos
* Node.js >= 14
* npm

### Instalación
1. Clona el repo
2. Instala dependencias (`npm install`)
3. Ejecuta (`npm start`)

## 🛠️ Tecnologías
* React
* Firebase

## ✒️ Autores
* **Tu Nombre** - [Link a Perfil]

## 📄 Licencia
Este proyecto está bajo la Licencia MIT.
```
