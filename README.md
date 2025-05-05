# Mailer-App

Una aplicación sencilla para enviar correos y visualizarlos.

## Tecnologías Usadas

- Python
- Flask
- MySQL
- Docker
- HTML5
- CSS3
- SendGrid

## Requisitos Técnicos

Para ejecutar la aplicación es necesario cumplir los siguientes requisitos:

- Docker para la ejecución de la aplicación y base de datos.
- Una cuenta en SendGrid para poder enviar correos.

## Descripción

Aplicación web que permite enviar correos utilizando la API de SendGrid y que una vez enviados se pueden visualizar los correos junto a su respectivo detalle.

## Pasos para ejecutar

1. Crear una cuenta en SendGrid, luego de acceder al Dashboard, ir a **Settings>API Keys>Create API Key**, una vez creada la clave copiarla en la variable de entorno **SENDGRID_API_KEY** en el archivo **docker-compose.yml**.

2. Ingresar tu correo a utilizar en la variable de entorno **FROM_EMAIL**, este correo debe ser el mismo que registraste para utilizar en SendGrid. Además debes ingresar un valor para la variable de entorno **SECRET_KEY**.

3. **Clonar el repositorio** del proyecto en tu máquina local:
   ```bash
   git clone https://github.com/MarcoAntonioRG/Mailer-App.git
   ```

4. Ejecutar microservicio con:
   ```bash
   docker-compose up --build