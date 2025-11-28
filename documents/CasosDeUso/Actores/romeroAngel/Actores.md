# Actores a considerar

Partiendo de la premisa *"Un actor es una entidad externa que interactúan con el sistema"* se pueden considerar los siguientes Actores:

1. ### Alumno:
    - Solicita una dispensa
    - Apela a una solicitud de Dispensa.
    - Consulta su historial(?)
    - Asiste a sesiones de clase

1. ### Profesor:
    - Gestiona una sesion de clase:
        - Inicia sesion
        - Toma asistencia
        - Finaliza sesion
    - Consulta Lista de Alumnos 
    - Modifica Lista de Alumnos(?)
    - Imparte Asignatura 

1. ### DirectorDeGrado:
    - Revisa una dispensa:
        - Aprueba una dispensa
        - Rechaza una dispensa
    - Consulta Asignaturas
    - Consulta Lista de Alumnos
    - Consulta Cursos


1. ### Secretaría:
    - Gestiona solicitudes de dispensa:
        - Recibe solicitudes
        - Revisa formato correcto
        - Envia Solicitud (ya revisada) a Director De Grado.
        - Recibe la decisión del Director
        - Notifica al Alumno sobre el resultado.
    - Gestiona apelaciones:
        - Gestiona solicitud de dispensa.
