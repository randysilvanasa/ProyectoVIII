# Regina’s Daycare Backend

Backend del sitio web **Regina’s Daycare**, desarrollado con Node.js, Express, MongoDB y Nodemailer.

## Funcionalidad
- Recibe datos del formulario de contacto.
- Envía correo de notificación.
- Guarda los mensajes en MongoDB Atlas.

## Instalación
```bash
git clone https://github.com/TU-USUARIO/reginasdaycare-backend.git
cd reginasdaycare-backend
npm install
```

Crea el archivo `.env` con tus variables:
```
PORT=5000
MONGO_URI=TU_URL_DE_MONGODB_ATLAS
EMAIL_USER=tu_correo@gmail.com
EMAIL_PASS=tu_contraseña_de_aplicacion
```

## Ejecutar
```bash
npm run dev
```

El servidor se ejecuta en:
```
http://localhost:5000
```

## Endpoint
POST `/api/contact`
```json
{
  "name": "Juan Pérez",
  "email": "juan@example.com",
  "message": "Hola, quiero información."
}
```

### Respuesta
```json
{
  "success": "Mensaje enviado y guardado con éxito"
}
```


