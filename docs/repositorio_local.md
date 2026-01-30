---

# Cómo crear un repositorio local con comandos de Git

## 📌 ¿Qué es un repositorio local?

Un **repositorio local** es una carpeta en tu computadora que está controlada por **Git**, lo que permite guardar versiones del proyecto, registrar cambios y volver a estados anteriores si es necesario.

---

## 🛠️ Pasos para crear un repositorio local

### 1️⃣ Abrir la consola

Abre **Git Bash** (en Windows) o la **terminal** (en Linux/macOS).

---

### 2️⃣ Crear o entrar a la carpeta del proyecto

Si la carpeta **no existe**, créala:

```bash
mkdir mi_proyecto
```

Entra a la carpeta:

```bash
cd mi_proyecto
```

📌 Puedes verificar tu ubicación con:

```bash
pwd
```

---

### 3️⃣ Inicializar el repositorio Git

Dentro de la carpeta del proyecto, ejecuta:

```bash
git init
```

✔ Este comando:

* Crea la carpeta oculta `.git`
* Convierte el directorio en un repositorio local

La consola mostrará algo como:

```
Initialized empty Git repository
```

---

### 4️⃣ Crear archivos en el repositorio

Por ejemplo:

```bash
touch README.md
```

O cualquier archivo del proyecto:

```bash
touch main.py
```

---

### 5️⃣ Ver el estado del repositorio

```bash
git status
```

Este comando muestra:

* Archivos sin seguimiento
* Archivos listos para guardar
* Estado general del repositorio

---

### 6️⃣ Agregar archivos al área de preparación (staging)

Agregar un archivo específico:

```bash
git add README.md
```

Agregar todos los archivos:

```bash
git add .
```

---

### 7️⃣ Guardar los cambios (commit)

```bash
git commit -m "Primer commit del proyecto"
```

✔ El commit guarda una **instantánea del proyecto**.

---

## 📋 Comandos principales usados

| Comando      | Función                    |
| ------------ | -------------------------- |
| `git init`   | Inicializa el repositorio  |
| `git status` | Muestra el estado          |
| `git add`    | Agrega archivos al staging |
| `git commit` | Guarda los cambios         |
| `pwd`        | Muestra la ruta actual     |
| `ls`         | Lista archivos             |
| `cd`         | Cambia de directorio       |
| `mkdir`      | Crea carpetas              |
| `touch`      | Crea archivos              |

---

## ✅ Conclusión

Crear un repositorio local con Git es un proceso sencillo que permite:

* Controlar versiones del proyecto
* Organizar el desarrollo
* Preparar el proyecto para subirlo a GitHub u otro repositorio remoto
