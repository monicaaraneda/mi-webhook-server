# Servidor de Webhooks en Node.js

Este proyecto es un servidor simple implementado en Node.js usando Express, diseñado para recibir y procesar webhooks. Puede ser utilizado como base para integrar diversas APIs que envían eventos en tiempo real.

## Características

- **Recepción de Webhooks**: Capaz de recibir solicitudes HTTP POST con datos JSON.
- **Logging**: Registra los detalles de cada webhook recibido en la consola.

## Requisitos

Para ejecutar este servidor necesitas tener instalado [Node.js](https://nodejs.org/) y npm (viene con Node.js). Asegúrate de que tu versión de Node.js sea la 12.x o superior.

## Instalación

Sigue estos pasos para configurar el servidor de webhooks en tu entorno local:

1. **Clona este repositorio**:
   ```bash
   git clone https://tu-repositorio.com/mi-webhook-server.git
   cd mi-webhook-server
   ``` 
2. **Instala las dependencias:
    ```bash
      npm install
    ```
3. **Inicia el servidor:
    ```bash
       npm start
      ```
Esto arrancará el servidor en http://localhost:3000.

4. **Para enviar un webhook al servidor, puedes usar curl o cualquier herramienta de prueba de API como Postman.

Ejemplo de solicitud con curl:
```bash
       curl -X POST http://localhost:3000/webhook -H "Content-Type: application/json" -d '{"message": "Hola, mundo!"}'
 ```
Respuesta esperada:
Si el webhook se recibe correctamente, el servidor responderá con:
```bash
        Webhook recibido
 ```
