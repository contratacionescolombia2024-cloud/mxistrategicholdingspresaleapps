# Guía de Configuración - MXI Strategic Holdings Presale Apps

## 📦 Cómo Reemplazar esta Plantilla con tu App de Natively.dev

Si descargaste una aplicación desde natively.dev y quieres subirla a este repositorio, sigue estos pasos:

### 1. Descargar tu App desde Natively.dev

1. Ve a [natively.dev](https://natively.dev)
2. Descarga el código fuente de tu aplicación
3. Extrae el archivo ZIP en tu computadora

### 2. Reemplazar los Archivos del Proyecto

**Importante**: Antes de reemplazar archivos, asegúrate de revisar qué archivos tiene tu app de natively.dev.

#### Archivos que debes mantener de este repositorio:
- `.git/` (carpeta - NO la elimines)
- `.gitignore`
- `README.md` (opcional, puedes modificarlo)

#### Archivos que probablemente reemplazarás:
- `package.json` - Reemplázalo con el de tu app
- `App.js` o `app.tsx` - Reemplázalo con el de tu app
- `app.json` - Reemplázalo con el de tu app
- `babel.config.js` - Reemplázalo si tu app tiene uno
- `assets/` - Reemplázala con tus assets

#### Pasos de Reemplazo:

```bash
# 1. Navega a la carpeta de este repositorio
cd /ruta/a/mxistrategicholdingspresaleapps

# 2. Copia los archivos de tu app descargada (excepto .git)
# Opción A: Manualmente copia los archivos
# Opción B: Usa comandos (ejemplo en Linux/Mac)
cp -r /ruta/a/tu-app-natively/* .

# 3. Asegúrate de mantener .gitignore
# Si se sobreescribió, revisa que incluya las exclusiones necesarias

# 4. Revisa los cambios
git status

# 5. Agrega los cambios
git add .

# 6. Haz commit
git commit -m "Importar app desde natively.dev"

# 7. Sube a GitHub
git push origin main  # o la rama que estés usando
```

### 3. Actualizar Dependencias

Después de copiar los archivos:

```bash
# Instala las dependencias
npm install

# O si usa yarn
yarn install
```

### 4. Probar la Aplicación

```bash
# Inicia el servidor de desarrollo
npm start

# O
expo start
```

### 5. Configuración Adicional

#### Si tu app usa Expo (recomendado):
- Verifica que `app.json` esté configurado correctamente
- Actualiza el `slug`, `name` y otros campos según tu app

#### Si tu app usa React Native CLI (sin Expo):
- Necesitarás carpetas `android/` e `ios/`
- Sigue las instrucciones específicas de React Native CLI

### 6. Assets e Iconos

Asegúrate de incluir:
- `assets/icon.png` (1024x1024 px)
- `assets/splash.png` (para splash screen)
- `assets/adaptive-icon.png` (para Android)

Puedes generar estos assets con:
- [App Icon Generator](https://appicon.co/)
- [Expo Asset Tools](https://docs.expo.dev/guides/app-icons/)

### 7. Configuración de EAS (Expo Application Services)

Si quieres compilar tu app:

```bash
# Instalar EAS CLI
npm install -g eas-cli

# Login
eas login

# Configurar
eas build:configure

# Construir
eas build --platform android
# o
eas build --platform ios
```

## 🚨 Problemas Comunes

### Error: "Cannot find module..."
**Solución**: Ejecuta `npm install` para instalar todas las dependencias

### Error con Assets
**Solución**: Verifica que todos los assets referenciados en `app.json` existan

### Error al iniciar Expo
**Solución**: 
1. Limpia caché: `expo start -c`
2. Reinstala dependencias: `rm -rf node_modules && npm install`

### Conflictos de Git
**Solución**: Si tienes conflictos al hacer push, consulta con tu equipo antes de forzar cambios

## 📞 Ayuda

Si necesitas ayuda adicional:
- Revisa la [documentación de Expo](https://docs.expo.dev/)
- Consulta el [foro de Expo](https://forums.expo.dev/)
- Lee la documentación de [natively.dev](https://natively.dev/docs)

## ✅ Checklist Final

Antes de compartir tu app, verifica:

- [ ] Instalaste las dependencias (`npm install`)
- [ ] La app inicia sin errores (`npm start`)
- [ ] Todos los assets están presentes
- [ ] Actualizaste el README.md con información de tu app
- [ ] El `app.json` tiene la configuración correcta
- [ ] Probaste la app en al menos un dispositivo/emulador
- [ ] Hiciste commit de todos los cambios importantes
- [ ] Subiste los cambios a GitHub (`git push`)
