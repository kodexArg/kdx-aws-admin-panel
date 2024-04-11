# KDX-AWS-Admin-Panel

Bienvenido al proyecto KDX-AWS-Admin-Panel! Esta aplicación sirve una página diseñada para simplificar las tareas de gestión de la nube para instancias AWS EC2. Funciona como una interfaz que permite a los usuarios iniciar o detener instancias EC2 con facilidad, e incluso programar estas tareas para una mejor automatización y eficiencia.

Este proyecto está especialmente diseñado para usuarios sin acceso a sistemas complicados, que sólo necesitan una interfaz sencilla para gestionar estas instancias dentro de su organización.

### Características

- **Gestión de Instancias EC2**: Inicia o detén tus instancias EC2 directamente desde la interfaz web.
- **Programación**: Planifica tus instancias para que se inicien o detengan en momentos específicos, optimizando el uso de recursos y reduciendo costos.
- **Notificaciones**: (Próximamente) Recibe actualizaciones sobre el estado de tus instancias EC2 a través de notificaciones de Telegram.

### Tecnologías

- **Frontend**: HTMX para interactividad dinámica sin necesidad de recargar la página.
- **Backend**: [FastAPI](https://fastapi.tiangolo.com/) para la creación de APIs con Python, ofreciendo una solución de alto rendimiento para el backend.
- **SDK de AWS**: [Boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) para la interacción con AWS, permitiendo gestionar servicios de AWS directamente desde la aplicación.
- **Notificaciones**: (Planificado) [python-telegram-bot](https://python-telegram-bot.org/) para enviar alertas y actualizaciones.

```
.
├── app.py
├── static
│   ├── css
│   │   └── tailwind.min.css
│   └── js
│       └── htmx.js
└── templates
    └── index.html
```

### Configuración del Entorno

Configura varias variables de entorno para manejar la autenticación de AWS de manera segura. Crea un archivo `.env` en la raíz del proyecto como sigue:

```
AWS_ACCESS_KEY_ID=tu_aws_access_key_id
AWS_SECRET_ACCESS_KEY=tu_aws_secret_access_key
AWS_DEFAULT_REGION=tu_region_de_aws
```

**Nota**: Reemplaza los valores con tus propias credenciales de AWS, que deben tener los permisos mínimos para iniciar, apagar y consultar las EC2 que necesitas modificar.

## TODO:
[ ] Json para el usuario de AWS
[ ] Implementar python-telegram-bot
[ ] Implementar HTMX para interactividad en el frontend


## Contribuir

El KDX-AWS-Admin-Panel es un proyecto abierto, y las contribuciones son bienvenidas.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para detalles.
