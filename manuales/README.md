# Manual de usuario inicial — LABCONTROL

Sistema web de gestión de laboratorios del Centro de Cómputo · Versión 1.0
Grupo SQLitos · Proyecto de Sistemas I · Universidad del Valle, Sede La Paz

## 1. Introducción

LABCONTROL permite consultar la disponibilidad de los laboratorios, solicitar su uso, reportar incidencias y dar seguimiento a cada trámite desde el navegador. Este manual inicial explica las dos funciones principales de la primera iteración: **iniciar sesión** y **solicitar el uso de un laboratorio**.

## 2. Requisitos

- Un navegador web actualizado (Chrome, Edge o Firefox).
- El sistema en ejecución. En el entorno de desarrollo se abre en `http://localhost:5297`.
- Un usuario registrado en el sistema.

## 3. Roles y usuarios de prueba

El sistema tiene cinco roles. En el entorno de pruebas existen estos usuarios, todos con la contraseña `Lab2026*`:

| Usuario | Rol | Qué puede hacer |
| :--- | :--- | :--- |
| `estudiante` | Estudiante | Consultar laboratorios, solicitar uso y reportar incidencias |
| `docente` | Docente | Igual que el estudiante |
| `encargado` | Encargado | Gestionar solicitudes e incidencias, ver utilización |
| `tecnico` | Técnico | Atender incidencias |
| `admin` | Administrador | Administrar usuarios, laboratorios y horarios, ver indicadores y reportes |

## 4. Iniciar sesión

1. Abre el navegador e ingresa a `http://localhost:5297/login`.
2. Escribe tu **usuario o correo** y tu **contraseña**.
3. Presiona el botón **Ingresar**.
4. Si los datos son correctos, entrarás al sistema y verás el menú según tu rol.
5. Si la contraseña es incorrecta, el sistema no permite el acceso y muestra un mensaje de error. Vuelve a intentarlo.

![Pantalla de inicio de sesión](img/01-login.png)

## 5. Solicitar el uso de un laboratorio

Esta función está disponible para estudiantes y docentes.

1. Inicia sesión con tu usuario.
2. En el menú, haz clic en **Nueva solicitud**.
3. Completa el formulario:
   - **Laboratorio:** elige el laboratorio que necesitas.
   - **Fecha:** el día de uso. No puede ser anterior a hoy.
   - **Hora de inicio y hora de fin:** la hora de fin debe ser posterior a la de inicio.
   - **Motivo:** explica para qué usarás el laboratorio.
4. Presiona **Enviar**.
5. El sistema registra la solicitud con estado **Pendiente**.

El sistema rechaza la solicitud si falta algún dato obligatorio, si el horario es inválido o si el laboratorio no está disponible en ese horario.

![Formulario de nueva solicitud](img/02-nueva-solicitud.png)

## 6. Ver el estado de mis solicitudes

1. En el menú, haz clic en **Mis solicitudes**.
2. Verás una tabla con fecha, laboratorio, horario, motivo, estado y respuesta.
3. Puedes filtrar la lista con el selector **Todos los estados**.
4. Una solicitud nueva aparece como **Pendiente** con la respuesta «Esperando respuesta» hasta que el encargado la gestione.

![Lista de Mis solicitudes](img/03-mis-solicitudes.png)

## 7. Cerrar sesión

Haz clic en **Cerrar sesión**, en la parte superior derecha. Es recomendable hacerlo siempre que uses un computador compartido.

## 8. Limitaciones conocidas de la versión 1.0

| Código | Descripción | Estado |
| :--- | :--- | :--- |
| INC-01 | El sistema permite enviar la misma solicitud más de una vez y todas quedan Pendiente. Evita repetir el envío. | Abierta (issue #2) |
| INC-02 | El paquete `System.Security.Cryptography.Pkcs` tiene avisos de vulnerabilidad; no afecta el uso actual. | Abierta (issue #3) |

## 9. Solución de problemas

| Problema | Qué hacer |
| :--- | :--- |
| No puedo ingresar | Revisa el usuario y la contraseña. Si sigue fallando, pide al administrador que verifique que tu usuario esté activo. |
| No abre la página | Verifica que el sistema esté en ejecución y que la dirección sea la correcta. |
| Mi solicitud fue rechazada al enviarla | Revisa que la fecha no sea pasada, que la hora de fin sea posterior a la de inicio y que el laboratorio esté libre en ese horario. |
| No veo una opción del menú | El menú depende de tu rol. Consulta con el administrador. |
