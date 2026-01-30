---

# Proceso para crear un repositorio remoto en GitHub

## 📌 ¿Qué es un repositorio remoto?

Un **repositorio remoto** es un repositorio que se aloja en **GitHub** y permite:

* Guardar el proyecto en la nube
* Compartir código
* Trabajar en equipo
* Tener respaldo del proyecto

---

## 🛠️ Pasos para crear un repositorio remoto

### 1️⃣ Crear una cuenta en GitHub

Si aún no tienes cuenta:

* Entra a **github.com**
* Regístrate con correo y contraseña

---

### 2️⃣ Iniciar sesión en GitHub

OAOAOAOAOAAccede a tu cuenta desde el navegador.

---
OAOAOAOAOA
### 3️⃣ Crear un nuevo repositorio

1. En la esquina superior derecha, haz clic en el botón **“+”**
OAOAOAOAOA2. Selecciona **“New repository”**

---

### 4️⃣ Configurar el repositorio

Completa los siguientes campos:

* **Repository name**: nombre del proyecto
  Ejemplo: `mi-primer-repo`
* **Description** (opcional): breve explicación del proyecto
* **Public / Private**: elegir visibilidad
* ❌ **NO marques** “Add a README file” (si ya tienes uno local)
* ❌ **NO marques** `.gitignore` ni `license` (si ya existen localmente)

---

### 5️⃣ Crear el repositorio

Haz clic en **“Create repository”**.

GitHub mostrará una página con instrucciones y la URL del repositorio.

---

## 🔗 Conectar el repositorio local con GitHub

### 6️⃣ Copiar la URL del repositorio

Ejemplo:

```
https://github.com/usuario/mi-primer-repo.git
```

---

### 7️⃣ Agregar el repositorio remoto

Desde la carpeta del proyecto local:

```bash
git remote add origin https://github.com/usuario/mi-primer-repo.git
```

Verifica:

```bash
git remote -v
```

---

### 8️⃣ Subir el proyecto a GitHub

```bash
git branch -M main
git push -u origin main
```

✔ Esto sube el contenido local al repositorio remoto.

---

## 📋 Comandos principales usados

| Comando                 | Función                          |
| ----------------------- | -------------------------------- |
| `git remote add origin` | Conecta el repo local con GitHub |
| `git remote -v`         | Verifica el remoto               |
| `git branch -M main`    | Define rama principal            |
| `git push`              | Envía cambios a GitHub           |

---

## ⚠️ Errores comunes

* ❌ Crear README en GitHub y también local → conflictos
* ❌ URL incorrecta
* ❌ No tener commits antes de hacer `push`
* ❌ No tener permisos del repositorio

---

## ✅ Conclusión

Crear un repositorio remoto en GitHub permite centralizar el proyecto, compartirlo y trabajar de forma profesional. Una vez conectado, el flujo normal de trabajo es:

```bash
git add .
git commit -m "Mensaje"
git push
```
