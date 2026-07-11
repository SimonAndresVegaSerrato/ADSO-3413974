
                     MINI SRS - POWERTRACK

Proyecto: POWERTRACK
Autor: Simon Vega
Programa: ADSO - SENA
Fecha: Julio 2026


1. INTRODUCCIÓN:

POWERTRACK es una aplicación web diseñada para facilitar la administración
de gimnasios. El sistema permitirá gestionar usuarios, entrenadores,
rutinas y ejercicios, además de registrar el progreso físico de los
clientes para mejorar el seguimiento de sus objetivos.


2. OBJETIVO GENERAL:

Desarrollar una plataforma web que permita administrar de forma eficiente
la información de un gimnasio, facilitando la creación de rutinas, el
seguimiento del progreso físico y la gestión de usuarios.


3. ALCANCE:

El sistema permitirá:

- Registrar clientes.
- Registrar entrenadores.
- Registrar administradores.
- Iniciar sesión.
- Recuperar contraseña.
- Crear rutinas.
- Editar rutinas.
- Asignar rutinas a clientes.
- Registrar ejercicios.
- Registrar progreso físico.
- Consultar historial.
- Generar reportes.


4. ACTORES:

CLIENTE

- Registrarse.
- Iniciar sesión.
- Consultar rutinas.
- Registrar progreso.
- Editar perfil.

ENTRENADOR

- Crear rutinas.
- Editar rutinas.
- Asignar rutinas.
- Consultar progreso de clientes.

ADMINISTRADOR

- Gestionar usuarios.
- Gestionar entrenadores.
- Gestionar ejercicios.
- Generar reportes.


5. REQUERIMIENTOS FUNCIONALES:

RF01. Registrar usuarios.

RF02. Iniciar sesión.

RF03. Recuperar contraseña.

RF04. Registrar entrenadores.

RF05. Registrar ejercicios.

RF06. Crear rutinas.

RF07. Editar rutinas.

RF08. Asignar rutinas.

RF09. Registrar progreso físico.

RF10. Consultar historial.

RF11. Administrar usuarios.

RF12. Generar reportes.


6. REQUERIMIENTOS NO FUNCIONALES:

RNF01. El sistema responderá en menos de 3 segundos.

RNF02. Las contraseñas estarán cifradas.

RNF03. Compatible con Google Chrome, Microsoft Edge y Firefox.

RNF04. Diseño adaptable para computador, tablet y celular.

RNF05. Disponibilidad mínima del 99%.


7. CASOS DE USO:

CU01 - Registrarse

Actor:
Cliente

Descripción:
Permite crear una nueva cuenta dentro del sistema.

------------------------------------------------------------

CU02 - Iniciar Sesión

Actor:
Cliente

Descripción:
Permite ingresar al sistema mediante correo y contraseña.

------------------------------------------------------------

CU03 - Crear Rutina

Actor:
Entrenador

Descripción:
Permite crear una rutina personalizada.

------------------------------------------------------------

CU04 - Asignar Rutina

Actor:
Entrenador

Descripción:
Permite asignar una rutina a un cliente.

------------------------------------------------------------

CU05 - Registrar Progreso

Actor:
Cliente

Descripción:
Permite registrar peso, medidas y observaciones.

------------------------------------------------------------

CU06 - Administrar Usuarios

Actor:
Administrador

Descripción:
Permite crear, modificar y eliminar usuarios.


8. DIAGRAMA DE CASOS DE USO:

                 POWERTRACK

             +----------------+
             |    Sistema     |
             +----------------+

Cliente

  ─ Registrarse

  ─ Iniciar sesión

  ─ Consultar rutinas

  ─ Registrar progreso

  ─ Editar perfil


Entrenador

  ─ Crear rutina

  ─ Editar rutina

  ─ Asignar rutina

  ─ Consultar progreso


Administrador

  ─ Gestionar usuarios

  ─ Gestionar entrenadores

  ─ Gestionar ejercicios

  ─ Generar reportes


9. DIAGRAMA DE CLASES:

+------------------------------------------------+
|                  Usuario                       |
+------------------------------------------------+
| idUsuario                                      |
| nombre                                         |
| correo                                         |
| contraseña                                     |
| rol                                            |
+------------------------------------------------+
| iniciarSesion()                                |
| cerrarSesion()                                 |
+------------------------------------------------+

                    ▲
                    │
      ┌─────────────┴─────────────┐
      │                           │

+------------------------+   +------------------------+
| Cliente                |   | Entrenador            |
+------------------------+   +------------------------+
| peso                   |   | especialidad          |
| estatura               |   | experiencia           |
+------------------------+   +------------------------+

                    │
                    │ posee
                    ▼

+------------------------------------------------+
|                  Rutina                        |
+------------------------------------------------+
| idRutina                                       |
| nombre                                         |
| descripcion                                    |
| nivel                                          |
+------------------------------------------------+

                    │
                    │ contiene
                    ▼

+------------------------------------------------+
|                Ejercicio                       |
+------------------------------------------------+
| idEjercicio                                    |
| nombre                                         |
| series                                         |
| repeticiones                                   |
+------------------------------------------------+

============================================================
10. CONCLUSIÓN
============================================================

POWERTRACK permitirá mejorar la administración de gimnasios mediante la
automatización de procesos relacionados con usuarios, entrenadores,
rutinas y seguimiento del progreso físico. Esto optimizará el trabajo
administrativo y ofrecerá una mejor experiencia a los clientes.

========================= FIN =========================
