# 🧩 Sistema de Gestión de Alumnos — Proyecto de Ingeniería de Software

> **Descripción general:**  
> Proyecto académico destinado al desarrollo de un sistema para la **gestión dinámica de listas de alumnos**, **dispensas** y **asistencias** en un entorno universitario donde las inscripciones permanecen abiertas durante todo el año.  

---

## 📚 Navegación rápida

| Sección | Descripción |
|----------|--------------|
| 🧠 [Modelo del Dominio](./documents/ModeloDelDominio/) | Diagramas conceptuales y definición de entidades principales. |
| 🧾 [Casos de Uso](./documents/CasosDeUso/) | Escenarios funcionales con actores, flujos y resultados esperados. |
| 📁 [Archivos del Proyecto](./documents/) | Documentos base, entregas y materiales del equipo. |
| 🧍‍♂️ [Reuniones](./documents/Reuniones/) | Actas y registros de cada sesión de requisitado. |
| 🖼️ [Recursos Visuales (Fotos/Diagramas)](./documents/images/) | Fotos de pizarras, diagramas, o maquetas iniciales. |

---

## 🧩 Contexto del problema

Las **listas de alumnos** deben mantenerse actualizadas en todo momento, dado que las **inscripciones están siempre abiertas**.  
Esto implica desafíos como:

- **Ingreso tardío de alumnos:**  
  Los nuevos alumnos no deben acumular faltas previas a su fecha de ingreso.

- **Dispensas:**  
  - Si la **dispensa** es **confirmada por el Director**, se aplica automáticamente desde la fecha indicada.  
  - Si la **dispensa** es **solicitada por el alumno**, pero no confirmada, queda en estado **pending** hasta revisión.

- **Asignaturas compartidas:**  
  Un mismo alumno puede estar matriculado en varias asignaturas.  
  El sistema debe **distinguir las dispensas por asignatura.**

- **Evaluaciones:**  
  Las **dispensas no afectan evaluaciones**, pero el sistema debe **notificar al alumno** de este hecho.

- **Asistencia:**  
  Se busca una forma **más eficiente de registrar la asistencia**, considerando múltiples asignaturas.

- **Historial académico:**  
  El sistema debe permitir detectar si **un alumno actual cursó asignaturas anteriores.**


## 🧭 Próximos pasos

1. ⏳ Crear diagrama de dominio (relaciones entre Alumnos, Asignaturas, Dispensas, Asistencias).  
2. ⏳ Redactar casos de uso por actor.  
3. ⏳ Especificar requerimientos funcionales y no funcionales.  
4. ⏳ Diseñar mockups o prototipos de interfaz (opcional).  
5. ⏳ Revisar consistencia de reglas de negocio con el equipo.

---
