# CheckOut

Aplicación móvil inteligente para prevenir el olvido de objetos personales al salir de casa.

## 🛠️ Tecnologías

- React Native
- JavaScript/TypeScript
- GPS/Geolocalización
- OpenWeather API

## 👥 Reglas de Colaboración

### Flujo de Ramas (GitHub Flow)

Este proyecto usa **GitHub Flow** simplificado para equipos pequeños:

#### Ramas Principales

- **`main`**: Rama principal protegida. Siempre debe estar en estado deployable.
  - ❌ NO se permite push directo
  - ✅ Requiere 1 revisión aprobada antes de merge
  - ✅ Requiere que pasen los checks de CI/CD

#### Ramas de Trabajo

- **`feature/nombre-funcionalidad`**: Para nuevas funcionalidades
  - Ejemplo: `feature/geofencing`, `feature/weather-api`
  
- **`fix/descripcion-bug`**: Para correcciones de bugs
  - Ejemplo: `fix/battery-drain`, `fix/crash-android`

### Proceso de Pull Request

1. **Crear rama** desde `main` actualizado
```bash
   git checkout main
   git pull origin main
   git checkout -b feature/mi-funcionalidad
```

2. **Desarrollar** la funcionalidad

3. **Commit** con mensajes descriptivos
```bash
   git add .
   git commit -m "feat: add geofencing module"
```

4. **Push** a GitHub
```bash
   git push origin feature/mi-funcionalidad
```

5. **Crear Pull Request** en GitHub
   - Asignar al otro miembro del equipo como revisor
   - Descripción clara de los cambios

6. **Revisión de Código**
   - El revisor aplica el checklist de código
   - Aprueba o solicita cambios

7. **Merge**
   - Una vez aprobado: **Squash and Merge**
   - Eliminar rama automáticamente después del merge

### Formato de Commits

Usamos **Conventional Commits**:
```
tipo: descripción breve (max 72 caracteres)

Tipos válidos:
- feat: Nueva funcionalidad
- fix: Corrección de bug
- docs: Cambios en documentación
- style: Formato, punto y coma faltantes, etc
- refactor: Refactorización de código
- test: Agregar tests
- chore: Mantenimiento, dependencias

Ejemplo:
feat: add voice command support for checklist
fix: resolve battery drain issue on Android
docs: update README with installation steps
```

### Checklist de Revisión de Código

Antes de aprobar un PR, verificar:
- ✅ Probado en iOS Y Android
- ✅ Geofencing funciona en background
- ✅ Tests unitarios para lógica crítica
- ✅ Tiempo de respuesta < 2 seg en 3G
- ✅ Tokens API en variables de entorno
- ✅ ESLint pasa sin warnings

## 🚀 Instalación
```bash
# Clonar repositorio
git clone https://github.com/tu-usuario/checkout-app.git
cd checkout-app

# Instalar dependencias
npm install

# Ejecutar en iOS
npm run ios

# Ejecutar en Android
npm run android
```

## 📄 Licencia

Este proyecto es parte del curso Electiva I - UCEVA 2026
