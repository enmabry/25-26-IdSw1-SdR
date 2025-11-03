<h1 align="center">🧩 Sistema de Gestión de Alumnos — Proyecto de Ingeniería de Software</h1>

<p align="center">
  <i>Proyecto académico orientado al desarrollo de un sistema para la gestión dinámica de listas de alumnos, dispensas y asistencias.</i>
</p>

---
<div align="center" style="
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 8px;
  background-color: #202225;
  border: 1px solid #333;
  border-radius: 6px;
  padding: 12px;
  margin: 20px 0;
">

  <!-- Modelo del Dominio (activo / color) -->
  <a href="./documents/ModeloDelDominio/" style="
    background-color: #1976D2;
    color: white;
    text-decoration: none;
    font-weight: bold;
    font-family: 'Segoe UI', sans-serif;
    padding: 8px 14px;
    border-radius: 6px;
    border: 1px solid #0D47A1;
    transition: 0.3s;
  ">
    📘 Modelo del Dominio
  </a>

  <!-- Casos de Uso (gris, pendiente) -->
  <a href="./documents/CasosDeUso/" style="
    background-color: #2b2b2b;
    color: #bbb;
    text-decoration: none;
    font-weight: bold;
    font-family: 'Segoe UI', sans-serif;
    padding: 8px 14px;
    border-radius: 6px;
    border: 1px solid #444;
    transition: 0.3s;
  ">
    📄 Casos de Uso
  </a>

  <!-- Archivos del Proyecto -->
  <a href="./documents/" style="
    background-color: #2b2b2b;
    color: #bbb;
    text-decoration: none;
    font-weight: bold;
    font-family: 'Segoe UI', sans-serif;
    padding: 8px 14px;
    border-radius: 6px;
    border: 1px solid #444;
    transition: 0.3s;
  ">
    🗂️ Archivos del Proyecto
  </a>

  <!-- Reuniones -->
  <a href="./documents/Reuniones/" style="
    background-color: #2b2b2b;
    color: #bbb;
    text-decoration: none;
    font-weight: bold;
    font-family: 'Segoe UI', sans-serif;
    padding: 8px 14px;
    border-radius: 6px;
    border: 1px solid #444;
    transition: 0.3s;
  ">
    👥 Reuniones
  </a>

  <!-- Recursos Visuales -->
  <a href="./documents/images/" style="
    background-color: #2b2b2b;
    color: #bbb;
    text-decoration: none;
    font-weight: bold;
    font-family: 'Segoe UI', sans-serif;
    padding: 8px 14px;
    border-radius: 6px;
    border: 1px solid #444;
    transition: 0.3s;
  ">
    🖼️ Recursos Visuales
  </a>

</div>

---

## 📚 Descripción general

Este repositorio contiene los artefactos correspondientes a la **fase de requisitado** del proyecto.  
El objetivo es modelar un sistema capaz de gestionar:

- Alumnos y su inscripción dinámica durante el año lectivo.  
- Dispensas (solicitadas por alumno o director).  
- Asistencias diferenciadas por asignatura.  
---

## 🧩 Contexto del problema

Las **listas de alumnos** deben mantenerse actualizadas en todo momento, dado que las **inscripciones están siempre abiertas**. Esto implica desafíos como:

- **Ingreso tardío de alumnos:** los nuevos no deben acumular faltas previas.  
- **Dispensas:** pueden ser aprobadas (director) o pendientes (alumno).  
- **Asignaturas compartidas:** un alumno puede estar en varias materias.  
- **Evaluaciones:** las dispensas no omiten evaluaciones, pero deben notificar al alumno.  
- **Asistencia:** registro más eficiente en múltiples asignaturas.  
- **Historial académico:** detectar si un alumno ya cursó asignaturas previas.  
---
<h2 id="proximos-pasos">🧭 Próximos pasos</h2>

<p align="center">
  <img alt="Estado: En progreso" src="https://img.shields.io/badge/⏳%20Estado-En%20progreso-ffb300?style=for-the-badge">
</p>

<p align="center">
  <strong>Progreso general</strong><br>
  <code>░░░░░</code> 0 / 5 completadas  
</p>

<table align="center">
  <tr>
    <td>
      <img src="https://img.shields.io/badge/⏳-Diagrama_de_Dominio-1976d2?style=for-the-badge" alt="Diagrama de Dominio">
    </td>
    <td>
      <img src="https://img.shields.io/badge/⚪-Casos_de_Uso-9e9e9e?style=for-the-badge" alt="Casos de Uso">
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://img.shields.io/badge/⚪-Req._Func._y_NoFunc.-9e9e9e?style=for-the-badge" alt="Requisitos">
    </td>
    <td>
      <img src="https://img.shields.io/badge/⚪-Mockups/Prototipos-9e9e9e?style=for-the-badge" alt="Mockups">
    </td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <img src="https://img.shields.io/badge/⚪-Revisión_de_Reglas-9e9e9e?style=for-the-badge" alt="Revisión">
    </td>
  </tr>
</table>

<ul>
  <li>[] Crear diagrama de dominio.</li>
  <li>[ ] Redactar casos de uso por actor.</li>
  <li>[ ] Especificar requerimientos funcionales y no funcionales.</li>
  <li>[ ] Diseñar mockups o prototipos de interfaz.</li>
  <li>[ ] Revisar consistencia de reglas de negocio con el equipo.</li>
</ul>
---

<div align="center">
  <sub>© 2025 — Proyecto académico para la asignatura <b>Ingeniería de Software</b></sub>
</div>
