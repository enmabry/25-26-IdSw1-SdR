# Priorización de Casos de Uso
## Centro de Gestión Universitaria

**Criterio de Priorización:** Complejidad técnica + dependencias del sistema + riesgos de implementación.

---

## Tabla Maestra de Casos de Uso Priorizados

| Prioridad | Fase | Caso de Uso | Módulo/Actor | Complejidad | Dependencias | Bloquea | Duración | Riesgos Clave |
|-----------|------|------------|--------------|-------------|--------------|--------|----------|---------------|
| 1 | 0 | CRUD Usuarios + Autenticación | Infraestructura | Alta | Ninguna | Todas | 1 sp | Encriptación, integridad de acceso |
| 2 | 1A | Crear Usuario | Admin | Baja | Fase 0 | - | 1 d | Validación de unicidad |
| 3 | 1A | Consultar Usuario | Admin | Baja | Fase 0 | - | 1 d | Visualización |
| 4 | 1A | Editar Usuario | Admin | Media | Fase 0 | - | 2 d | Auditoría de cambios |
| 5 | 1A | Guardar Usuario | Admin | Baja | Fase 0 | - | 1 d | Persistencia |
| 6 | 1A | Cerrar Usuario | Admin | Baja | Fase 0 | - | 1 d | Navegación |
| 7 | 1B | Generar Listado de Alumnos por Curso | Secretaria | Media | Fase 0 | - | 1-2 sp | Filtrado dinámico, rendimiento |
| 8 | 1C | Consultar Lista de Alumnos | Profesor/Secretaria | Baja | Fase 1A | - | 1-2 d | Visualización |
| 9 | 1C | Ver Detalle de Alumno | Profesor/Secretaria | Baja | Fase 1A | - | 1-2 d | Información correlacionada |
| 10 | 1C | Actualizar Datos de Alumno | Secretaria | Media | Fase 1A | - | 1-2 sp | Validación múltiple, auditoría |
| 11 | 1C | Eliminar Alumno | Secretaria | Media | Fase 1A | - | 1-2 d | Cascada de eliminación |
| 12 | 1C | Importar Alumnos | Profesor | **Crítica** | Fase 1A | Fases 1D, 2, 3 | 2-3 sp | Validación, duplicados, transacciones |
| 13 | 1D | Ver Detalle de Matrícula | Admin | Media | Fase 1C | - | 1-2 d | Información referencial |
| 14 | 1D | Importar Matrículas | Admin | **Crítica** | Fase 1C | Fases 2, 3 | 2-3 sp | Integridad referencial, bulk load |
| 15 | 2 | Crear Sesión de Clase | Profesor | Media | Fase 1D | - | 1-2 sp | Inicialización de contexto |
| 16 | 2 | Registrar Toma de Asistencia | Profesor | **Crítica** | Fase 2.1 | Fase 2.4, 3 | 2-3 sp | Sincronización, cálculos, integridad |
| 17 | 2 | Cerrar Sesión de Clase | Profesor | Baja | Fase 2.2 | - | 1 d | Transición de estado |
| 18 | 2 | Exportar Historial de Asistencias | Profesor | **Crítica** | Fase 2.2 | - | 2-3 sp | Generación PDF/Excel, estadísticas |
| 19 | 3 | Crear Solicitud de Dispensa (Alumno) | Alumno | Media | Fase 2 | - | 1 sp | Validación formulario |
| 20 | 3 | Editar Solicitud de Dispensa (Alumno) | Alumno | Media | Fase 2 | - | 1 sp | Validación de estado |
| 21 | 3 | Guardar Solicitud de Dispensa (Alumno) | Alumno | Media | Fase 2 | - | 1 sp | Transaccionalidad |
| 22 | 3 | Ver Estado de Dispensa (Alumno) | Alumno | Baja | Fase 2 | - | 1 d | Sincronización |
| 23 | 3 | Cerrar Solicitud de Dispensa (Alumno) | Alumno | Baja | Fase 3.1 | - | 1 d | Transición de estado |
| 24 | 3 | Crear Solicitud de Dispensa (Secretaria) | Secretaria | Media | Fase 2 | - | 1 sp | Búsqueda de alumno |
| 25 | 3 | Adjuntar Documentación de Dispensa | Secretaria | Media | Fase 3.1 | - | 1-2 sp | Gestión de archivos, validación |
| 26 | 3 | Ver Estado de Dispensa (Secretaria) | Secretaria | Baja | Fase 2 | - | 1 d | Sincronización |
| 27 | 3 | Generar Informe de Dispensas | Secretaria | **Crítica** | Fase 3.1 | - | 2-3 sp | Filtrado dinámico, agregación, reportes |
| 28 | 3 | Cerrar Solicitud de Dispensa (Secretaria) | Secretaria | Baja | Fase 3.2 | - | 1 d | Transición de estado |
| 29 | 3 | Consultar Solicitudes de Dispensas | Director Grado | Media | Fase 2 | - | 1-2 sp | Filtrado avanzado, refrescado |
| 30 | 3 | Editar Solicitud de Dispensa (Director) | Director Grado | Media | Fase 3.7 | - | 1 sp | Validación, auditoría |
| 31 | 3 | Guardar Cambios de Dispensa (Director) | Director Grado | Media | Fase 3.8 | - | 1 sp | Persistencia segura |
| 32 | 3 | Cerrar Solicitud de Dispensa (Director) | Director Grado | Baja | Fase 3.8 | - | 1 d | Transición de estado |
| 33 | 3 | Consultar Solicitud de Dispensa (Profesor) | Profesor | Media | Fase 2 | - | 1 sp | Filtrado básico |

