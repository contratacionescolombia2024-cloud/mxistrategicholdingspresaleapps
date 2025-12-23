# MXI Strategic Holdings Presale Apps

Una aplicación React Native construida con Expo para MXI Strategic Holdings.

## 📋 Requisitos Previos

- Node.js (versión 18 o superior)
- npm o yarn
- Expo CLI (se instalará automáticamente)
- Expo Go app en tu dispositivo móvil (opcional para pruebas)

## 🚀 Inicio Rápido

### 1. Instalar Dependencias

```bash
npm install
```

### 2. Iniciar el Servidor de Desarrollo

```bash
npm start
```

Esto abrirá Expo Developer Tools en tu navegador.

### 3. Ejecutar en Diferentes Plataformas

```bash
# Android
npm run android

# iOS (solo en macOS)
npm run ios

# Web
npm run web
```

## 📱 Ejecutar en tu Dispositivo

1. Instala la app **Expo Go** desde:
   - [Google Play Store](https://play.google.com/store/apps/details?id=host.exp.exponent) (Android)
   - [Apple App Store](https://apps.apple.com/app/expo-go/id982107779) (iOS)

2. Ejecuta `npm start` en tu computadora

3. Escanea el código QR que aparece en la terminal o en el navegador:
   - **Android**: Usa la app Expo Go para escanear
   - **iOS**: Usa la cámara del iPhone para escanear

## 🏗️ Estructura del Proyecto

```
mxistrategicholdingspresaleapps/
├── App.js              # Punto de entrada principal de la aplicación
├── app.json            # Configuración de Expo
├── package.json        # Dependencias y scripts
├── babel.config.js     # Configuración de Babel
├── eas.json           # Configuración de Expo Application Services
├── assets/            # Imágenes y recursos estáticos
│   └── README.md      # Instrucciones para los assets
└── README.md          # Este archivo
```

## 🔧 Configuración de Assets

Antes de compilar la aplicación para producción, necesitas agregar los siguientes archivos en la carpeta `assets/`:

- `icon.png` - Ícono de la app (1024x1024 px)
- `splash.png` - Pantalla de inicio
- `adaptive-icon.png` - Ícono adaptativo para Android
- `favicon.png` - Favicon para la versión web

Consulta `assets/README.md` para más detalles.

## 📦 Construir para Producción

### Usando EAS Build (Recomendado)

1. Instala EAS CLI:
```bash
npm install -g eas-cli
```

2. Inicia sesión en Expo:
```bash
eas login
```

3. Configura tu proyecto:
```bash
eas build:configure
```

4. Construye para tu plataforma:
```bash
# Para Android
eas build --platform android

# Para iOS
eas build --platform ios

# Para ambos
eas build --platform all
```

## 📝 Scripts Disponibles

- `npm start` - Inicia el servidor de desarrollo de Expo
- `npm run android` - Ejecuta la app en un emulador/dispositivo Android
- `npm run ios` - Ejecuta la app en un simulador/dispositivo iOS
- `npm run web` - Ejecuta la app en el navegador web

## 🌐 Despliegue

### Web
Para desplegar la versión web:
```bash
npm run web
```

La versión web se puede hospedar en servicios como:
- Netlify
- Vercel
- GitHub Pages
- Firebase Hosting

## 🤝 Contribuir

1. Haz fork del proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto es privado y pertenece a MXI Strategic Holdings.

## 🆘 Soporte

Para problemas o preguntas:
- Abre un issue en GitHub
- Consulta la [documentación de Expo](https://docs.expo.dev/)
- Visita la [comunidad de Expo](https://forums.expo.dev/)

## 🔗 Enlaces Útiles

- [Documentación de Expo](https://docs.expo.dev/)
- [Documentación de React Native](https://reactnative.dev/)
- [Expo Snack](https://snack.expo.dev/) - Prueba código en el navegador