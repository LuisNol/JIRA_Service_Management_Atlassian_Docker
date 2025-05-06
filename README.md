# JIRA Service Management con Docker

Este repositorio permite desplegar Atlassian JIRA Service Management usando Docker y Docker Compose en sistemas Linux.

## Requisitos
- Sistema operativo Linux
- Acceso a una terminal con permisos de superusuario
- Git
## Instalación
### 1. Instalar Docker
```bash
curl -fsSL https://get.docker.com | sudo sh
```
### 2. Descargar Docker Compose
```bash
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
docker-compose --version
```
### 3. Clonar el repositorio

```bash
git clone https://github.com/LuisNol/JIRA_Service_Management_Atlassian_Docker.git
cd JIRA_Service_Management_Atlassian_Docker
```
### 4. Ejecutar el contenedor
```bash
docker-compose up --build
```
Esto iniciará los servicios necesarios para JIRA Service Management en tu máquina local.

## Notas
- Este entorno está pensado para desarrollo o pruebas locales.
- Asegúrate de tener suficientes recursos (CPU, RAM, y disco) antes de ejecutar los contenedores.
