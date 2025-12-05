<div align="center">

| [![](https://img.shields.io/badge/🏠_INICIO-1565C0?style=for-the-badge&labelColor=0D47A1)](/README.md) [![](https://img.shields.io/badge/📘_MODELO_DEL_DOMINIO-1E88E5?style=for-the-badge&labelColor=1565C0)](/documents/ModeloDelDominio/) [![](https://img.shields.io/badge/🧍‍♂️_ACTORES-1E88E5?style=for-the-badge&labelColor=1565C0)](/documents/CasosDeUso/Actores/) [![](https://img.shields.io/badge/📄_CASOS_DE_USO-1E88E5?style=for-the-badge&labelColor=1565C0)](/documents/CasosDeUso/) [![](https://img.shields.io/badge/🔍_DETALLADO_CASOS_DE_USO-555555?style=for-the-badge&labelColor=2b2b2b)](/documents/CasosDeUso/DetalladoCasosDeUso/) [![](https://img.shields.io/badge/🌐_DIAGRAMA_DE_CONTEXTO-1E88E5?style=for-the-badge&labelColor=1565C0)](/documents/CasosDeUso/DiagramaDeContexto/) [![](https://img.shields.io/badge/🧩_PROTOTIPOS-555555?style=for-the-badge&labelColor=2b2b2b)](/documents/CasosDeUso/Prototipos) [![](https://img.shields.io/badge/👥_REUNIONES-555555?style=for-the-badge&labelColor=2b2b2b)](/documents/Reuniones/) [![](https://img.shields.io/badge/🖼️_RECURSOS_ADICIONALES-555555?style=for-the-badge&labelColor=2b2b2b)](/documents/images/) |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |

</div>

---

# 📂 Documentación del Proyecto

> Este directorio agrupa **todos los artefactos generados durante la fase de requisitado** del sistema **de Gestión de Alumnos**, incluyendo modelos, diagramas, descripciones y materiales de apoyo.  
> Su propósito es **mantener la trazabilidad del análisis**, desde los primeros requisitos hasta la definición completa de funcionalidades.

---

## 🧭 Flujo de trabajo documental

La carpeta `documents/` refleja el **proceso de construcción progresiva del sistema**, donde cada sección representa un paso dentro del análisis y diseño.

### 🔹 1. **Modelo del Dominio**
Contiene los **diagramas de clases** y **modelos conceptuales** que definen las entidades principales y sus relaciones.  
Sirve como base para comprender el sistema y derivar los casos de uso.  

📁 [`/documents/ModeloDelDominio/`](./ModeloDelDominio/)

---

### 🔹 2. **Casos de Uso**
Estructura central donde se descompone el comportamiento del sistema.  
Dividido en subcarpetas para un desarrollo modular y ordenado:

- 🧍‍♂️ [`Actores`](./CasosDeUso/Actores/) — Define los roles y agentes externos que interactúan con el sistema.  
- 📄 [`Casos de Uso`](./CasosDeUso/) — Diagramas globales y descripciones funcionales.  
- 🔍 [`Detallado Casos de Uso`](./CasosDeUso/DetalladoCasosDeUso/) — Flujos, postcondiciones y escenarios alternos.  
- 🌐 [`Diagrama de Contexto`](./CasosDeUso/DiagramaDeContexto/) — Representa el sistema en relación con su entorno.  
- 🧩 [`Prototipos`](./CasosDeUso/Prototipos/) — Bocetos y representaciones gráficas preliminares de interfaz.

---

### 🔹 3. **Reuniones**
Registro cronológico de las **sesiones de requisitado**.  
Incluye decisiones, observaciones y cambios en los requerimientos del sistema.

📁 [`/documents/Reuniones/`](./Reuniones/)

---

### 🔹 4. **Recursos Visuales**
Contiene imágenes, fotos, y diagramas auxiliares utilizados en las sesiones o documentos del proyecto.

📁 [`/documents/images/`](./images/)

---

## ⚙️ Estructura de análisis del sistema

El sistema se aborda desde tres ejes principales:

| Módulo | Descripción | Objetivo |
|--------|--------------|-----------|
| 🧾 **Listas de Alumnos** | Representa la estructura dinámica de inscripciones que cambian durante el ciclo lectivo. | Mantener actualizadas las listas ante nuevos ingresos. |
| 🕒 **Asistencias** | Registra la presencia o ausencia de alumnos en clases y actividades. | Garantizar el control eficiente y automatizado. |
| 🪪 **Dispensas** | Maneja solicitudes de excusas o permisos, tanto de alumnos como del director. | Determinar las condiciones bajo las cuales se aplican o quedan pendientes. |

Cada una de estas áreas se desarrolla progresivamente a través de los artefactos del repositorio (diagramas, casos de uso, reuniones y modelos conceptuales).

---

## 📘 Notas finales

- Este repositorio sigue un **flujo incremental**: cada sesión de trabajo amplía o refina los documentos existentes.  
- Los **colaboradores** deben trabajar en **ramas individuales**, actualizando siempre desde `develop` antes de crear nuevos cambios.  
- La documentación se mantendrá **sincronizada con los avances del proyecto funcional** para conservar coherencia entre análisis y desarrollo.

---

> 🧩 *Proyecto desarrollado en el marco de la asignatura Ingeniería de Software — Fase de Requisitado.*
