# Historias de Usuario - LABCONTROL

Las historias de usuario están construidas con el formato: **«Como [tipo de usuario], quiero [funcionalidad], para [beneficio]»**.

---

### HU-01 — Inicio de sesión

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como usuario registrado, quiero iniciar sesión mediante usuario/correo y contraseña, para acceder a las funciones correspondientes a su rol. |
| **Prioridad XP** | Alta |
| **Story Points** | 8 |
| **Iteración** | 1 |
| **Criterios de aceptación** | - Las credenciales se validan.<br>- El acceso depende de credenciales válidas.<br>- El usuario accede según su rol. |
| **Tareas** | - Diseñar login<br>- Implementar validación<br>- Aplicar roles y permisos<br>- Probar acceso válido e inválido |

---

### HU-02 — Consultar disponibilidad de laboratorios

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como estudiante o docente, quiero consultar laboratorios disponibles según fecha y horario, para encontrar un espacio sin revisar físicamente cada laboratorio. |
| **Prioridad XP** | Alta |
| **Story Points** | 3 |
| **Iteración** | 1 |
| **Criterios de aceptación** | - Se puede seleccionar fecha y horario.<br>- Se muestran laboratorios disponibles/no disponibles. |
| **Tareas** | - Diseñar consulta<br>- Relacionar horarios y laboratorios<br>- Implementar filtros<br>- Probar resultados |

---

### HU-03 — Consultar horarios

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como estudiante o docente, quiero consultar los horarios registrados de un laboratorio, para planificar el uso del espacio con información organizada. |
| **Prioridad XP** | Alta |
| **Story Points** | 3 |
| **Iteración** | 1 |
| **Criterios de aceptación** | - Se selecciona un laboratorio.<br>- Se muestran día y horas.<br>- El horario corresponde al periodo académico. |
| **Tareas** | - Diseñar vista<br>- Crear consulta<br>- Relacionar laboratorio y periodo<br>- Probar visualización |

---

### HU-04 — Consultar información de laboratorio

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como estudiante, docente o encargado, quiero consultar información básica de un laboratorio, para conocer sus características antes de utilizarlo o solicitarlo. |
| **Prioridad XP** | Media |
| **Story Points** | 3 |
| **Iteración** | 1 |
| **Criterios de aceptación** | - Se muestran nombre, ubicación, capacidad, estado y descripción. |
| **Tareas** | - Diseñar ficha<br>- Consultar datos<br>- Mostrar información<br>- Probar diferentes laboratorios |

---

### HU-05 — Solicitar uso de laboratorio

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como estudiante o docente, quiero enviar una solicitud indicando laboratorio, fecha, horario y motivo, para gestionar el uso del laboratorio de forma organizada. |
| **Prioridad XP** | Alta |
| **Story Points** | 5 |
| **Iteración** | 1 |
| **Criterios de aceptación** | - Se selecciona laboratorio, fecha y horario.<br>- Se registra el motivo.<br>- Se validan campos obligatorios.<br>- La solicitud queda registrada. |
| **Tareas** | - Diseñar formulario<br>- Validar disponibilidad<br>- Guardar solicitud<br>- Asignar estado inicial |

---

### HU-06 — Consultar mis solicitudes

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como estudiante o docente, quiero ver mis solicitudes realizadas, para dar seguimiento a las solicitudes enviadas. |
| **Prioridad XP** | Media |
| **Story Points** | 3 |
| **Iteración** | 1 |
| **Criterios de aceptación** | - Solo aparecen solicitudes del usuario autenticado.<br>- Se muestran fecha, laboratorio, horario y estado. |
| **Tareas** | - Crear listado<br>- Filtrar por usuario<br>- Diseñar vista<br>- Probar estados |

---

### HU-07 — Consultar estado de solicitud

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como estudiante o docente, quiero consultar el estado de una solicitud, para saber si está pendiente, aprobada o rechazada. |
| **Prioridad XP** | Media |
| **Story Points** | 3 |
| **Iteración** | 1 |
| **Criterios de aceptación** | - Cada solicitud muestra un estado.<br>- El estado corresponde al registro almacenado. |
| **Tareas** | - Definir estados<br>- Mostrar estado<br>- Validar cambios<br>- Probar seguimiento |

---

### HU-08 — Gestionar solicitudes

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como encargado del Centro de Cómputo, quiero revisar y aprobar o rechazar solicitudes, para controlar el uso de los laboratorios. |
| **Prioridad XP** | Alta |
| **Story Points** | 5 |
| **Iteración** | 2 |
| **Criterios de aceptación** | - El encargado ve solicitudes pendientes.<br>- Puede aprobar o rechazar.<br>- El nuevo estado queda registrado. |
| **Tareas** | - Diseñar panel<br>- Implementar aprobar/rechazar<br>- Registrar cambios<br>- Controlar permisos |

---

