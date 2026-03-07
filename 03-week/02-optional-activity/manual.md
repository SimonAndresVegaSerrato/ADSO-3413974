# Manual de Git desde la Terminal

## 1. ¿Qué es Git?

Git es un sistema de control de versiones distribuido que permite registrar los cambios realizados en archivos a lo largo del tiempo.

Es ampliamente utilizado en el desarrollo de software porque permite:

- Guardar el historial de cambios de un proyecto.
- Trabajar en equipo sin sobrescribir archivos.
- Recuperar versiones anteriores del código.
- Crear diferentes líneas de desarrollo mediante ramas.

Git es una herramienta fundamental en el desarrollo moderno porque facilita la colaboración entre programadores y el control del código fuente.

---

## 2. Instalación de Git

### Windows

1. Ir al sitio oficial de Git: https://git-scm.com  
2. Descargar **Git for Windows**  
3. Ejecutar el instalador.  
4. Instalar con las opciones por defecto.

### Linux (Ubuntu / Debian)

Instalar Git desde la terminal:

```bash
sudo apt update
sudo apt install git
```

### MacOS

Si se utiliza Homebrew:

```bash
brew install git
```

### Verificar la instalación

Para comprobar que Git se instaló correctamente:

```bash
git --version
```

Ejemplo de salida:

```
git version 2.42.0
```

---

## 3. Configuración Inicial

Antes de usar Git por primera vez es necesario configurar el nombre y el correo electrónico.  
Esta información se asociará a cada cambio guardado en el repositorio.

Configurar nombre de usuario:

```bash
git config --global user.name "Tu Nombre"
```

Configurar correo electrónico:

```bash
git config --global user.email "tuemail@gmail.com"
```

Ver toda la configuración actual:

```bash
git config --list
```

---

## 4. Crear un Repositorio

Un **repositorio** es el espacio donde Git guarda todos los cambios de un proyecto.

Para crear un repositorio nuevo:

```bash
git init
```

Este comando crea una carpeta oculta llamada:

```
.git
```

Esta carpeta contiene todo el historial del proyecto.

---

## 5. Estados de los Archivos en Git

Git maneja tres áreas principales para el control de archivos.

| Área | Descripción |
|-----|-------------|
| Working Directory | Archivos del proyecto |
| Staging Area | Archivos preparados para guardar |
| Repository | Historial del proyecto |

Flujo de trabajo básico:

```
Modificar archivo
      ↓
git add
      ↓
git commit
```

---

## 6. Ver el Estado del Proyecto

Para revisar el estado actual del repositorio:

```bash
git status
```

Este comando muestra:

- Archivos modificados.
- Archivos listos para guardar.
- Archivos que Git aún no está siguiendo.

---

## 7. Agregar Archivos al Staging

Antes de guardar los cambios, los archivos deben agregarse al área de preparación.

Agregar un archivo específico:

```bash
git add archivo.txt
```

Agregar todos los archivos del proyecto:

```bash
git add .
```

---

## 8. Guardar Cambios (Commit)

Un **commit** representa un punto de guardado en el historial del proyecto.

Guardar cambios:

```bash
git commit -m "mensaje del cambio"
```

Ejemplo:

```bash
git commit -m "Agrega sistema de autenticación"
```

El mensaje debe describir claramente qué cambio se realizó.

---

## 9. Ver Historial de Cambios

Para ver todos los commits realizados:

```bash
git log
```

Versión resumida:

```bash
git log --oneline
```

Esto muestra cada commit en una sola línea.

---

## 10. Ver Cambios en los Archivos

Para ver las diferencias entre archivos modificados y la última versión guardada:

```bash
git diff
```

Ver cambios de un archivo específico:

```bash
git diff archivo.txt
```

---

## 11. Trabajar con Ramas

Las **ramas** permiten desarrollar nuevas funciones sin afectar la versión principal del proyecto.

Ver ramas existentes:

```bash
git branch
```

Crear una nueva rama:

```bash
git branch nueva-rama
```

Cambiar a una rama:

```bash
git checkout nueva-rama
```

Crear y cambiar a una rama en un solo comando:

```bash
git checkout -b nueva-rama
```

---

## 12. Unir Ramas (Merge)

Para combinar los cambios de una rama con la rama principal:

Primero cambiar a la rama principal:

```bash
git checkout main
```

Luego unir la rama:

```bash
git merge nueva-rama
```

Esto integra los cambios de ambas ramas.

---

## 13. Repositorios Remotos

Los repositorios remotos permiten almacenar el proyecto en servidores externos y colaborar con otros desarrolladores.

Los servicios más comunes son:

- GitHub
- GitLab
- Bitbucket

---

## 14. Clonar un Repositorio

Clonar significa copiar un repositorio remoto a tu computadora.

```bash
git clone URL_DEL_REPOSITORIO
```

Ejemplo:

```bash
git clone https://github.com/usuario/proyecto.git
```

---

## 15. Conectar un Repositorio Local con uno Remoto

Agregar un repositorio remoto:

```bash
git remote add origin URL
```

Ver repositorios remotos configurados:

```bash
git remote -v
```

---

## 16. Subir Cambios al Repositorio Remoto

Enviar cambios al repositorio remoto:

```bash
git push origin main
```

---

## 17. Descargar Cambios del Repositorio Remoto

Para actualizar el repositorio local con cambios del remoto:

```bash
git pull origin main
```

---

## 18. Flujo de Trabajo Básico

Ejemplo de flujo de trabajo típico con Git:

Inicializar repositorio:

```bash
git init
```

Agregar archivos:

```bash
git add .
```

Guardar cambios:

```bash
git commit -m "primer commit"
```

Conectar repositorio remoto:

```bash
git remote add origin URL
```

Subir proyecto:

```bash
git push -u origin main
```

Después de esto el flujo normal es:

```bash
git add .
git commit -m "nuevo cambio"
git push
```

---

## 19. Comandos Más Usados

| Comando | Función |
|--------|--------|
| git init | Crear repositorio |
| git status | Ver estado del proyecto |
| git add | Preparar archivos |
| git commit | Guardar cambios |
| git log | Ver historial |
| git branch | Ver ramas |
| git checkout | Cambiar de rama |
| git merge | Unir ramas |
| git push | Subir cambios |
| git pull | Descargar cambios |

---

## 20. Buenas Prácticas

Para trabajar correctamente con Git se recomienda:

- Hacer commits pequeños y frecuentes.
- Escribir mensajes de commit claros.
- Crear ramas para nuevas funciones.
- Actualizar el repositorio antes de trabajar.
- No subir contraseñas o archivos sensibles.
- Utilizar un archivo `.gitignore`.

---

## 21. Archivo .gitignore

El archivo `.gitignore` permite excluir archivos o carpetas del control de versiones.

Ejemplo:

```
node_modules/
.env
*.log
dist/
```

Esto evita que Git guarde archivos innecesarios.

---

## 22. Estructura Típica de un Proyecto con Git

Ejemplo de estructura de un proyecto:

```
mi-proyecto/
│
├── src/
├── docs/
├── README.md
├── .gitignore
└── .git
```

La carpeta `.git` contiene toda la información del historial del repositorio.

---

## Fin del manual