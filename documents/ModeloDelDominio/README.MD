# 🧠 Modelo del Dominio — Sistema de Gestión de Alumnos

> **Descripción general:**  
> Esta sección contiene los artefactos que describen la **estructura conceptual** del sistema.  
> El modelo del dominio representa las **entidades principales**, sus **atributos** y **relaciones**, sirviendo como base para el diseño posterior y la definición de casos de uso.

---

## 📚 Contenido del modelo del dominio

| Artefacto | Descripción |
|------------|-------------|
| 🧩 [Diagrama de Clases](./DiagramasDeClase/) | Representa las entidades del sistema, sus atributos, operaciones y relaciones entre ellas. |
| 🔄 [Diagrama de Estados](./DiagramasDeEstado/Dispensas/) | Describe los posibles estados de las entidades dinámicas (como Alumno o Dispensa) y las transiciones entre ellos. |
| 🧮 [Diccionario de Clases](./DiccionarioDeClases.md) | Define los atributos y métodos de cada clase con su descripción y tipo de dato.
---

## 🧩 Objetivos del modelo del dominio

El **modelo del dominio** busca:

1. **Identificar las entidades centrales del sistema**, tales como:
   - Alumno  
   - Asignatura  
   - Dispensa  
   - Asistencia  
   - Profesor  
   - Director  
   - Secretaría  

2. **Establecer las relaciones** entre ellas, por ejemplo:
   - Un Alumno puede estar inscrito en varias Asignaturas.  
   - Cada Asignatura tiene múltiples Asistencias registradas.  
   - Las Dispenas se asocian a un Alumno y a una Asignatura específica.  
   - El Director autoriza o revisa las Dispenas.  

3. **Servir como base conceptual** para:
   - Los **Casos de Uso** (interacciones entre actores y entidades).  
   - El **Diseño de Clases** (estructura de implementación futura).  
   - El **Modelo de Datos** (mapa para el desarrollo de la base de datos).

---

## 🔍 Diagrama de Clases

📁 [Abrir diagrama](./DiagramaDeClases.png)

El **Diagrama de Clases** refleja la estructura estática del sistema.  
Permite visualizar las entidades principales, sus atributos y los vínculos entre ellas.  
Se centra en el **qué existe** en el sistema, no en **cómo se comporta**.

**Elementos principales:**
- **Clases:** representan objetos del dominio (Alumno, Dispensa, Asignatura, etc.).  
- **Atributos:** propiedades que describen las clases.  
- **Asociaciones:** relaciones entre las clases (1 a N, N a N, etc.).  
- **Generalizaciones:** jerarquías o herencia si corresponde.

---

## 🔄 Diagrama de Estados

📁 [Abrir diagrama](./DiagramaDeEstados.png)

El **Diagrama de Estados** muestra los diferentes **estados posibles** de una entidad y **cómo cambia** según las acciones del sistema o los actores.

**Ejemplo:**  
Entidad: `Dispensa`
- Estado inicial: *Solicitada*  
- Transición: *Aprobación del Director*  
- Estado final: *Aprobada* o *Rechazada*

Este diagrama ayuda a entender **cómo evoluciona la información** dentro del sistema y qué eventos provocan esos cambios.

---

## 📘 Vocabulario

📄 [Ver documento completo](./DiccionarioDeClases.md)

Describe cada clase del modelo con:
- Su propósito dentro del sistema.  
- Sus atributos (nombre, tipo de dato, descripción).  
- Sus métodos principales o comportamientos esperados.  

Este documento complementa al diagrama, aportando detalle textual y semántico.

---


> ✨ *El modelo del dominio constituye la base conceptual del proyecto, garantizando que todos los miembros del equipo compartan una misma comprensión sobre la estructura y funcionamiento del sistema.*