### HU-09 — Registrar utilización

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como encargado del Centro de Cómputo, quiero registrar el uso de un laboratorio o equipo, para mantener trazabilidad de utilización. |
| **Prioridad XP** | Media |
| **Story Points** | 5 |
| **Iteración** | 2 |
| **Criterios de aceptación** | - Se registra usuario, laboratorio/equipo, fecha y observación cuando corresponda. |
| **Tareas** | - Diseñar registro<br>- Crear estructura<br>- Validar datos<br>- Guardar y consultar |

---

### HU-10 — Administrar laboratorios

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como encargado o administrador, quiero registrar y actualizar laboratorios, para mantener actualizada la información base. |
| **Prioridad XP** | Media |
| **Story Points** | 5 |
| **Iteración** | 2 |
| **Criterios de aceptación** | - Puede registrar y modificar laboratorios.<br>- Se controla el estado. |
| **Tareas** | - CRUD de laboratorios<br>- Validar datos<br>- Implementar estados<br>- Probar |

---

### HU-11 — Administrar horarios

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como encargado o administrador, quiero registrar y actualizar horarios, para mantener disponible la información operativa. |
| **Prioridad XP** | Media |
| **Story Points** | 5 |
| **Iteración** | 2 |
| **Criterios de aceptación** | - El horario se asocia a laboratorio y periodo.<br>- Se registran día y horas. |
| **Tareas** | - Gestión de horarios<br>- Relacionar entidades<br>- Validar datos<br>- Probar |

---

### HU-12 — Administrar usuarios y roles

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como administrador, quiero gestionar usuarios y asignar roles, para controlar acceso a funciones. |
| **Prioridad XP** | Media |
| **Story Points** | 5 |
| **Iteración** | 2 |
| **Criterios de aceptación** | - Cada usuario tiene un rol.<br>- Solo usuarios autorizados gestionan usuarios. |
| **Tareas** | - Gestión de usuarios<br>- Implementar roles<br>- Aplicar permisos<br>- Probar perfiles |

---

### HU-13 — Reportar incidencia

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como estudiante, docente o encargado, quiero registrar una incidencia indicando laboratorio y equipo, para dejar constancia de una falla para facilitar su atención. |
| **Prioridad XP** | Alta |
| **Story Points** | 5 |
| **Iteración** | 3 |
| **Criterios de aceptación** | - Se selecciona laboratorio/equipo cuando corresponda.<br>- Se registra descripción, fecha y usuario.<br>- La incidencia queda con estado inicial. |
| **Tareas** | - Diseñar formulario<br>- Relacionar equipo/laboratorio<br>- Guardar reporte<br>- Definir estados |

---

### HU-14 — Consultar estado de incidencia

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como usuario que reportó o personal autorizado, quiero consultar el estado de una incidencia, para conocer si está pendiente, en atención o resuelta. |
| **Prioridad XP** | Media |
| **Story Points** | 3 |
| **Iteración** | 3 |
| **Criterios de aceptación** | - Se muestra el estado.<br>- El usuario autorizado puede consultar el detalle. |
| **Tareas** | - Diseñar consulta<br>- Implementar estados<br>- Controlar permisos<br>- Probar |

---

### HU-15 — Gestionar incidencias

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como encargado o técnico autorizado, quiero revisar y actualizar incidencias, para dar seguimiento ordenado a fallas. |
| **Prioridad XP** | Alta |
| **Story Points** | 5 |
| **Iteración** | 3 |
| **Criterios de aceptación** | - Se visualizan incidencias.<br>- Se actualiza estado.<br>- Se registra fecha de atención y observación técnica. |
| **Tareas** | - Diseñar panel<br>- Actualizar estados<br>- Registrar atención<br>- Controlar permisos |

---

### HU-16 — Consultar historial de solicitudes

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como encargado o administrador, quiero consultar solicitudes anteriores, para obtener trazabilidad histórica. |
| **Prioridad XP** | Baja |
| **Story Points** | 5 |
| **Iteración** | 4 |
| **Criterios de aceptación** | - Se consultan solicitudes históricas.<br>- Se muestran datos principales. |
| **Tareas** | - Diseñar historial<br>- Implementar filtros<br>- Consultar registros |

---

### HU-17 — Consultar historial de incidencias

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como encargado o administrador, quiero consultar incidencias anteriores, para identificar antecedentes de equipos. |
| **Prioridad XP** | Baja |
| **Story Points** | 5 |
| **Iteración** | 4 |
| **Criterios de aceptación** | - Se identifican laboratorio y equipo.<br>- Se muestran estados y fechas. |
| **Tareas** | - Diseñar historial<br>- Implementar filtros<br>- Consultar registros |

---

### HU-18 — Generar reportes de gestión

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como administrador o encargado, quiero generar reportes sobre solicitudes, utilización e incidencias, para apoyar la revisión de la gestión. |
| **Prioridad XP** | Baja |
| **Story Points** | 5 |
| **Iteración** | 4 |
| **Criterios de aceptación** | - Se selecciona un tipo de reporte.<br>- La información proviene de registros del sistema. |
| **Tareas** | - Definir reportes<br>- Crear consultas<br>- Diseñar presentación<br>- Validar datos |

---