---

| Fase | Sprint | Casos de Uso | Esfuerzo Total | Duración | Prerequisitos |
|------|--------|--------------|-----------------|----------|---------------|
| 0 | 1 | CRUD Usuarios + Autenticación | 1 sprint | 1 sp | Ninguno |
| 1A | 2 | Crear, Consultar, Editar, Guardar, Cerrar Usuario | 1 sprint | 1 sp | Fase 0 |
| 1B | 2-3 | Generar Listado de Alumnos por Curso | 1-2 sprints | 1-2 sp | Fase 0 |
| 1C | 3-4 | Alumnos: Consultar, Ver, Actualizar, Eliminar, **Importar** | 2-3 sprints | 2-3 sp | Fase 1A, 1B |
| 1D | 4-5 | Matrículas: Ver Detalle, **Importar** | 2-3 sprints | 2-3 sp | Fase 1C |
| 2 | 6-8 | Asistencias: Crear Sesión, **Registrar**, Cerrar, **Exportar Historial** | 3 sprints | 3 sp | Fase 1D |
| 3 | 9-12 | Dispensas: Alumno (5), Secretaria (5), Director (4), Profesor (1) | 4 sprints | 4 sp | Fase 2 |

**Total:** 32 Casos de Uso en 7 fases | Duración estimada: 14-16 sprints (7-8 meses)

---

## Casos de Uso Críticos

| ID | Caso de Uso | Módulo | Duración | Riesgo Principal |
|----|------------|--------|----------|------------------|
| 12 | Importar Alumnos | Profesor | 2-3 sp | Validación, duplicados, transacciones parciales |
| 14 | Importar Matrículas | Admin | 2-3 sp | Integridad referencial, carga masiva |
| 16 | Registrar Toma de Asistencia | Profesor | 2-3 sp | Sincronización, cálculos, historial |
| 18 | Exportar Historial de Asistencias | Profesor | 2-3 sp | Generación de reportes PDF/Excel, estadísticas |
| 27 | Generar Informe de Dispensas | Secretaria | 2-3 sp | Filtrado múltiple, agregación, rendimiento |

---




