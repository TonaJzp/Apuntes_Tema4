# Comandos básicos de Git

## ¿Qué es Git?
Git es un sistema de control de versiones que permite gestionar cambios en el código fuente de forma distribuida.

## Comandos principales

| Comando | Descripción |
|--------|-------------|
| `git init` | Inicia un repositorio local |
| `git clone` | Clona un repositorio remoto |
| `git status` | Muestra el estado del repositorio |
| `git add` | Añade archivos al área de staging |
| `git commit` | Guarda los cambios |
| `git push` | Sube los cambios al remoto |
| `git pull` | Trae cambios del remoto |
| `git branch` | Lista o crea ramas |
| `git checkout` | Cambia de rama |
| `git merge` | Fusiona ramas |

## Ejemplo de uso

```bash
git init
git add .
git commit -m "Primer commit"
git remote add origin URL
git push -u origin main
 