### HU-19 — Recibir notificaciones

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como usuario del sistema, quiero recibir avisos sobre solicitudes o incidencias, para conocer cambios importantes oportunamente. |
| **Prioridad XP** | Media |
| **Story Points** | 5 |
| **Iteración** | 4 |
| **Criterios de aceptación** | - Se genera aviso ante eventos definidos.<br>- La notificación corresponde al usuario. |
| **Tareas** | - Definir eventos<br>- Diseñar notificaciones<br>- Implementar generación<br>- Probar |

---

### HU-20 — Visualizar indicadores y estadísticas

| Campo | Contenido |
| :--- | :--- |
| **Historia de usuario** | Como administrador o encargado, quiero consultar indicadores y estadísticas de uso, para obtener una visión resumida del funcionamiento. |
| **Prioridad XP** | Baja |
| **Story Points** | 5 |
| **Iteración** | 4 |
| **Criterios de aceptación** | - Los indicadores usan datos registrados.<br>- La información es comprensible. |
| **Tareas** | - Definir indicadores<br>- Crear consultas agregadas<br>- Diseñar dashboard<br>- Validar cálculos |

# Product Backlog y Matriz RACI - LABCONTROL

---

## 7. Product Backlog

| ID | Requerimiento | Prioridad | Puntos | Iteración |
| :--- | :--- | :--- | :--- | :--- |
| **PB-01** | Inicio de sesión / autenticación | Alta | 8 | 1 |
| **PB-02** | Consultar disponibilidad | Alta | 3 | 1 |
| **PB-03** | Consultar horarios | Alta | 3 | 1 |
| **PB-04** | Consultar información de laboratorio | Media | 3 | 1 |
| **PB-05** | Solicitar uso de laboratorio | Alta | 5 | 1 |
| **PB-06** | Consultar mis solicitudes | Media | 3 | 1 |
| **PB-07** | Consultar estado de solicitud | Media | 3 | 1 |
| **PB-08** | Registrar utilización de laboratorio/equipo | Media | 5 | 2 |
| **PB-09** | Reportar incidencia de equipo | Alta | 5 | 3 |
| **PB-10** | Consultar estado de incidencia | Media | 3 | 3 |
| **PB-11** | Gestionar incidencias | Alta | 5 | 3 |
| **PB-12** | Administrar laboratorios | Media | 5 | 2 |
| **PB-13** | Administrar horarios | Media | 5 | 2 |
| **PB-14** | Administrar usuarios y roles | Media | 5 | 2 |
| **PB-15** | Historial de solicitudes | Baja | 5 | 4 |
| **PB-16** | Historial de incidencias | Baja | 5 | 4 |
| **PB-17** | Reportes de gestión | Baja | 5 | 4 |
| **PB-18** | Indicadores de gestión | Baja | 5 | 4 |
| **PB-19** | Notificaciones | Media | 5 | 4 |
| **PB-20** | Estadísticas de uso | Baja | 5 | 4 |

---

## Matriz RACI actualizada — LABCONTROL
*Equipo de 3 integrantes · Sistema web para la gestión y control de laboratorios del Centro de Cómputo de UNIVALLE*

### 1. Integrantes y roles principales

| Integrante | Rol principal | Responsabilidades |
| :--- | :--- | :--- |
| **Dustin Fernando Vaca Aguilar** | Desarrollador Frontend / UX-UI | Interfaces, formularios, navegación, experiencia de usuario y pruebas visuales. |
| **Jorge Angel Cores Andrade** | Desarrollador Backend / Base de Datos | API, lógica de negocio, diseño de base de datos e integración con el servidor. |
| **Jheremy Jhostin Ramirez Arcani** | Analista de requisitos y coordinador del proyecto | Requisitos, historias de usuario, seguimiento de tareas, documentación, coordinación de integración y apoyo en pruebas. |

### 2. Matriz RACI por actividad
*Leyenda: **R** = Responsable · **A** = Aprobador · **C** = Consultado · **I** = Informado.*

| Actividad | Dustin | Jorge | Jheremy |
| :--- | :---: | :---: | :---: |
| **1. Levantamiento de requisitos** | C | C | R/A |
| **2. Historias de usuario y Product Backlog** | C | C | R/A |
| **3. Diseño de la base de datos** | I | R/A | C |
| **4. Diseño de interfaces UX/UI** | R/A | C | C |
| **5. Desarrollo del Frontend** | R/A | C | I |
| **6. Desarrollo del Backend y API** | C | R/A | I |
| **7. Integración Frontend–Backend** | R | R | A |
| **8. Pruebas de interfaz y navegación** | R/A | C | C |
| **9. Pruebas de API y base de datos** | C | R/A | C |
| **10. Pruebas funcionales generales** | R | R | A |
| **11. Gestión de tareas e Issues** | C | C | R/A |
| **12. Repositorio, ramas y convenciones de commits** | R | R/A | C |
| **13. Documentación técnica y README** | C | C | R/A |
| **14. Manual de usuario** | R | C | R/A |
| **15. Seguimiento de avances e iteraciones XP** | C | C | R/A |
| **16. Preparación y defensa de la exposición** | R | R | R/A |
