# 🚀 Guía Rápida: Lanzar con Expo

## Para Usuarios que tienen la App de Natively.dev

Si ya descargaste tu aplicación desde natively.dev, sigue estos pasos:

### Opción 1: Reemplazar el Código Base (Recomendado)

1. **Descarga tu app desde natively.dev**
   ```bash
   # Descarga y extrae el ZIP de tu app
   ```

2. **Clona este repositorio**
   ```bash
   git clone https://github.com/contratacionescolombia2024-cloud/mxistrategicholdingspresaleapps.git
   cd mxistrategicholdingspresaleapps
   ```

3. **Reemplaza los archivos (conserva .git y .gitignore)**
   ```bash
   # Copia todos los archivos de tu app descargada aquí
   # EXCEPTO la carpeta .git
   ```

4. **Instala dependencias**
   ```bash
   npm install
   ```

5. **Prueba la app**
   ```bash
   npm start
   # o
   expo start
   ```

6. **Sube a GitHub**
   ```bash
   git add .
   git commit -m "Importar app desde natively.dev"
   git push
   ```

### Opción 2: Usar la Plantilla Actual

Si quieres usar la plantilla Expo que ya está configurada:

1. **Clona el repositorio**
   ```bash
   git clone https://github.com/contratacionescolombia2024-cloud/mxistrategicholdingspresaleapps.git
   cd mxistrategicholdingspresaleapps
   ```

2. **Instala dependencias**
   ```bash
   npm install
   ```

3. **Inicia Expo**
   ```bash
   npm start
   ```

4. **Modifica la app según tus necesidades**
   - Edita `App.js` para cambiar la interfaz
   - Actualiza `app.json` con tu configuración
   - Agrega tus assets en la carpeta `assets/`

## 📱 Ejecutar en tu Dispositivo

### Android o iOS

1. Instala **Expo Go** desde tu tienda de apps
2. Ejecuta `npm start` en tu computadora
3. Escanea el código QR con tu dispositivo

### Navegador Web

```bash
npm run web
```

## 🔨 Construir para Producción

### Con Expo Application Services (EAS)

```bash
# Instalar EAS CLI
npm install -g eas-cli

# Login
eas login

# Configurar proyecto
eas build:configure

# Construir para Android
eas build --platform android

# Construir para iOS (requiere cuenta de Apple Developer)
eas build --platform ios
```

## 📋 Checklist Antes de Lanzar

- [ ] ¿Instalaste las dependencias? (`npm install`)
- [ ] ¿La app inicia correctamente? (`npm start`)
- [ ] ¿Agregaste tus assets (icon.png, splash.png)?
- [ ] ¿Configuraste app.json con tu información?
- [ ] ¿Probaste en al menos un dispositivo?
- [ ] ¿Subiste todo a GitHub? (`git push`)

## 🆘 Problemas Comunes

### "Cannot find module 'expo'"
```bash
npm install
```

### La app no se conecta
```bash
# Limpia la caché
expo start -c
```

### Error con assets
Asegúrate de que los archivos referenciados en `app.json` existan en la carpeta `assets/`

## 📚 Más Información

- **README.md** - Documentación completa del proyecto
- **SETUP_GUIDE.md** - Guía detallada de configuración
- [Documentación de Expo](https://docs.expo.dev/)
- [Natively.dev Docs](https://natively.dev/docs)

---

¿Tienes preguntas? Abre un issue en GitHub o consulta la documentación oficial.
