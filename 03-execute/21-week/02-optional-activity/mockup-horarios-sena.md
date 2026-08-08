# Mejoras propuestas al mockup de Gestión de Horarios — SENA

Este documento resume qué le hace falta al mockup y qué cambios se recomiendan para que quede más completo y fácil de usar. Está escrito en lenguaje sencillo, pensado para compartir con el equipo del proyecto.

## Contenido

1. [Pantallas que faltan en el recorrido](#1-pantallas-que-faltan-en-el-recorrido)
2. [Detalles de cumplimiento que se notan en el diseño](#2-detalles-de-cumplimiento-que-se-notan-en-el-diseño)
3. [Que el usuario nunca se sienta perdido](#3-que-el-usuario-nunca-se-sienta-perdido)
4. [Pulido de la página principal](#4-pulido-de-la-página-principal)

---

## 1. Pantallas que faltan en el recorrido

### 🔴 Pantalla de choque de horario
Cuando dos clases se cruzan (mismo instructor, mismo salón, o mismo grupo en dos lugares a la vez), el sistema debería mostrar un aviso claro de que hay un problema. Hoy esa pantalla no existe en el recorrido, y es justamente el caso más importante que un sistema de horarios tiene que resolver.

### 🔴 Pantallas para cuando "no hay nada todavía"
Faltan las pantallas que se ven cuando:
- Un aprendiz nuevo todavía no tiene horario asignado.
- Un coordinador va a armar un horario pero no hay instructores disponibles.
- Una búsqueda no encuentra resultados (por ejemplo, buscar una ficha que no existe).

Son pantallas fáciles de pasar por alto, pero cualquier usuario se las va a encontrar tarde o temprano.

### 🔴 Historial de cambios
Sería útil que cada horario muestre algo simple como: *"Modificado por [nombre] el [fecha]"*. No se trata de armar un sistema de auditoría completo, solo de que quede visible quién cambió qué.

### 🔴 Confirmación antes de guardar cambios importantes
Cuando un coordinador borra o mueve una clase que ya tiene aprendices asignados, debería aparecer un mensaje de confirmación ("¿Seguro que quieres hacer este cambio?"). Hoy no se ve ninguna pantalla de este tipo en el inventario.

### 🟡 Notificaciones al usuario
No se ve ninguna pantalla de avisos o notificaciones (por ejemplo, "tu horario cambió" para un aprendiz, o "te asignaron una nueva clase" para un instructor). Es una pieza que normalmente conecta todos los roles entre sí.

---

## 2. Detalles de cumplimiento que se notan en el diseño

### 🟡 Aviso sobre el manejo de datos personales
En la pantalla de inicio de sesión falta un espacio (una casilla + un enlace) donde se le informe al usuario cómo se van a usar sus datos. No hace falta redactar todo el texto legal ahora, pero sí dejar el espacio diseñado.

### 🟡 Revisar los colores
El verde institucional que se usa en botones y tarjetas debe verificarse para asegurarse de que se lea bien tanto para personas con baja visión como en pantallas de mala calidad. Es una revisión rápida con herramientas gratuitas en línea.

### 🟡 Que se note cuándo algo está seleccionado con el teclado
Ahora mismo, los botones y tarjetas del mockup solo cambian de aspecto cuando se les pasa el mouse por encima (`hover`), pero no cuando se navega usando solo el teclado. Hay que agregar ese detalle visual para que cualquier persona pueda usar el sistema sin necesidad de mouse.

### 🟡 Textos de error fáciles de entender
Si un formulario falla (por ejemplo, un horario mal diseñado), el mensaje de error debería explicar en palabras simples qué pasó y qué hacer, en vez de mostrar un código o un mensaje técnico.

---

## 3. Que el usuario nunca se sienta perdido

### 🟢 Mostrar en qué rol estás
Con 7 roles distintos (coordinador, instructor, aprendiz, etc.), sería bueno tener algo visible en pantalla —un pequeño distintivo o etiqueta— que le recuerde al usuario en qué rol está navegando, en lugar de que esto solo se sepa mirando la dirección web.

### 🟢 Aclarar si el mockup funciona bien en celular
Hay 45 capturas pensadas para celular, pero no queda claro si uno puede navegar el mockup real desde un celular o si esas capturas son solo imágenes de referencia. Conviene aclararlo para no generar expectativas equivocadas.

### 🟢 Migas de pan o "dónde estoy"
En un sistema con tantas pantallas, ayuda mostrar la ruta actual (por ejemplo: Horarios > Ficha 3413974 > Editar) para que el usuario sepa cómo volver atrás sin perderse.

### 🟢 Buscador visible
Con 53 pantallas y varios roles, un buscador general (por ficha, instructor o ambiente) ayudaría mucho a moverse rápido, y hoy no aparece mencionado.

---

## 4. Pulido de la página principal

### 🟢 Enlace directo al listado de pantallas por rol
Ahora mismo solo hay un botón genérico de "Índice". Ayudaría tener un enlace que lleve directo al listado de las 53 pantallas organizado por rol.

### 🟢 Separar mejor los dos bloques de accesos
En la página principal hay dos secciones que se ven muy parecidas: la de accesos generales y la de "entrar directo por rol". Convendría diferenciarlas visualmente para que quede claro cuál usar primero.

### 🟢 Nota de advertencia más visible
La nota amarilla sobre datos ficticios y documentación privada podría ir acompañada de un ícono, para que se distinga de un simple párrafo de texto y llame más la atención.

### 🟢 Créditos con más peso visual
El nombre del autor y el repositorio están en letra muy pequeña al final; si el mockup se va a compartir con evaluadores externos, vale la pena darle un poco más de peso visual a esos créditos.

