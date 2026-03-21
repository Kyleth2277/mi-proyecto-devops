# mi-proyecto-devops
## Descripción del proyecto

En esta actividad, el estudiante implementará un flujo básico de DevOps utilizando Git y GitHub, simulando el desarrollo, mantenimiento y despliegue de un proyecto web estático.
Debido a que actualmente no se cuenta con acceso a AWS Academy, el despliegue será simulado mediante scripts locales y control de versiones en GitHub.

## Objetivo

Al finalizar la actividad, el alumno será capaz de:

    Configurar Git en su equipo local
    Crear y administrar un repositorio en GitHub
    Aplicar buenas prácticas de control de versiones
    Trabajar con ramas (branches)
    Simular un flujo DevOps sin servicios en la nube
    Documentar un proyecto de software

## Estructura del repositorio

mi-proyecto-devops/
│── src/
│   ├── index.html
│   ├── styles.css
│── scripts/
│   └── deploy.sh
│── README.md
│── .gitignore

## Flujo de trabajo:

Parte 1: Configuración inicial
git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@example.com"
Crea un repositorio en GitHub llamado mi-proyecto-devops y clónalo:

git clone https://github.com/TU-USUARIO/mi-proyecto-devops.git
cd mi-proyecto-devops
Parte 2: Creación del proyecto
Crea la estructura de carpetas y archivos indicada anteriormente.

Contenido base del archivo index.html:

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Proyecto DevOps</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Proyecto DevOps con GitHub</h1>
    <p>Este sitio forma parte de una práctica de control de versiones.</p>
</body>
</html>
Parte 3: Primer commit
git add .
git commit -m "Estructura inicial del proyecto"
git push origin main
Parte 4: Simulación de despliegue
Crea el archivo scripts/deploy.sh con el siguiente contenido:

#!/bin/bash
echo "Simulando despliegue del sitio web..."
echo "Archivos listos para producción"
Da permisos de ejecución y ejecútalo:

chmod +x scripts/deploy.sh
./scripts/deploy.sh
Realiza el commit:

git add scripts/deploy.sh
git commit -m "Script de despliegue simulado"
git push origin main
Parte 5: Trabajo con ramas
git checkout -b feature-update
Agrega una nueva sección al archivo index.html:

<p>Este proyecto utiliza GitHub como plataforma DevOps.</p>
git add src/index.html
git commit -m "Nueva sección agregada"
git push origin feature-update


## Comandos Git principales

git commit
git push origin

chmod +x scripts/deploy.sh
./scripts/deploy.sh
git add
git clone
git config