# Talonario de Rifa Digital

Una aplicación web moderna para gestionar talonarios de rifa con sincronización en tiempo real entre pestañas.

## 🚀 Características

- **Interfaz moderna y responsive**: Diseño optimizado para dispositivos móviles y escritorio
- **Sincronización en tiempo real**: Los números seleccionados se sincronizan automáticamente entre todas las pestañas abiertas
- **Almacenamiento local**: Las reservas se guardan localmente en el navegador
- **Notificaciones visuales**: Feedback inmediato para las acciones del usuario
- **Validación de datos**: Formulario completo con validación de campos requeridos

## 📱 Uso

1. Abre la aplicación en tu navegador
2. Selecciona los números que deseas reservar haciendo clic en ellos
3. Completa el formulario con tus datos personales
4. Haz clic en "Reservar Números" para confirmar tu selección
5. Los números reservados se mostrarán en rojo y se sincronizarán automáticamente

## 🔄 Sincronización

La aplicación utiliza **BroadcastChannel API** para sincronizar los datos entre pestañas:

- Los números seleccionados se actualizan en tiempo real
- Las reservas se comparten automáticamente entre todas las pestañas
- El estado de sincronización se muestra en la parte superior de la aplicación

## 🌐 Despliegue en GitHub Pages

### Configuración automática

1. Sube este proyecto a un repositorio de GitHub
2. Ve a **Settings** > **Pages** en tu repositorio
3. En **Source**, selecciona "GitHub Actions"
4. El workflow automático desplegará la aplicación

### URL de acceso

Una vez configurado, tu aplicación estará disponible en:
```
https://tu-usuario.github.io/nombre-del-repositorio
```

## 🛠️ Tecnologías utilizadas

- HTML5
- CSS3 (Flexbox, Grid, Gradientes)
- JavaScript ES6+
- BroadcastChannel API
- LocalStorage API

## 📋 Estructura del proyecto

```
├── index.html          # Aplicación principal
├── .github/
│   └── workflows/
│       └── deploy.yml  # Workflow de GitHub Actions
└── README.md          # Este archivo
```

## 🔧 Desarrollo local

Para ejecutar la aplicación localmente:

```bash
# Opción 1: Servidor HTTP simple con Python
python -m http.server 8080

# Opción 2: Servidor HTTP simple con Node.js
npx http-server

# Opción 3: Live Server (VS Code extension)
# Instala la extensión "Live Server" y haz clic derecho > "Open with Live Server"
```

Luego abre `http://localhost:8080` en tu navegador.

## 📝 Notas importantes

- La sincronización funciona solo entre pestañas del mismo dominio
- Los datos se almacenan localmente en cada navegador
- Para sincronización entre dispositivos, se requiere implementar un backend
- La aplicación es completamente funcional sin conexión a internet

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.