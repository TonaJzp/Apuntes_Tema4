 # Comandos básicos de Git

## ¿Qué es Git?

Git es un sistema de control de versiones que permite gestionar cambios en el código fuente de forma distribuida. Facilita el trabajo en equipo, la creación de ramas, el control de versiones y la colaboración en proyectos de desarrollo.

---

## 🧰 Comandos fundamentales de Git

| Comando | Descripción |
|--------|-------------|
| `git init` | Inicia un nuevo repositorio local |
| `git status` | Muestra el estado de los archivos |
| `git add .` | Añade todos los cambios al área de preparación (staging) |
| `git commit -m "mensaje"` | Guarda los cambios localmente con un mensaje |
| `git log` | Muestra el historial de commits |
| `git branch` | Lista todas las ramas locales |
| `git checkout -b nombre-rama` | Crea una nueva rama y cambia a ella |
| `git merge nombre-rama` | Fusiona una rama con la actual |
| `git remote add origin URL` | Conecta el repo local con GitHub |
| `git push -u origin main` | Sube los cambios al repositorio remoto |

---

## 🌿 Flujo de trabajo básico

```bash
git init
git add .
git commit -m "Primer commit"
git branch -M main
git remote add origin https://github.com/usuario/repositorio.git
git push -u origin main

